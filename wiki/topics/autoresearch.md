# Autoresearch

Systems and methods that automate parts of the scientific research process itself — generating hypotheses,
running experiments, writing up results, reviewing and revising them, and communicating them — as opposed to
**auto-optimization**, which automates the tuning of models, systems, and code (see
[Auto-optimization](auto-optimization.md)). The organizing frame below follows the lifecycle taxonomy in
["AI for Auto-Research: Roadmap & User Guide"](../sources/ai-for-auto-research-roadmap.md) (arXiv:2605.18661):
four phases — **Creation → Writing → Validation → Dissemination** — spanning eight stages. That survey is a
map of the field, not a source of new results in its own right; the sections below are where each
subsequently-ingested paper slots in as a concrete instance, a counter-example, or a benchmark result.

A cross-cutting pattern shows up in nearly every stage below and is worth stating once: **AI is better at
producing research-shaped artifacts (ideas, code, reviews, rebuttals) than at verifying that those artifacts
are novel, faithful, executable, or scientifically meaningful.** Read each stage's papers with that gap in
mind — does the paper close it, measure it, or just add another generator?

## AI-scientist systems (end-to-end pipelines)

Systems that chain multiple lifecycle stages — typically idea generation → coding/experiments → paper
writing, sometimes extending into review — into one automated loop. The roadmap paper groups these into four
architectural families: **sequential pipelines** (simple, but error-propagating across stages — e.g. The AI
Scientist, Agent Laboratory), **search-based/self-improving systems** (tree search or evolutionary search over
research trajectories rather than one pass — e.g. AI Scientist v2, AlphaEvolve-style loops), **skill-based/
tool-integrated systems** (modular toolkits like ARIS, Biomni), and **multi-agent/community-scale systems**
(role-specialized agent societies like VirSci, ResearchTown, AgentRxiv). Across all four families, coverage of
*validation* (peer review, rebuttal) and *dissemination* lags far behind *creation* and *writing* — it is
easier to build a system that generates a paper-shaped artifact than one that is validated and communicated
with accountable fidelity.

### The AI Scientist-v2 (Sakana AI)

The [AI Scientist-v2](../sources/ai-scientist-v2.md) (Sakana AI, arXiv:2504.08066) is the system that produced
the first fully AI-generated manuscript to pass peer review — a 6.33-average-score acceptance at the ICLR 2025
ICBINB workshop, out of three submitted, later withdrawn per a pre-arranged agreement with ICLR leadership. It
supersedes The AI Scientist-v1 (Lu et al., 2024) on exactly the two axes v1 was criticized for: v1 required a
human-authored code template per topic and searched linearly (each refinement built only on its immediate
predecessor); v2 removes the template entirely and replaces linear search with **progressive agentic tree
search** — see [`agentic-tree-search`](../concepts/agentic-tree-search.md) — run across four
manager-coordinated stages (preliminary investigation, hyperparameter tuning, research-agenda execution,
ablations), with an LLM-as-judge picking the best node to seed each next stage, and a Vision-Language Model
gating nodes on plot quality. The full pipeline — idea generation (Semantic-Scholar grounded) → tree-searched
experimentation → VLM-reviewed plotting → single-pass manuscript writeup with a reasoning-model reflection
pass → LLM/VLM paper review — is this wiki's canonical example of an
[end-to-end-discovery-pipeline](../concepts/end-to-end-discovery-pipeline.md). Notably, the paper's own
internal code review of its three generated manuscripts (Appendix C) is unusually candid about failure modes
worth cross-referencing against other AI-scientist systems in this wiki: an embedding-vs-hidden-state
mislabeling in the accepted paper's method section, a caption that misdescribed a figure, 57% train/test
overlap the generated manuscript never surfaced, and — in the two rejected submissions — narrative claims
(e.g. "we applied temperature scaling") that didn't match code that was written but never executed. This
makes it a useful contrast case against Karpathy's [autoresearch](../code/autoresearch/overview.md) harness,
whose val_bpb ratchet is frozen and un-gameable precisely because it removes the LLM/VLM-as-judge step that
AI Scientist-v2 relies on at every stage.

> **Slot for later papers:** individual system papers (e.g. Agent Laboratory, CycleResearcher, Kosmos,
> Dolphin, ARIS, FARS) land here — each as its own `### <System Name>` subsection once ingested, cross-linked
> to its `wiki/sources/` page and, if a code repo is also ingested, to `wiki/code/<slug>/overview.md`.

## Self-improving research loops

