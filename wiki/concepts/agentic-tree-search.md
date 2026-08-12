# Agentic tree search

**Definition.** Agentic tree search is a method for structuring open-ended LLM-driven experimentation as a
search over a tree of experiment attempts ("nodes"), rather than a single linear chain of edits. Each node
bundles an experiment script, the LLM's plan for it, an execution trace (or error), runtime, metrics, LLM
feedback, a plotting script, figure paths, VLM feedback on those figures, and a final buggy/non-buggy status.
Expansion is parallel (several nodes expanded concurrently each iteration) and choice of what to expand next
is itself LLM-mediated: a fixed probability biases the search toward debugging existing buggy nodes, and
otherwise a **best-first search over non-buggy nodes** is guided by an LLM judge weighing performance metrics,
training dynamics, and plot quality.

**How The AI Scientist-v2 implements it.** [The AI Scientist-v2](../sources/ai-scientist-v2.md) (Sakana AI,
arXiv:2504.08066) introduces this as the replacement for its predecessor's strictly linear search, where each
code refinement built only on the immediately preceding experiment (source, p.5 §3.2.2, p.3 §2). The search runs
under a dedicated **experiment progress manager agent** that partitions the whole project into four sequential
stages — preliminary investigation, hyperparameter tuning, research-agenda execution, ablation studies — each
with its own stopping criterion (a working prototype; convergence across ≥2 datasets; budget exhaustion; budget
exhaustion), and the manager promotes the single best node (chosen by an LLM evaluator) from one stage to seed
the next, additionally spinning up replication runs for statistics (source, p.4–5 §3.2.1). Beyond generic
buggy/non-buggy nodes, the tree has four specialized node kinds: **hyperparameter nodes** and **ablation nodes**
(each tracking prior configurations tried, to avoid redundant work), **replication nodes** (same experiment,
different seed, for mean/std statistics), and **aggregation nodes** (no new experiment — just a script that
combines replication-node outputs into one summary figure) (source, p.7). A node is marked buggy either from a
Python execution error, or — critically — if a Vision-Language Model reviewing its generated plot flags issues
like missing legends or misleading visualization, even when the code ran without error (source, p.5). Per Table
3 (source, p.21), Stage 1 gets 21 nodes and Stages 2–4 get 12 each, debug probability is 1.0, max debug depth 3,
and per-node runtime is capped at 1 hour, with a full paper run taking up to 15 hours; code-generation itself
used Claude 3.5 Sonnet (v2), with GPT-4o driving the LLM/VLM feedback and summary agents (source, Table 2, p.21).

**Why it matters.** Tree search over LLM-generated code turns "did this experiment work" into a *branching*
question instead of a linear one — the system can abandon a bad direction and backtrack to any earlier
non-buggy node rather than being stuck compounding a flawed baseline, which the paper credits as the main reason
v2 could remove the human-authored template dependency that constrained v1 (source, p.1, p.4 §3). The tradeoff,
visible in the paper's own annotated appendix (source, p.41–44), is that the judge making "is this node good"
calls is itself an LLM/VLM — the accepted workshop paper's regularizer description, dataset overlap, and a
figure caption all slipped past this judge even though the search "succeeded" by its own criteria, which is a
useful case study for anyone comparing agentic-search-based systems against harnesses (like
[autoresearch](../code/autoresearch/overview.md)) that instead freeze the evaluation metric itself.

## See also
- [`end-to-end-discovery-pipeline`](end-to-end-discovery-pipeline.md)
- [`../sources/ai-scientist-v2.md`](../sources/ai-scientist-v2.md)
- [`../topics/autoresearch.md`](../topics/autoresearch.md)

