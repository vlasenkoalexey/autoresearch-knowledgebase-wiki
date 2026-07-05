# Wiki log

Append-only, chronological. One entry per operation, prefixed so it stays greppable with plain Unix
tools (`grep '^## \[' wiki/log.md | tail -5`). Prefixes: `ingest-code | <slug>` (code repo via the
skill), `ingest | <source>` (article/doc/note), `connect | <scope>` (cross-repo), `lint | <scope>`,
`note | <title>`. Newest at the bottom.

## [2026-07-04] ingest-code | autoresearch
Ingested [karpathy/autoresearch](https://github.com/karpathy/autoresearch) @ `228791f` as a submodule under
`raw/code/autoresearch`. 177 symbols, 2 modules. Wrote concept pages
[train](code/autoresearch/concepts/train.md) and [prepare](code/autoresearch/concepts/prepare.md), an
[overview](code/autoresearch/overview.md), and 4 doc-concepts from `program.md`/`README.md` (autonomous
experiment loop, experiment logging, fixed time budget, single-file agent edits). Finalize green, 100%
symbol coverage (7/7 classes). Adversarial verify caught and fixed one error (Muon momentum is
step-indexed, not `progress`-indexed). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | tpu-performance-autoresearch-wiki
Ingested the methodology layer of [vlasenkoalexey/tpu_performance_autoresearch_wiki](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki)
@ `3344c6a` — README, SCHEMA, sample-program.md, the optimization blueprint + index, and all 8 procedural
skills (`create-experiment`, `formulate-hypothesis`, `start-experiment`, `stop-experiment`,
`create-retrospective`, `ingest-source`, `edit-model-code`, `lint`), clipped verbatim into
`raw/papers/tpu-performance-autoresearch-wiki/`. Deliberately skipped: ~26 ingested reference codebases
(`wiki/codebases/`), 900+ per-model experiment logs (`wiki/experiments/`), and TPU-domain technical content
(`wiki/concepts/`, `wiki/sources/`) — implementation, not methodology. Wrote
[wiki/sources/tpu-performance-autoresearch-wiki.md](sources/tpu-performance-autoresearch-wiki.md) (summary)
and [wiki/topics/wiki-driven-autoresearch-loop.md](topics/wiki-driven-autoresearch-loop.md) (synthesis
against `karpathy/autoresearch`). Cross-linked from
[code/autoresearch/overview.md](code/autoresearch/overview.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | vlasenkoalexey-blog-autoresearch-series
Ingested the last 3 posts from [vlasenkoalexey/vlasenkoalexey.github.io](https://github.com/vlasenkoalexey/vlasenkoalexey.github.io/tree/main/_posts)
@ `010a622` (2026-05-01, 2026-06-05, 2026-06-26) — the author's own narrative of the
`tpu_performance_autoresearch_wiki` project: initial case studies (Llama 3 8B vs. MaxText; Qwen3 8B
four-harness comparison), the context-pollution diagnosis behind loop unreliability and its `/loop`
Stop-hook + retrospective fixes, and the later skill-vs-sub-agent decomposition (+ sub-wiki scoping +
hypothesis-firing audit) that made the loop portable across Claude Code/Codex/Antigravity. Raw clips in
`raw/papers/2026-0{5,6}-*.md`. Wrote 3 summary pages under `wiki/sources/` and substantially extended
[wiki/topics/wiki-driven-autoresearch-loop.md](topics/wiki-driven-autoresearch-loop.md) with the
context-pollution/decomposition generalization and cross-harness evidence. Registered in
[`index.md`](index.md).

## [2026-07-04] ingest | ai-for-auto-research-roadmap
Downloaded arXiv:2605.18661 ("AI for Auto-Research: Roadmap & User Guide", 18 May 2026) to
`raw/papers/ai-for-auto-research-roadmap.pdf` and read all 65 pages. Wrote
[wiki/sources/ai-for-auto-research-roadmap.md](sources/ai-for-auto-research-roadmap.md) summarizing its
4-phase/8-stage lifecycle taxonomy (Creation→Writing→Validation→Dissemination), 5 methodological families,
5 central findings (verification lags generation; human-governed collaboration beats full autonomy; layered
architectures win; governance is the bottleneck), and 6 open-challenge themes. This paper's structural role
seeded the new [wiki/topics/autoresearch.md](topics/autoresearch.md) scaffold. Part of a 6-paper parallel
pass (Sonnet 5 subagents). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | ai-scientist-v2
Downloaded arXiv:2504.08066 ("The AI Scientist-v2", Sakana AI) to `raw/papers/ai-scientist-v2.pdf` and read
it in full including the annotated appendices. Wrote
[wiki/sources/ai-scientist-v2.md](sources/ai-scientist-v2.md) covering progressive agentic tree search, the
four manager-coordinated stages, template removal vs. v1, the end-to-end pipeline, the first-AI-paper
peer-review milestone (6.33 avg, ICLR 2025 workshop; later Nature), and the paper's own candid failure-mode
audit. Seeded concept pages [agentic-tree-search](concepts/agentic-tree-search.md) and
[end-to-end-discovery-pipeline](concepts/end-to-end-discovery-pipeline.md), and added a subsection to
[topics/autoresearch.md](topics/autoresearch.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | ai-co-scientist
Downloaded arXiv:2502.18864 (Google Co-Scientist, v2 "Accelerating scientific discovery with Co-Scientist")
to `raw/papers/ai-co-scientist.pdf` and read it. Wrote
[wiki/sources/ai-co-scientist.md](sources/ai-co-scientist.md): the six-agent Gemini architecture
(Generation/Reflection/Ranking/Proximity/Evolution/Meta-review), Elo-tournament + scientific-debate ranking,
test-time-compute scaling, three human-confirmed biomedical validations, and the explicit stop at hypothesis
generation (no autonomous experimentation) — the key contrast with AI Scientist-v2 on "who closes the loop."
Seeded [hypothesis-generation](concepts/hypothesis-generation.md) and
[multi-agent-debate](concepts/multi-agent-debate.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | rd-agent
Ingested two companion Microsoft papers as one project: the general R&D-Agent framework (arXiv:2505.14738,
MLE-Bench SOTA 35.1% Any-Medal Rate) → `raw/papers/rd-agent.pdf`, and RD-Agent(Q) (arXiv:2505.15155, NeurIPS
2025) → `raw/papers/rd-agent-quant.pdf`, which specializes the Research/Development split into a five-unit
quant-finance pipeline with a contextual-bandit factor/model scheduler. Wrote
[wiki/sources/rd-agent.md](sources/rd-agent.md) and seeded
[research-development-loop](concepts/research-development-loop.md) and
[closed-loop-experiment-design](concepts/closed-loop-experiment-design.md); added the "Industrial R&D loop"
section to [topics/autoresearch.md](topics/autoresearch.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | darwin-godel-machine
Downloaded arXiv:2505.22954 ("Darwin Gödel Machine") to `raw/papers/darwin-godel-machine.pdf` and read it.
Wrote [wiki/sources/darwin-godel-machine.md](sources/darwin-godel-machine.md): the archive-based,
empirically-validated self-modification loop (SWE-bench 20→50%, Polyglot 14.2→30.7% over 80 iters), the
stepping-stone selection ablations, and the Appendix-H objective-hacking case as a Goodhart warning. Seeded
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md) and
[self-referential-code-rewriting](concepts/self-referential-code-rewriting.md), framing `autoresearch` as the
archive-size-1, non-self-referential special case. Registered in [`index.md`](index.md).

## [2026-07-04] ingest | alphaevolve
Downloaded arXiv:2506.13131 ("AlphaEvolve", DeepMind) to `raw/papers/alphaevolve.pdf` and read all 44 pages.
Wrote [wiki/sources/alphaevolve.md](sources/alphaevolve.md): the LLM-driven evolutionary code-search loop
(FunSearch successor, MAP-elites/island database, programmatic `evaluate`), its provably-correct discoveries
(rank-48 4×4 complex matmul; ~50 open math problems) and four production auto-optimization wins (Borg
scheduling, Gemini kernels, TPU RTL, XLA IR). Seeded
[evolutionary-algorithm-discovery](concepts/evolutionary-algorithm-discovery.md); flagged as the bridge
between [topics/autoresearch.md](topics/autoresearch.md) and
[topics/auto-optimization.md](topics/auto-optimization.md) (new stub). Registered in [`index.md`](index.md).

## [2026-07-04] ingest-code | ai-scientist-v2
Ingested [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) @ `96bd516` as a submodule
under `raw/code/ai-scientist-v2` — the implementation behind the paper source
[sources/ai-scientist-v2.md](sources/ai-scientist-v2.md). 785 documentable symbols across 33 modules; 15 deep
concept pages + 5 README doc-concepts; finalize green, 100% symbol coverage (32/32 classes). Core pages:
[ParallelAgent](code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) (agentic tree search),
[AgentManager](code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md) (four-stage protocol),
[Journal & Node](code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md) (experiment tree data model),
[ideation](code/ai-scientist-v2/concepts/ai_scientist-perform_ideation_temp_free.md),
[interpreter](code/ai-scientist-v2/concepts/ai_scientist-treesearch-interpreter.md), and
[writeup](code/ai-scientist-v2/concepts/ai_scientist-perform_icbinb_writeup.md);
[overview](code/ai-scientist-v2/overview.md). Adversarial verify on the 5 core mechanism pages caught and fixed
3 errors: AgentManager stage identity is carried by a `stage_number` int field (not purely the `name` string);
the writeup's citation persistence lives in `gather_citations`'s loop (not `get_citation_addition`); and the
interpreter re-sends `SIGINT` each ~1s poll (not once). Registered in [`index.md`](index.md). Connect step next.

## [2026-07-04] connect | 4 concepts wired across 2 repos
Connected `ai-scientist-v2` on the concept axis via `wikify connect --apply`. Wired 4 authoritative
tag-matched vocabulary concepts down to their grounded implementations (and up-linked each silo page):
[agentic-tree-search](concepts/agentic-tree-search.md) → ParallelAgent + AgentManager + Journal/Node;
[end-to-end-discovery-pipeline](concepts/end-to-end-discovery-pipeline.md) → launch_scientist_bfts;
[closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → same three tree-search pages;
[hypothesis-generation](concepts/hypothesis-generation.md) → ideation. Added hub prose above the `connect:auto`
blocks on the two headline concepts framing the tree-search-plus-LLM/VLM-judge path against `autoresearch`'s
frozen-metric ratchet. Left the other 6 vocabulary concepts unconnected (this repo doesn't implement them).

## [2026-07-04] ingest | bilevel-autoresearch
Ingested Qu & Lu, "Bilevel Autoresearch: Meta-Autoresearching Itself" (arXiv:2603.23420) →
`raw/papers/bilevel-autoresearch.pdf`. An outer loop wraps this wiki's own `autoresearch` inner loop
(unmodified) and, at runtime, reads its runner code + search trace and injects new Python search-mechanism
code (Tabu Search, multi-armed bandit, orthogonal design-of-experiments); ~5x val_bpb gain over the inner
loop alone vs. no reliable gain from parameter-only tuning. Wrote
[wiki/sources/bilevel-autoresearch.md](sources/bilevel-autoresearch.md), seeded new concept
[mechanism-level-self-improvement](concepts/mechanism-level-self-improvement.md), added contrastive cross-links
to [self-referential-code-rewriting](concepts/self-referential-code-rewriting.md) and
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md), and added a "Bilevel Autoresearch"
subsection to [topics/autoresearch.md](topics/autoresearch.md). Its codebase
([EdwardOptimization/Bilevel-Autoresearch](https://github.com/EdwardOptimization/Bilevel-Autoresearch)) is
queued for code ingest (after `dgm`). Registered in [`index.md`](index.md).

## [2026-07-04] ingest-code | rd-agent
Ingested [microsoft/RD-Agent](https://github.com/microsoft/RD-Agent) @ `4f9ecb0` as a submodule under
`raw/code/rd-agent` — the implementation behind the paper source [sources/rd-agent.md](sources/rd-agent.md)
(the general R&D-Agent framework + RD-Agent(Q)). 6226 documentable symbols across 541 modules (100%
represented, 592/592 classes); 24 deep concept pages + 6 README doc-concepts; finalize green. Core pages:
[LoopBase](code/rd-agent/concepts/rdagent-utils-workflow-loop.md) (the generic `while time remains` engine
realizing Algorithm 1), [Hypothesis/Trace/ExpGen](code/rd-agent/concepts/rdagent-core-proposal.md) +
[DSTrace + schedulers](code/rd-agent/concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) (the
Research phase), [Experiment/Workspace/Task](code/rd-agent/concepts/rdagent-core-experiment.md) (the shared
currency), the Co-STEER coding agent ([evolving framework](code/rd-agent/concepts/rdagent-core-evolving_framework.md),
[evaluators](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-evaluators.md),
[knowledge management](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)),
[Env](code/rd-agent/concepts/rdagent-utils-env.md) sandbox, and the
[RDAgentTimer](code/rd-agent/concepts/rdagent-log-timer.md); [overview](code/rd-agent/overview.md).
Adversarial verify on 8 core mechanism pages caught and fixed 4 errors: `withdraw_loop` reloads the
*earliest* (min step-index) dump of the previous loop, not the last (`loop.py:408`); the `-1`→`len-1`
index translation lives in `get_sota_experiment`, not `get_parents` (`proposal.py:309`); only the three
`ExpGen2TraceAndMerge*` dispatchers gate on `merge_hours` (the inner `MergeExpGen`/`ExpGen2Hypothesis`
recombine unconditionally); and `MCTSScheduler` scores over *every* recorded node index while only
`ProbabilisticScheduler` restricts to `get_leaves()` (`trace_scheduler.py:365`). Registered in
[`index.md`](index.md). Connect step next (3rd silo).

## [2026-07-04] connect | 2 concepts wired across 2 repos (rd-agent joined)
Connected `rd-agent` on the concept axis via `wikify connect --apply`. Wired the two strong, tag-matched
vocabulary concepts down to rd-agent's grounded implementations (and up-linked each silo page):
[research-development-loop](concepts/research-development-loop.md) → 10 rd-agent pages (LoopBase, the
Experiment/Task/Trace core, the Co-STEER coder+evaluators+knowledge-mgmt, Env) — RD-Agent is this concept's
canonical instance; [closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → refreshed to
span BOTH repos (8 rd-agent + the 3 existing ai-scientist-v2 tree-search pages). Added hub prose to
`closed-loop-experiment-design` contrasting RD-Agent's explicit Research→Development split (feedback = a
recorded `Trace` driving the next proposal) against ai-scientist-v2's in-tree LLM/VLM-verdict feedback.
Deliberately left rd-agent's other two tag matches — `agentic-tree-search` and `hypothesis-generation` —
unconnected (preferring the two strong matches; connecting everything drowns the pages, per SCHEMA).

## [2026-07-04] ingest-code | pi-autoresearch-vkf
Ingested [EricJahns/pi-autoresearch-vkf](https://github.com/EricJahns/pi-autoresearch-vkf) @ `cd8085d`
(`v0.10.0-9-gcd8085d`) as a submodule under `raw/code/pi-autoresearch-vkf` — a `pi` coding-agent extension
(TypeScript) that turns a blind optimization loop into a self-improving researcher with verifiable long-term
memory (VKF). 746 symbols across 27 modules (100% represented, 72/72 classes); 14 concept pages (autonomy
watchdog, VKF cards, session config, context pruning, terminal dashboard, experiment log, frontmatter
parser, the tool spine, workspace layout, dashboard payload assembly, idea scoring, hypothesis synthesis,
the experiment search tree, the vkf CLI bridge) + 5 README/CLAUDE.md doc-concepts (skills architecture, tool
reference, benchmark methodology, browser dashboard export, configuration env vars). Finalize green on the
first full pass (a dozen dead module-namespace citations — a packet-generation quirk where `Namespace`-kind
symbols aren't in the coverage-documentable set — were de-linked to plain page references rather than
symbol anchors). Adversarial verify (5 parallel passes, one per page-group) checked all 218 load-bearing
claims and refuted/fixed ~24: notably confirmed as *true* (not refuted) the page's central claim that
`selectExpansion` never calls `frontier` — this implementation always hill-climbs from the single current
best node rather than expanding a multi-node frontier, unlike AIDE/The AI Scientist v2's tree search: a real,
citable design contrast, not a bug. Also fixed a `paths.ts` claim that `dashboard.ts`'s top-level exports read
"exclusively through `sessionPaths`" — they also route through `memoryPaths` via `listCards`/`memoryCounts`,
directly contradicting the module's own "two halves mirror the architecture" docstring. Registered in
[`index.md`](index.md). Connect step next (4th silo).

## [2026-07-04] connect | 4 concepts wired across 4 repos (pi-autoresearch-vkf joined)
Connected `pi-autoresearch-vkf` (4th silo) via `wikify connect --apply`, using its own `concepts:` frontmatter
tags (applied during synthesis, not guessed post hoc): [agentic-tree-search](concepts/agentic-tree-search.md)
→ +3 pi-autoresearch-vkf pages (tree.ts, experiments.ts, index.ts) alongside ai-scientist-v2's 3;
[research-development-loop](concepts/research-development-loop.md) → +2 (config.ts, index.ts) alongside
rd-agent's 10; [closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → +4 (cards.ts,
scoring.ts, tree.ts, index.ts), now spanning all 3 code silos; [hypothesis-generation](concepts/hypothesis-generation.md)
→ +1 (synthesis.ts) alongside ai-scientist-v2's ideation page. Deliberately excluded rd-agent's two
`agentic-tree-search`/`hypothesis-generation` tag matches from those two concepts (via `--exclude`), preserving
the prior connect pass's decision to keep those two selective — but this required a two-call sequence
(`--apply research-development-loop,closed-loop-experiment-design` first with no exclude, then
`--apply agentic-tree-search,hypothesis-generation --exclude <rd-agent's 2 paths>` second) plus a manual fix:
the second call's per-(repo,path) `--exclude` blanket-dropped those same 2 rd-agent pages from *all* keys'
up-block regeneration that call (not just the 2 being applied), silently deleting their
`closed-loop-experiment-design`/`research-development-loop` up-links even though those concepts' down-blocks
(untouched that call) still correctly listed them — a real tool-mechanics gap between `--exclude`'s per-call,
per-(repo,path) scope and the intended per-(repo,path,key) exclusion. Manually restored both up-blocks to
match their down-block state. Did **not** connect `mechanism-level-self-improvement` — no
pi-autoresearch-vkf page was tagged with it (the VKF layer operates the search mechanism, it doesn't optimize
it, so the tag was correctly withheld during synthesis) — nor `end-to-end-discovery-pipeline` (no manuscript/
figures pipeline here). Added hub prose on all 4 connected concept pages: `agentic-tree-search` gets the
sharpest contrast — a source-verified finding that `selectExpansion` never calls `frontier`, so unlike
ai-scientist-v2's multi-node frontier expansion this implementation always hill-climbs from a single best
node; `research-development-loop` contrasts RD-Agent's six fixed components against pi-autoresearch-vkf's
single optimize/ideate config fork; `closed-loop-experiment-design` extends the existing 2-repo comparison to
a 3-way axis (live tree state vs. recorded Trace vs. durable trust-gated VKF card store);
`hypothesis-generation` contrasts Co-Scientist/ai-scientist-v2's LLM-mediated generation against
pi-autoresearch-vkf's deterministic contradiction/transfer/composition mining over already-verified memory.

## [2026-07-05] ingest-code | dgm
Ingested [jennyzzt/dgm](https://github.com/jennyzzt/dgm) @ `a565fd2d1d` (the **Darwin Gödel Machine**,
arXiv:2505.22954) as a submodule under `raw/code/dgm` — the 5th code silo, and the implementation behind the
paper source [`sources/darwin-godel-machine.md`](sources/darwin-godel-machine.md). 371 documentable symbols
across 37 modules (100% represented, 10/10 classes); 9 concept pages + 3 README doc-concepts. Auto-discovery
seeded 7 concepts; added 2 config seed concepts (`DGM_outer`, `self_improve_step`) so the archive/parent-
selection loop and the self-referential edit-and-validate step each got a deep page. Concept pages: the outer
archive loop (`DGM_outer` — stepping-stone `score_child_prop` parent sampling + `keep_all` archive growth),
one self-improvement attempt (`self_improve_step` — diagnose → container-run the agent to self-edit →
re-score on SWE-bench/Polyglot), the coding agent being evolved (`coding_agent`), model-agnostic tool-calling
(`llm_withtools`), the diagnosis-prompt builder (`prompts-self_improvement_prompt`), the bash tool
(`tools-bash`), per-framework test-log parsing (`utils-swe_log_parsers`), the Polyglot Docker image pipeline
(`polyglot-docker_build`), and offline lineage plotting (`analysis-visualize_archive`). Finalize green on the
second pass (first pass hit 4 lint errors — 2 `filter_compiled` citations outside the DGM_outer subgraph,
de-linked to plain-name references; 2 uncited Mechanism steps, re-cited to in-subgraph `main`/`choose_selfimproves`
and one demoted to `[!inferred]`). Adversarial verify (parallel, all 120 load-bearing claims across 9 pages)
refuted + fixed 3: `DGM_outer`'s `best` method sorts *ascending* (takes the lowest scorers — an apparent
upstream bug, now noted in-page rather than described as "top scorers"); `polyglot-docker_build` over-claimed
that `build_instance_image` cascade-removes downstream images (only `get_env_configs_to_build` does, via
`find_dependent_images`); `analysis-visualize_archive` claimed lineage edges are colored by score direction,
but the source renders all edges black (the color code is commented out — only edge *thickness* distinguishes
the lineage). Manually confirmed the load-bearing `coding_agent` claim that `self.self_improve` is nearly
inert (its only use is forcing `instance_id='dgm'` at coding_agent.py:84; `forward()` never branches on it —
the self-referential effect comes entirely from `self_improve_step.py` pointing the agent at DGM's own repo).
Registered in [`index.md`](index.md). Connect step next (5th silo).

## [2026-07-05] connect | 2 concepts wired to dgm (5th silo joined)
Connected `dgm` (5th silo) via `wikify connect --apply self-referential-code-rewriting,evolutionary-self-improvement`
— using dgm's own `concepts:` frontmatter tags (applied during synthesis). Both are DGM-exclusive concepts (no
other silo implements them, correctly): [self-referential-code-rewriting](concepts/self-referential-code-rewriting.md)
→ 3 dgm pages (coding_agent, self_improve_step, prompts-self_improvement_prompt);
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md) → 1 dgm page (DGM_outer). Up-link
blocks written on all 4 dgm silo pages. Added hub prose to both concept pages above their auto blocks:
`evolutionary-self-improvement` now lays out the four-silo ladder ratchet (autoresearch) → single-node
hill-climb (pi-autoresearch-vkf) → best-first tree (ai-scientist-v2) → genuine growing archive (dgm), noting
only DGM keeps every viable variant selectable; `self-referential-code-rewriting` pins down where the
self-reference actually lives (the agent's self_improve flag is nearly inert — the effect is an emergent
wiring effect in self_improve_step pointing the generic agent at its own code) and notes even DGM leaves its
own outer archive loop human-owned. Deliberately did NOT connect `mechanism-level-self-improvement` (no dgm
page tagged it — DGM's outer loop is fixed, not itself optimized, so the tag was correctly withheld) nor any
of the 5 already-connected concepts (dgm implements none of them — not a candidate for any). **Known `--exclude`/
up-link-regeneration bug hit again (differently):** the `--apply` run regenerated ALL silos' up-link blocks
from page frontmatter tags, re-adding `agentic-tree-search` + `hypothesis-generation` up-links to two rd-agent
pages (rdagent-core-proposal, rdagent-scenarios-data_science-proposal-exp_gen-base) even though those two
concepts' down-blocks deliberately exclude rd-agent (the 2026-07-04 pass kept them selective). Since the
regeneration keys off the page's `concepts:` tags rather than actual down-block membership, it re-introduced
the exact links the prior pass had pruned. Restored both rd-agent up-link blocks to their committed
2-concept state (`closed-loop-experiment-design`, `research-development-loop`) and re-ran `wikify finalize
rd-agent` (green, 6226 symbols 100%). ai-scientist-v2 and pi-autoresearch-vkf up-links were untouched (their
tags match their down-block membership). dgm finalize re-confirmed green after connect (371 symbols, 100%).