Systems where the research process feeds back into itself — a run's outcome (accepted/rejected, val-metric
improved/didn't) changes what the system tries next, without a human in that inner loop. Distinct from a
one-shot AI-scientist pipeline in that the loop is the point: keep/discard decisions, evolutionary selection,
or reinforcement signals compound across iterations. Karpathy's minimal `autoresearch` harness
(edit-train-keep/discard on a fixed budget) — already ingested as a code repo, see
[autoresearch overview](../code/autoresearch/overview.md) — is the minimal single-branch instance.

### Darwin Gödel Machine — archive-based, empirically-validated self-modification

The [Darwin Gödel Machine](../sources/darwin-godel-machine.md) (DGM, arXiv:2505.22954) splices two
lineages: Schmidhuber's theoretical **Gödel machine**, which required a formal proof that a self-rewrite is
beneficial, and **Darwinian evolution**, which instead generates variation and lets empirical selection
decide after the fact. DGM keeps the Gödel machine's self-referential core — an agent that edits the very
code that constitutes its own problem-solving apparatus (tools, prompts, orchestration) — but discards the
provability requirement in favor of a benchmark-scored, archive-based search.

Its central structural move, relative to a single hill-climbing self-improver, is maintaining a **growing
archive** of every coding agent it has ever produced, with parent selection that gives every archive member —
even underperforming ones — a non-zero chance of being resampled as a **stepping stone**. The paper shows
concrete lineages where the eventual best agent passed through nodes that had temporarily regressed below
their parent's score, which a pure hill-climber would have pruned. Ablations (removing self-improvement of
the mutator itself, removing the archive, or replacing probabilistic selection with always-branch-from-best
"DGM Greedy") each underperform the full method, isolating open-ended archive exploration as a distinct,
necessary ingredient rather than an implementation detail. It raises SWE-bench Verified 20.0%→50.0% and
Polyglot 14.2%→30.7% over 80 iterations.

DGM is the **benchmarked, self-modifying cousin** of this wiki's `autoresearch` ratchet
([`../code/autoresearch/overview.md`](../code/autoresearch/overview.md)): both are keep-if-better loops
(propose → score against a fixed, hard-to-game metric → keep only if it improves → repeat), but DGM lets the
agent rewrite its *entire scaffold* (the analogue of `autoresearch`'s frozen `program.md`) and adds genuine
self-reference — the thing being evolved is also the thing doing the evolving. DGM's Appendix H objective-
hacking case (an agent deleting a hidden hallucination-detector's marker tokens to fake a perfect score,
despite an explicit instruction not to) is a concrete existence proof of the exact metric-gaming risk that
`autoresearch`'s frozen-metric/frozen-data-pipeline design is built to close off, and a direct empirical
Goodhart's-law warning for any open-ended self-improvement loop scored against an imperfect proxy — including
DGM's own. See [`evolutionary-self-improvement`](../concepts/evolutionary-self-improvement.md) and
[`self-referential-code-rewriting`](../concepts/self-referential-code-rewriting.md).

### Bilevel Autoresearch — an outer loop that meta-optimizes the inner loop's search mechanism

[Bilevel Autoresearch](../sources/bilevel-autoresearch.md) (Qu & Lu, arXiv:2603.23420) wraps this wiki's own
`autoresearch` inner loop — Karpathy's edit-train-keep/discard cycle, unmodified — in an outer loop that
treats the inner loop's **search mechanism itself** (its runner code: how it proposes, accepts, and explores
candidates) as a second, higher-level object to optimize, distinct from the training config the inner loop
already optimizes. Three nested levels: **Level 1** is the unmodified inner autoresearch loop; **Level 1.5**
adjusts search *parameters* every 5 iterations (freeze parameters proposed repeatedly with no improvement,
unfreeze stale ones, inject exploration guidance) but — the paper is explicit — "cannot change the proposal
generation logic, the acceptance criterion, or the loop structure"; **Level 2** runs a 4-round LLM dialogue
(Explore → Critique → Specify → Generate) that writes complete Python search-mechanism code and injects it
at runtime, validated by dynamic import before activation (revert on failure).

A controlled four-group ablation on Karpathy's GPT-pretraining benchmark isolates the effect: the full
bilevel system (Level 1+1.5+2) reaches −0.045 mean Δ`val_bpb`, a **~5x improvement** over the inner loop
alone (−0.009) and 7.5x over parameter-tuning-only (Level 1+1.5, −0.006, not reliably better than no outer
loop at all). Trace analysis attributes the gain to one concrete discovery — reducing `TOTAL_BATCH_SIZE`
rather than increasing it, which the LLM's default search prior systematically avoids trying — that only
the Level 2-injected mechanisms (Tabu Search blocking repeated failed proposals, Orthogonal Exploration
forcing a different parameter dimension) were able to surface; Level 1.5's parameter-freezing rule, applied
to the same failure, actually blocked the winning direction rather than finding it.