## Grounded in code
The paper-side mechanism above is now grounded in the ingested [ai-scientist-v2](../code/ai-scientist-v2/overview.md)
source. The mechanism splits across three pages: the search engine itself — best-first-vs-debug-probability node
selection, parallel worker execution, and the LLM-plus-VLM double verdict — is
[ParallelAgent](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md); the fixed four-stage
protocol that wraps it (promote-best-node, replication runs) is
[AgentManager](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md); and the node/tree data
model both read and write is [Journal & Node](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md).
A verified detail the code makes concrete: a node is `good` only if **both** `is_buggy` (LLM verdict on the run)
and `is_buggy_plots` (independent VLM verdict on the figures) are false — a clean-exiting script with a bad plot is
still rejected. This is the design foil to Karpathy's [autoresearch](../code/autoresearch/overview.md), which
freezes the evaluation metric instead of trusting a learned judge (see [`../topics/autoresearch.md`](../topics/autoresearch.md)).

## A narrower instance: pi-autoresearch-vkf

[pi-autoresearch-vkf](../code/pi-autoresearch-vkf/overview.md) is the fourth silo in this wiki and the one that
most explicitly cites this pattern: its own CHANGELOG says v0.9.0 was "Inspired by agentic tree-search (AIDE,
The AI Scientist v2)." The core idea transfers — experiments are nodes with a `parent_id`, and
[`nodeBaseline`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-experiments.ts.md) judges
each node against *its own parent's* value rather than one fixed session baseline, the same "branching, not
linear" reframing The AI Scientist-v2 makes. But the expansion policy is considerably narrower. Where
ParallelAgent expands a **set** of frontier nodes per iteration with an LLM/VLM judge choosing among several
live candidates (plus a separate debug-probability branch), pi-autoresearch-vkf's
[`selectExpansion`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md) was
verified (by reading the source directly) to call only `bestNode` and `selectBalanced` — it never calls the
module's own `frontier` helper. Every pick in a round, whether an "exploit" or "explore" slot, attaches to the
*same* single current-best node; the explore/exploit budget decides which **idea** gets tried next, not which
**node** the search branches from. It buys the headline property — backtrack out of a dead end instead of
grinding forward from the latest possibly-worse result — with a much cheaper, fully deterministic mechanism
(no LLM/VLM judge call per expansion decision), at the cost of never trying two different branches of the tree
in the same round the way ai-scientist-v2's multi-node frontier does. This wiki's own
[karpathy/autoresearch](../code/autoresearch/overview.md) is the ratchet this generalizes from: one global
best-vs-current baseline becomes one best-vs-parent baseline, still without a judge, still without a frontier.

## The production instance: KernelEvolve, and the oracle-vs-judge split

[KernelEvolve](../sources/kernelevolve.md) (Meta, ISCA 2026) is the same pattern run continuously in
business-critical infrastructure, and it cites the same lineage (AIDE, Jiang et al. 2025). Its formalization
is the cleanest in the wiki — a search graph `G_t = (V_t, E_t)` specified by the tuple `(F, π_sel, O, τ)`:
fitness, selection policy, operator, termination rule (source §3.1, p.12). Nodes carry the same
`is_buggy` flag The AI Scientist-v2 uses, and the search likewise runs a **draft phase** of independent
sampling (steps 0–10, no feedback) before a **tree-expansion phase** where each node inherits its ancestors'
profiling, compilation, and correctness feedback (source §4, p.23–24). Reported search depths: 50 steps for
trivial ATen operators, **300 steps** for a production conv1d.

Three differences are load-bearing:

- **The oracle replaces the judge.** AI Scientist-v2 marks a node buggy on an *LLM* verdict over the run plus
  an independent *VLM* verdict over the plots; KernelEvolve marks a node buggy on `torch.allclose` against a
  PyTorch reference and scores it as `F = t_pytorch / t_triton`, with `F = 0` for anything that fails
  correctness or compilation. There is nothing to fool. This is why a 300-step production search can be
  trusted to ship its winner, and it is the same design instinct as Karpathy's
  [autoresearch](../code/autoresearch/overview.md) freezing `val_bpb` — arrived at independently, in a domain
  where a free oracle happens to exist. The tradeoff is the domain restriction: this only works where a
  reference implementation can be differentially tested (see
  [`llm-kernel-generation`](llm-kernel-generation.md)).
