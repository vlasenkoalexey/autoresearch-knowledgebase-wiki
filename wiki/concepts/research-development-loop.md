# Research–Development loop

A **Research–Development (R&D) loop** decomposes an autoresearch/auto-optimization system into two
explicitly separated phases: a **Research** phase that proposes and refines *what to try next* before
spending compute on it, and a **Development** phase that turns the chosen idea into working, evaluated code.
The split is the architectural bet: cheap idea-generation and filtering happen before expensive
implementation and execution, rather than interleaving them ad hoc.

## Canonical instance: RD-Agent (Microsoft Research)

[RD-Agent](../sources/rd-agent.md) is the wiki's reference implementation of this pattern, formalized as
**six fixed components** across the two phases (rd-agent.pdf, pp.4–6):

**Research** — discover and refine promising ideas before costly implementation:
1. **FC-Planning** — dynamically allocates exploration effort over time (explore early, exploit late).
2. **FC-Exploration Path Structuring** — how candidate solutions are organized (chain vs. tree vs.
   RD-Agent's adaptive DAG that maximizes first-layer diversity, then greedily exploits the best branch).
3. **FC-Reasoning Pipeline** — turns memory context into concrete ideas: dataset analysis → hypothesis
   formulation → trade-off assessment.
4. **FC-Memory Context** — stores/retrieves historical solutions and insights across iterations.

**Development** — turn the chosen idea into a bug-free, evaluated solution:
5. **FC-Coding Workflow** — idea → runnable code, with early bug detection via rapid prototyping on
   sampled data before full-scale runs.
6. **FC-Evaluation Strategy** — reliable, consistent scoring (stable metrics, fixed validation splits,
   aggregated evaluation to filter noise/overfitting).

The high-level algorithm (Algorithm 1, rd-agent.pdf p.6): while time remains, run
**Planning → SelectParents → Memory Context → Reasoning Pipeline** (Research), then **Dev → Eval**
(Development), appending `(parents, idea, code, score)` to a growing exploration graph `G`. RD-Agent's own
ablations (Table 3, rd-agent.pdf p.8) rank component importance: exploration-path structuring matters most
(removing it costs 28% relative Any-Medal Rate on MLE-Bench), then reasoning pipeline and planning (~24%
each), then memory context (~9%); on the Development side, removing the efficient debug workflow hurts
immediately and persistently (34.7% → 24.0%), while removing aggregated evaluation only hurts after solutions
get complex enough to overfit (~2h in).

## Domain specialization: RD-Agent(Q)

[RD-Agent(Q)](../sources/rd-agent.md) re-instantiates the same two-phase split for quantitative finance with
five domain-specific units instead of the six generic ones (rd-agent-quant.pdf, Fig. 3, p.3): **Specification**
(top of Research, encodes the task tuple `S = (B, D, F, M)`), **Synthesis** (Research, generates the next
hypothesis from a "knowledge forest," conditioned on which axis — factor or model — is being optimized),
**Implementation** (Development, runs **Co-STEER**, a dedicated code-generation agent with a complexity-aware
DAG scheduler and retrieval over past task/code/feedback triples), **Validation** (Development, de-duplicates
new factors by pairwise IC correlation, backtests survivors via Qlib), and **Analysis** (bridges phases,
scores the round and decides the next iteration's optimization axis).

> [!inferred] The mapping between the two instantiations isn't 1:1 — RD-Agent(Q)'s Analysis Unit (a
> contextual two-armed bandit over IC/ICIR/ARR/IR/etc.) is best read as a concrete, domain-specialized
> instance of the general framework's **FC-Planning** component (deciding *where* to spend the next
> iteration's budget), just specialized to a two-armed factor-vs-model action space rather than a
> continuous explore/exploit schedule.

## A lighter-weight instance: pi-autoresearch-vkf

[pi-autoresearch-vkf](../code/pi-autoresearch-vkf/overview.md)'s own CHANGELOG cites RD-Agent's
"structured Research→Development cycle" as a direct influence, but the code realizes the split far more
minimally than RD-Agent's six fixed components. There is no dedicated exploration-path-structuring unit, no
Co-STEER-style evaluator ensemble, and no domain-specific bandit scheduler — the entire split collapses into
one branching decision in [`ResearchConfig`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-config.ts.md):
whether `init_research` was given a measurable metric. `optimize` sessions run the Development-flavored,
metric-driven experiment loop; `ideate` sessions stop at a Research-flavored ranked plan with no execution
step at all. The tool spine in
[`autoresearchExtension`](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md)
still separates pre-test tools (`remember_claim`/`find_contradictions`/`find_transfers`/`find_compositions`/
`draft_research_plan`) from post-test ones (`plan_next_step`/`vkf_run_experiment`/`vkf_log_experiment`), but
there is no equivalent of RD-Agent's FC-Memory-Context-as-a-DAG or its sandboxed `Env` — memory is a flat VKF
card store, and "development" is just running the user's own measure command. Where RD-Agent formalizes R→D
as the object of study, pi-autoresearch-vkf treats it as one config-time fork inside a smaller, VKF-memory-
centric loop — the same lineage, a much thinner instantiation.

## See also
- [`closed-loop-experiment-design`](closed-loop-experiment-design.md) — the feedback mechanism that
  connects a completed Development-phase result back into the next Research-phase proposal.
- [`../topics/autoresearch.md`](../topics/autoresearch.md) — where this pattern sits relative to academic
  AI-scientist systems targeting novel discovery rather than repeatable MLE/quant labor.
- [`agentic-tree-search`](agentic-tree-search.md) — pi-autoresearch-vkf's other stated influence (AIDE / The
  AI Scientist v2), wired into the same tool spine as this concept.

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **research-development-loop** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [rd-agent](../code/rd-agent/concepts/rdagent-components-coder-CoSTEER-evaluators.md) — Co-STEER Evaluators — grading generated code down to one bool
- [rd-agent](../code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md) — Co-STEER Knowledge Management — RAG memory over task/code/feedback triples
- [rd-agent](../code/rd-agent/concepts/rdagent-components-coder-factor_coder-factor.md) — Factor coder — turning a factor hypothesis into an executed value
- [rd-agent](../code/rd-agent/concepts/rdagent-components-knowledge_management-graph.md) — UndirectedGraph — the shared semantic + connectivity memory substrate
- [rd-agent](../code/rd-agent/concepts/rdagent-core-evolving_framework.md) — The evolving framework — Co-STEER's propose/evaluate/refine engine
- [rd-agent](../code/rd-agent/concepts/rdagent-core-experiment.md) — Experiment, Workspace, and Task — the R&D loop's shared currency
- [rd-agent](../code/rd-agent/concepts/rdagent-core-proposal.md) — Hypothesis, Trace, and ExpGen — the Research phase's proposal machinery
- [rd-agent](../code/rd-agent/concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) — DSTrace — the data-science exploration DAG and its ExpGen proposers
- [rd-agent](../code/rd-agent/concepts/rdagent-utils-env.md) — Env — the sandboxed execution substrate for the Development phase
- [rd-agent](../code/rd-agent/concepts/rdagent-utils-workflow-loop.md) — LoopBase — the generic async engine behind Algorithm 1's R&D loop
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-config.ts.md) — Session config (`ResearchConfig`) — the optimize/ideate switch and explore/exploit defaults
- [pi-autoresearch-vkf](../code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md) — The tool spine — autoresearchExtension and the autoresearch loop's control surface
<!-- connect:auto:end -->
