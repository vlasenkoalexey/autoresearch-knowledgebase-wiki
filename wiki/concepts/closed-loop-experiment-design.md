# Closed-loop experiment design

A **closed-loop experiment design** is a research-automation pattern where each completed experiment's
outcome is fed back into the *next* hypothesis or resource-allocation decision, rather than experiments
running independently off a fixed, pre-planned list. The loop closes over four steps: **hypothesize →
implement → validate/evaluate → feed back**, and what a given system does at the "feed back" step — what
state it updates, and what decision that state changes next — is the interesting design variable across
systems in this wiki.

## Instances in RD-Agent

[RD-Agent](../sources/rd-agent.md) (Microsoft Research) instantiates this loop twice, at two levels of
granularity:

- **General framework** (rd-agent.pdf): each R&D-loop iteration appends `(parents, idea, code, score)` to a
  growing exploration graph `G` (Algorithm 1, p.6). The **FC-Memory Context** component reads this graph back
  into the next iteration's **FC-Reasoning Pipeline**, and a **collaborative memory** mechanism — a
  probabilistic interaction kernel (Eq. 1, p.19) — additionally lets parallel exploration branches share their
  best/similar hypotheses without collapsing diversity across branches.
- **RD-Agent(Q)** (rd-agent-quant.pdf): the **Analysis Unit** closes the loop explicitly — it scores each
  round against the current SOTA factor/model configuration, feeds structured feedback back to the
  **Synthesis Unit**, and additionally decides *which axis* (factor or model) the next iteration should
  optimize, formulated as a **contextual two-armed bandit** solved via linear Thompson sampling over an
  8-dimensional performance-state vector (IC, ICIR, rank-IC, rank-ICIR, ARR, IR, −MDD, SR) (rd-agent-quant.pdf,
  §2.5 and Appendix A.2, pp.5,16). Ablating this scheduler against an LLM-based scheduler and random
  scheduling shows the bandit wins on IC, ARR, and number of SOTA selections found under a fixed 12-hour
  compute budget (Table 3, rd-agent-quant.pdf p.9).

> [!inferred] The two instances differ in *what* closes the loop: the general framework's feedback is
> unstructured (a graph of past attempts, retrieved by similarity), while RD-Agent(Q)'s feedback is a
> structured, low-dimensional state vector driving an explicit bandit policy. This suggests closed-loop
> designs sit on a spectrum from "retrieve-similar-past-attempts" to "formal sequential-decision-policy over
> summary statistics," and RD-Agent(Q)'s domain (quant finance, where IC/ARR/etc. are already the field's
> standard sufficient statistics) is what makes the more formal bandit treatment tractable.

## How the implementations differ (across this wiki's repos)
The two ingested code silos close the loop at different granularities, and the contrast is the useful thing
to hold. **[ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md)**
closes it *inside a single tree search*: each `Node` is a full experiment attempt, and "feed back" means
folding an LLM+VLM verdict on the node's results/plots back into the tree's ranking so the next `step()` picks
a better parent to expand — the feedback state is the tree itself.
**[rd-agent](../code/rd-agent/concepts/rdagent-utils-workflow-loop.md)** instead closes it *across an explicit
Research→Development boundary*: its [`LoopBase`](../code/rd-agent/concepts/rdagent-utils-workflow-loop.md)
engine appends each scored `(hypothesis, code, feedback)` to a
[`Trace`](../code/rd-agent/concepts/rdagent-core-proposal.md), and a fresh Research step reads that history
(and, in RD-Agent(Q), a bandit over summary statistics) to decide the *next* proposal — the feedback state is
a structured trace of past attempts, deliberately separated from the code-generation step that Co-STEER runs.
The axis: ai-scientist-v2's feedback is *retrieve-similar-node-in-one-search*, RD-Agent's is
*decide-next-proposal-from-a-recorded-history* — the same spectrum flagged in the RD-Agent inference block
above, now visible as two real codebases.
**[pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-cards.ts.md)**
adds a third point on that axis: its feedback state is neither a live search tree nor a Trace of scored
attempts, but a durable, trust-gated **VKF card store** written back independently of any single session —
[`buildExperimentCard`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
stages a result as a `locally_tested` card (win *or* loss — losses are kept, not discarded) with structured
`next_suggestions`, and belief compounds via a Beta posterior over accumulated evidence rather than being
overwritten each round. Where RD-Agent's Trace and ai-scientist-v2's tree are scoped to one run,
pi-autoresearch-vkf's card store is scoped to the *project* (and, via `promote_to_global`, across projects) —
closer to "retrieve-verified-claims-from-a-persistent-memory" than either of the other two.

## See also
- [`research-development-loop`](research-development-loop.md) — the two-phase (Research/Development)
  structure that this feedback loop closes across.
- [`../topics/autoresearch.md`](../topics/autoresearch.md) — other closed-loop systems in this wiki and how
  their feedback mechanisms compare.

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **closed-loop-experiment-design** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [rd-agent](../code/rd-agent/concepts/rdagent-components-coder-CoSTEER-evaluators.md) — Co-STEER Evaluators — grading generated code down to one bool
- [rd-agent](../code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md) — Co-STEER Knowledge Management — RAG memory over task/code/feedback triples
- [rd-agent](../code/rd-agent/concepts/rdagent-components-knowledge_management-graph.md) — UndirectedGraph — the shared semantic + connectivity memory substrate
- [rd-agent](../code/rd-agent/concepts/rdagent-core-evolving_framework.md) — The evolving framework — Co-STEER's propose/evaluate/refine engine
- [rd-agent](../code/rd-agent/concepts/rdagent-core-experiment.md) — Experiment, Workspace, and Task — the R&D loop's shared currency
- [rd-agent](../code/rd-agent/concepts/rdagent-core-proposal.md) — Hypothesis, Trace, and ExpGen — the Research phase's proposal machinery
- [rd-agent](../code/rd-agent/concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) — DSTrace — the data-science exploration DAG and its ExpGen proposers
- [rd-agent](../code/rd-agent/concepts/rdagent-utils-workflow-loop.md) — LoopBase — the generic async engine behind Algorithm 1's R&D loop
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-cards.ts.md) — VKF cards — the trust-lifecycle memory model
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md) — The tool spine — autoresearchExtension and the autoresearch loop's control surface
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-scoring.ts.md) — Idea scoring & explore/exploit balancing (`scoring.ts`)
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md) — The experiment search tree — best-first expansion over a parent-relative frontier
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md) — AgentManager — the four-stage experiment orchestrator
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md) — Journal & Node — the experiment tree's data model
- [ai-scientist-v2](../code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) — ParallelAgent — the agentic tree-search engine
<!-- connect:auto:end -->