- **The selection policy is a swappable parameter, not the architecture.** `π_sel` is documented as
  instantiable three ways — greedy (highest-scoring node), MCTS with UCT, or an evolutionary algorithm
  maintaining a population for crossover/mutation. Where AI Scientist-v2 hard-codes best-first-plus-debug-
  probability and [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/overview.md) hard-codes single-best
  hill-climbing, KernelEvolve treats the whole exploration strategy as configuration. The paper never reports
  which policy produced which result, so its relative-value question stays open.
- **The tree is a database, not a data structure.** Nodes persist to a relational metadata store
  (`id`, `pid`, `score`, `is_buggy`, `path_ref`) backed by an object store; graph views are reconstructed via
  recursive SQL CTEs rather than materialized in memory. That buys three things a per-process tree cannot:
  hundreds of agents concurrently expanding different nodes under transaction isolation, resumption after a
  crash (each node insert *is* a checkpoint), and reuse of trees from **prior sessions** — a new kernel
  request is matched by operator type / shape / platform against history and the search is *initialized* from
  the best prior implementation instead of from the baseline (source §3.2.2, p.15).

> [!inferred] The third point is the one the other tree-search systems in this wiki have no answer to.
> ai-scientist-v2's `Journal` and pi-autoresearch-vkf's tree are both born and die inside one run; a
> "checkpoint" at best resumes the run you were in. KernelEvolve's claim is stronger — that the *right* place
> to start search step 0 is a node from a search that finished last month, on a different but similar
> operator. If inference-time scaling is the axis these systems compete on, warm-starting from a durable
> cross-session corpus is a multiplier none of the single-run designs can match, and it is the same bet this
> wiki makes about accumulating pages instead of re-deriving answers per query.

## An argument against multi-operator search

