# Wiki-driven autoresearch loop

A pattern for autonomous, unattended optimization: an LLM agent iterates hypothesize → experiment →
observe → revise against a fixed, cheap, comparable unit of experimentation, while a persistent markdown
wiki (not a vector store) accumulates the priors that make each new hypothesis better than the last. This
page synthesizes two instances of the pattern currently in this knowledge base — the seed idea and a
much larger generalization of it — and extracts what's common across both.

## The two instances

| | [karpathy/autoresearch](../code/autoresearch/overview.md) | [tpu_performance_autoresearch_wiki](../sources/tpu-performance-autoresearch-wiki.md) |
|---|---|---|
| Optimizes | model *quality* (loss) | model *performance* (step time, MFU, tokens/sec, memory) |
| Objective metric | `val_bpb` (bits/byte, vocab-independent) — [prepare.py](../code/autoresearch/concepts/prepare.md) | MFU / step time / memory, read off a real profiler |
| Fixed experimental unit | a wall-clock 5-minute training run — [the fixed time budget](../code/autoresearch/doc-concepts/fixed-time-budget.md) | one experiment testing one hypothesis on one `(size, hardware)` variant |
| Mutable vs. frozen | one file (`train.py`) mutable; `prepare.py` (data + metric) frozen — [single-file agent edits](../code/autoresearch/doc-concepts/single-file-agent-edits.md) | a per-experiment git fork/branch is mutable; the evaluation discipline (no semantics drift) is invariant |
| The observer | the frozen `evaluate_bpb` function, called in-process | XProf (OpenXLA's TPU profiler) wrapped as an MCP server, called by the agent as a tool |
| Ledger | one flat `results.tsv` row per run — [experiment logging](../code/autoresearch/doc-concepts/experiment-logging.md) | eight page types (source / codebase / concept / model / hypothesis / experiment / observation / analysis), each schema-templated and cross-linked |
| Ranking | none — single active branch, keep/revert | hypotheses ranked by `expected_gain × confidence / effort`; "next hypotheses" mandatory per experiment |
| Autonomy safeguard | fast-fail NaN/loss guard aborts a bad run in seconds — [train.py — edge cases](../code/autoresearch/concepts/train.md) | a Stop-hook gate blocks the session from ending in never-stop mode until a fresh retrospective exists — see [methodology summary](../sources/tpu-performance-autoresearch-wiki.md) |
| Exhaustion handling | none stated (`program.md` just says keep thinking harder) | a dedicated retrospective skill re-reads the *entire* experiment history before the agent is allowed to declare a search exhausted |
| Loop decomposition | none — a single flat `program.md` prompt, single session | one monolithic per-iteration prompt originally, later split into skills (shared context: `formulate-hypothesis`, `edit-model-code`) and sub-agents (isolated context: `gke-cluster-runner`, `profile-analyzer`) once it needed to run reliably on weaker models — see [2026-06-26 post](../sources/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md) |

## What generalizes

**A fixed, fair, cheap unit of comparison is the load-bearing design choice in both.** `autoresearch`
achieves it with a wall-clock time budget so *any* code change is automatically priced by the throughput
it costs; the TPU wiki achieves it with a pinned `(size, hardware)` variant row and a frozen
no-semantics-drift invariant. Either way, the trick is the same: make "did this help" a comparison the
agent cannot win by cheating, so autonomy doesn't require constant human auditing of *individual* results
— only of the substrate that makes results comparable.

**A domain-grounded observer is what keeps the loop from degenerating into guessing.** `autoresearch`'s
observer is a single frozen eval function; the TPU wiki's is a full profiler exposed as MCP tools. The TPU
wiki states this generalization explicitly: without a real-signal observation step, "hypothesize →
experiment → observe → revise" collapses into flag-guessing — the observer is what raises the
signal-to-noise of every iteration (see [methodology summary](../sources/tpu-performance-autoresearch-wiki.md)).
This is a claim worth carrying into *any* future auto-optimization source this wiki ingests: the interesting
design question for a new domain is rarely the search strategy, it's *what grounded signal plays the role
of the observer*.

**Falsifiability and pre-registration compound better than post-hoc justification.** Both systems commit to
an expected outcome before running: `autoresearch` doesn't formalize this beyond "did the loss go down,"
but the TPU wiki makes it explicit machinery — every hypothesis states its falsification criterion up
front, and cheap pre-flight checks (an HLO pre-filter, an AOT cost-analysis screen) are used to refute
hypotheses on a compiler pass *before* spending a real run, mirroring the cheaper end of `autoresearch`'s
own fast-fail instinct (abort a diverging run in seconds rather than let it burn the whole time budget).

**Unattended loops need an explicit accountability mechanism, not just a policy.** `autoresearch`'s
`program.md` states "NEVER STOP" as an instruction the agent is trusted to follow. The TPU wiki instead
*enforces* a version of this with a Stop hook that mechanically blocks session termination unless a
recent, lane-specific retrospective exists — turning "keep going" from a policy into a gate. The
retrospective itself exists because of a documented failure mode: a search declared exhausted, and a
real win landed a week later once someone looked harder. The generalizable lesson is that "I'm out of
ideas" is a claim that should require evidence (a coverage audit against a known taxonomy of what *could*
be tried), not just be taken at the agent's word.

