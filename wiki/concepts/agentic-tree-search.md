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

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **agentic-tree-search** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md) — AgentManager — the four-stage experiment orchestrator
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md) — Journal & Node — the experiment tree's data model
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) — ParallelAgent — the agentic tree-search engine
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-experiments.ts.md) — Experiment log & parent-relative baselines — what makes the tree-search meaningful
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md) — The tool spine — autoresearchExtension and the autoresearch loop's control surface
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md) — The experiment search tree — best-first expansion over a parent-relative frontier
<!-- connect:auto:end -->