KernelEvolve also contests a design shared by most systems on this page. It uses a **single universal
operator** rather than the specialized `Draft` / `Debug` / `Improve` operators that tree-search harnesses
typically dispatch between, on the premise (Toledo et al., 2025) that "performance bottlenecks in LLM-based
code generation stem primarily from operator design rather than search algorithms" — a static `Debug` prompt
is error-focused whether the fault is algorithmic or a memory-access pattern. If that is right, then
ai-scientist-v2's debug-probability branch and RD-Agent's Research/Development split are optimizing the wrong
half of the system. The counter-evidence in this wiki cuts the other way, though: Bilevel Autoresearch found
that rewriting the *search mechanism* produced ~5× while parameter tuning produced nothing (see
[`mechanism-level-self-improvement`](mechanism-level-self-improvement.md)). Neither result is a controlled
comparison of the other's claim — noted here as an open disagreement, not a settled one. Full treatment in
[`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md).

**Update from a later paper.** [Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md) (July 2026) cites the same
Toledo et al. premise and reaches the opposite conclusion: it keeps four specialized operators and makes
them **post-training targets**. Its evidence is narrow but direct — the `nomad2018` case study pits a
single-lineage search applying seven successive `Debug` steps against one targeted `Crossover` over two
complementary parents, and the recombination wins by 8–11% RMSE. Crucially, OpenMLE-Evo's operators are
*not* the static templates KernelEvolve objects to: each operator gets a different runtime-constructed
context. So the two systems agree that prompts must be computed per-iteration and disagree only on whether
the move's *name* is a useful index into that computation — a much narrower gap than "operators vs. no
operators." Full treatment in
[`program-evolution-operators`](program-evolution-operators.md).

## Experience-guided expansion: OpenMLE-Evo

[Frontis-MA1](../sources/frontis-ma1.md)'s **OpenMLE-Evo** harness is this wiki's most developed answer to
the question every system on this page has to answer — *which node do I expand next?* — and it is the only
one that measures the answer's cost per useful discovery.

It starts from an **AIRA-Evo-style population loop** (AIDE lineage, same as everything above) and changes
four things, each stated as a delta against the original (§5, p.15):

1. **Deterministic state before prose.** Every evaluated node gets an **experience card** — provenance,
   method family, delta-vs-parent, rank, execution outcome, resource usage — extracted deterministically
   from search state and execution result, never LLM-generated. All cards aggregate into a task-global
   **experience board** (family-wise bests, underexplored directions, repeated failures, score trends,
   parent graph). Compare ai-scientist-v2's `Journal`, whose per-node verdict *is* an LLM/VLM judgment.
2. **Three-factor parent selection.** Not softmax over fitness, but over
   *U = λ_s·quality + λ_Δ·progress + λ_n·novelty* — validation score, normalized positive improvement over
   the strongest parent, and method-family novelty. The `right-whale` study makes the mechanism visible:
   a parent ranked **6th by score** but **1st by gain**, carrying a structurally distinct representation,
   goes from 10.47% to **17.09%** selection probability in the same ten-parent pool (weights 1.0/0.6/0.3);
   it gets picked for `Improve` and its child sets the run's best held-out AUC. The paper's own caution is
   worth keeping: the factors "do not force a lower-scoring branch to win," they keep a distinct branch
   *actionable long enough* to be selected.
3. **Lazy, operator-scoped memory.** AIRA-Evo eagerly LLM-summarizes every evaluated node — paying for
   nodes never selected, and summarizing *before* the decision context that should shape the summary
   exists. OpenMLE-Evo defers synthesis until an `Improve`/`Crossover`/`Debug` call has already chosen its
   nodes, then summarizes only those, and caches.
4. **Bounded, operator-conditioned context** — a vertical ancestor trace plus a horizontal sibling set
   ranked by the same utility, rather than an ever-growing serialized history.

**The measurement is the contribution.** Same checkpoint, same seed, 12 h budget, 66 matched task–runs
(§6.5, Figure 16): total model tokens **−41.7%** and prompt tokens **−50.3%**, while evaluated nodes fall
only **12.4%** — so the saving is in making each expansion cheaper, not in searching less. New-best
validation updates per million tokens rise **1.77 → 3.27 (+84.3%)**, and the share of `Improve` calls that
set a new best roughly doubles (4.73% → 9.36%). The `Improve` prompt's **99th percentile** collapses from
389.0K to 54.3K characters (−86.1%).

> [!inferred] That p99 number is the most transferable result on this page. Every tree search here — the
> `Journal`, the VKF card store, KernelEvolve's node table — accumulates history, and the default move is to
> serialize more of it into each prompt. OpenMLE-Evo is the only system in this wiki that *measured* what
> that costs and showed the frontier is not "more context vs. less" but **structured retrieval vs. bulk
> replay**: it kept the same node throughput while cutting tail context by ~86%. It is also, notably, the
> same diagnosis this wiki's own
> [context-pollution write-up](../sources/2026-06-05-making-karpathy-autoresearch-production-ready.md)
> reached from operating a loop, and that
> [`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md) reaches from the
> kernel side — three independent arrivals at the same architecture.

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **agentic-tree-search** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md) — AgentManager — the four-stage experiment orchestrator
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md) — Journal & Node — the experiment tree's data model
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) — ParallelAgent — the agentic tree-search engine
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-experiments.ts.md) — Experiment log & parent-relative baselines — what makes the tree-search meaningful
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md) — The tool spine — autoresearchExtension and the autoresearch loop's control surface
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md) — The experiment search tree — best-first expansion over a parent-relative frontier
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md) — Tree-search state — the append-only event log and resumable snapshot behind SFT collection
<!-- connect:auto:end -->