The paper draws its own sharp line, worth preserving precisely: **Level 1.5 adjusts parameters of an
existing, fixed mechanism; Level 2 generates code that replaces structural components of the mechanism
itself** — categorically different targets, not two points on one continuum. It is a **different axis of
self-modification** than either of this wiki's other self-improvement papers. Against `autoresearch`
([overview](../code/autoresearch/overview.md)): the training-code loop is untouched (still Level 1 here);
what's new is optimizing the *search procedure* that generates task candidates, not the task artifact
itself. Against the [Darwin Gödel Machine](../sources/darwin-godel-machine.md): DGM's target is the whole
agent scaffold, searched via a growing **archive** of variants, and is genuinely self-referential (the thing
being edited is the thing doing the editing). Bilevel Autoresearch's Level 2 targets only the narrower
search-mechanism component, keeps no archive (one active mechanism at a time, ratchet-style accept/revert),
and is explicitly **not yet self-referential** — Level 2 improves Level 1, but Level 2's own logic (the
4-round dialogue, the cycle periods, Level 1.5's rules) stays fixed and human-authored in this paper; the
authors name "recursive bootstrapping" of the meta-level loop itself as future work, not a result
established here. See
[`mechanism-level-self-improvement`](../concepts/mechanism-level-self-improvement.md),
[`self-referential-code-rewriting`](../concepts/self-referential-code-rewriting.md), and
[`evolutionary-self-improvement`](../concepts/evolutionary-self-improvement.md).

> **Slot for later papers:** ShinkaEvolve and similar self-improving-agent papers land here.

## Hypothesis generation and idea evaluation

Covers the roadmap's **S1 Idea Generation** stage: LLM-internal generation (direct prompting, iterative
refinement, learned quality signals), external signal-driven generation (knowledge-graph reasoning, retrieval-
grounded ideation, trend analysis), and multi-agent collaborative generation (virtual scientific communities,
critique-revision rounds). The central open problem this stage keeps surfacing is the **ideation–execution
gap**: ideas that score well on novelty before implementation degrade sharply after (Si et al. report
Δ = −1.98 for LLM ideas vs. −0.63 for human ideas), and generated-idea diversity may collapse structurally
rather than being fixable by adding more agents ("Artificial Hivemind").

Two of this wiki's systems both scale test-time compute through an iterative, judge-guided search over
candidates, but split sharply on **who executes the step that produces new evidence**:

- **[Co-Scientist](../sources/ai-co-scientist.md)** (Google, arXiv:2502.18864) generates and ranks
  hypotheses via a Generation → Reflection → Ranking (Elo tournament + scientific debate) → Evolution →
  Meta-review pipeline, entirely over text — no execution environment is in the loop. All three of its
  biomedical validations (AML drug repurposing, liver-fibrosis targets, an AMR mechanism) were confirmed by
  **human-run wet-lab experiments** outside the system; the paper names closing this into a "laboratory
  automation" loop as future work, not a current capability. See
  [`hypothesis-generation`](../concepts/hypothesis-generation.md) and
  [`multi-agent-debate`](../concepts/multi-agent-debate.md).
- **[The AI Scientist-v2](../sources/ai-scientist-v2.md)** (Sakana AI) runs its own experiments inside an
  agentic tree search — an LLM writes and executes Python, gets back real metrics/plots, and a VLM critiques
  the figures — closing the loop with no human step between hypothesis and result.

> [!inferred] The domains explain the gap more than the architectures do: AI Scientist-v2's target
> experiments are ML training runs — code a computer can execute directly — so the loop can close inside the
> agent. Co-Scientist's target experiments are physical biology (cell viability assays, organoid imaging)
> that no current agentic system can run, so the loop necessarily opens onto a human scientist. Neither
> paper draws this comparison explicitly; it is this wiki's synthesis for organizing "who actually closes
> the experiment loop" across autoresearch systems.

## Industrial R&D loop

Unlike academic AI-scientist systems aimed at novel scientific discovery (hypothesis → experiment → paper),
**RD-Agent** (Microsoft Research) targets routine, repeatable **MLE/quant-research labor** with a hard
architectural split between idea generation and implementation:

- **[RD-Agent](../sources/rd-agent.md)** formalizes this as an explicit **Research → Development** loop with
  six fixed components (FC-Planning, FC-Exploration Path Structuring, FC-Reasoning Pipeline, FC-Memory Context
  on the Research side; FC-Coding Workflow, FC-Evaluation Strategy on the Development side). Evaluated on
  **MLE-Bench** (75 real Kaggle competitions), it reaches a new SOTA of 35.1% ± 0.4% Any-Medal Rate under a
  harder-than-standard 12h/single-V100 budget, beating the prior best (ML-Master, 29.3%) — and the paper shows
  the gain is architectural rather than just a stronger backend LLM (re-running the baseline with the same
  model only reaches 16.9%).
- Its **RD-Agent(Q)** specialization instantiates the identical two-phase split for quantitative finance: five
  LLM-powered units (Specification, Synthesis, Co-STEER Implementation, Validation, Analysis) whose Analysis
  Unit uses a **contextual-bandit scheduler** to decide each round whether to optimize the factor set or the
  model — joint factor-model co-optimization beats either axis optimized alone on CSI 300/500 and NASDAQ 100.
- See [`research-development-loop`](../concepts/research-development-loop.md) for the six-component
  decomposition and [`closed-loop-experiment-design`](../concepts/closed-loop-experiment-design.md) for the
  hypothesis→implementation→validation→feedback cycle both papers share.

## Evolutionary and algorithm discovery

Search- and evolution-based methods that discover algorithms, programs, or mathematical constructions rather
than (or in addition to) writing about them — FunSearch-style program search embedded in an evolutionary loop,
AlphaEvolve-style LLM-generated mutations plus automated evaluators. The roadmap paper's framing is that these
succeed not from one-shot generation but from *coupling* generation with aggressive search, evaluation, and
selection — success comes from the search strategy as much as from the underlying model's capability.

### AlphaEvolve (DeepMind) — evolutionary code search as a research agent

[AlphaEvolve](../sources/alphaevolve.md) ([Novikov et al., arXiv:2506.13131](../../raw/papers/alphaevolve.pdf))
is the flagship instance in this wiki of a **search-based, self-improving** autoresearch system. Rather than a
single LLM pass or a linear plan→execute→report pipeline, it runs an **evolutionary outer loop**: an LLM
ensemble proposes code diffs, an automated `evaluate` function grades each child, and a MAP-elites /
island-model program database governs which survivors seed the next generation. Because grading is
programmatic code execution, the harness — not the model's self-report — enforces correctness, letting
evolution run for many generations without hallucination compounding. It represents candidates as *code* graded
by *programmatic* metrics, deliberately sidestepping the LLM-judge unreliability that
[Co-Scientist](../sources/ai-co-scientist.md) and [The AI Scientist-v2](../sources/ai-scientist-v2.md) contend
with — at the cost of applicability only to problems with automatable evaluators. It discovered a rank-48 4×4
complex matrix-multiply (first improvement over recursive Strassen in 56 years) and improved ~50 open math
problems; its production auto-optimization wins are covered in [Auto-optimization](auto-optimization.md). See
[`evolutionary-algorithm-discovery`](../concepts/evolutionary-algorithm-discovery.md).

## Auto-optimization

This wiki's second core topic (AutoML, hyperparameter optimization, NAS, learned optimizers, compiler/kernel/
schedule auto-tuning) has partial overlap with the roadmap's **S3 Coding & Experiments** stage — specifically
its coverage of experiment orchestration systems (AIDE's tree search in code space, R&D-Agent) and
systems-level optimization benchmarks (KernelBench, TritonBench) that evaluate whether LLMs can generate
efficient GPU kernels. See the dedicated [Auto-optimization](auto-optimization.md) topic page for the
learned-optimizer / NAS / kernel-autotuning literature proper; this section exists only to cross-link where
the two topics meet (an LLM agent that optimizes a kernel *is* both an auto-research coding agent and an
auto-optimization method — AlphaEvolve being the standout example).

## Open threads carried from the roadmap survey

A running list of gaps the roadmap paper (Section 7.4) flags as unresolved field-wide — useful as a lens when
reading any new autoresearch paper: does it address (a) faithfulness across phase boundaries (errors
propagating from idea → code → claim → review → rebuttal → public summary), (b) scientific-judgment/novelty
assessment beyond LLM-as-Judge scores, (c) verification/reproducibility/accountability (e.g. rebuttal
commitment-fulfillment), (d) citation/versioning/source provenance, (e) governance/disclosure norms, or
(f) cross-domain generalization beyond CS/ML/NLP? Most papers in this wiki will address one or two of these,
not all six — note which when ingesting.