**The root cause of every reliability failure the TPU wiki's author found was context pollution, in two
different shapes.** First shape: governing instructions sit at the top of a session's context and sink
further down every turn, until a long enough session gives them less effective weight than everything
accumulated on top — the fix is external, periodic re-injection (`/loop`), because an in-context
instruction to "remember to re-read yourself" degrades under the exact pollution it's meant to fix. Second
shape: even with instructions kept on top, a single per-iteration prompt that reads ten wiki pages,
inspects prior experiments, edits code, launches a job, polls it, and analyzes a profile all in one
context overloads weaker models into skipping steps — the fix there is decomposition, not reinforcement.
Strong models can compensate for pollution with sheer context headroom; the general lesson does not depend
on having a strong model available (see [2026-06-05](../sources/2026-06-05-making-karpathy-autoresearch-production-ready.md)
and [2026-06-26](../sources/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)).

**Decomposition into skills (shared context) vs. sub-agents (isolated context) is the general fix for the
second pollution shape.** The dividing line: if the master needs to remember the work for its next
decision, keep it a skill; if the work would burn tens of thousands of tokens of intermediate state the
master doesn't need (cluster polling logs, raw profiler output), isolate it in a sub-agent and return only
a synthesized summary. Paired with this is **sub-wiki scoping** — force a component to load only its own
curated slice of the wiki (an optimization index for hypothesis proposal, a separate profiler/HLO reference
for profile interpretation) rather than trust the agent to select the right pages from the whole thing.
Neither idea is TPU-specific; both apply to any agentic loop whose per-iteration prompt has grown to do
more than one job.

**Verify the predicted mechanism actually fired — don't just measure the outcome metric.** The TPU wiki's
`profile-analyzer` sub-agent runs a "hypothesis-firing audit": it checks the HLO dump for structural
evidence that the change under test actually took effect (e.g., does the intended kernel really appear as
a `custom_call`), and downgrades the verdict to inconclusive if not. Before this check, a silent no-op — a
compiler optimizing away the change, or a flag that never took effect — could get recorded as a genuine win
on a lucky noise sample. This generalizes past profiling specifically: any autoresearch loop whose
observer only reads a final scalar (not the mechanism that's supposed to produce it) is vulnerable to the
same silent-no-op failure mode.

**Portability across models/harnesses is itself evidence for a methodology, not just a nice-to-have.** A
four-way head-to-head on the same model/hardware/skills/sub-agents (Codex + GPT-5.5, Claude Code + Fable 5,
Claude Code + Opus 4.8, Antigravity + Gemini 3.1 Pro) had all four run the loop unattended and file real
experiment trails, with two of four autonomously beating an optimized reference implementation (see
[2026-06-26](../sources/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)). The
author's own framing: the point isn't which model won, it's that the *specialization into skills and
sub-agents* — not any one model's superiority — is what let all four run the loop at all. That's a useful
signal for judging any future auto-optimization methodology this wiki ingests: does it hold up across more
than one underlying model, or was it only ever validated on the strongest model available?

**A ledger that only records outcomes is thinner than one that records structure.** `autoresearch`'s
`results.tsv` (commit, score, memory, status, one-line description) is sufficient for a single-file,
single-metric loop. Once the search space has multiple models, multiple hardware targets, and multiple
technique families, the TPU wiki's schema shows what has to be added to keep the ledger useful: a ranked,
falsifiable hypothesis *queue* (not just a log of what was tried), a cross-variant "does this technique
transfer" matrix, and a mandatory "what does this motivate next" field on every completed run — the
structure needed to keep a large search from re-deriving its own history by accident.

## See also
- [karpathy/autoresearch — overview](../code/autoresearch/overview.md)
- [tpu_performance_autoresearch_wiki — methodology summary](../sources/tpu-performance-autoresearch-wiki.md)
- [TPU Model Performance Auto-optimization (blog, 2026-05-01)](../sources/2026-05-01-tpu-model-performance-auto-optimization.md)
- [Making Karpathy's autoresearch production-ready (blog, 2026-06-05)](../sources/2026-06-05-making-karpathy-autoresearch-production-ready.md)
- [Making TPU auto-optimization work with other agents (blog, 2026-06-26)](../sources/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)
