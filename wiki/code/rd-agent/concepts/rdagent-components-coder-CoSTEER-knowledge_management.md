---
title: Co-STEER Knowledge Management — RAG memory over task/code/feedback triples
type: concept
provenance: mixed
concept: rdagent-components-coder-CoSTEER-knowledge_management
concepts: [research-development-loop, closed-loop-experiment-design]
updated: 2026-07-04
status: fresh
---

# Co-STEER Knowledge Management — RAG memory over task/code/feedback triples

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [closed-loop-experiment-design](../../../concepts/closed-loop-experiment-design.md), [research-development-loop](../../../concepts/research-development-loop.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview

This is Co-STEER's own persistent memory — the concrete mechanism behind
[the RD-Agent paper](../../../sources/rd-agent.md)'s claim that Co-STEER "retrieves similar past
task/code/feedback triples from a persistently growing knowledge base to seed new code generation."
`CoSTEERKnowledgeBaseV2` stores every task/code/feedback triple Co-STEER has ever produced as nodes in a
shared knowledge graph (the generic structure documented in
[the knowledge_management/graph concept page](rdagent-components-knowledge_management-graph.md)), and
`CoSTEERRAGStrategyV2` is the retrieval-augmented-generation strategy wrapped around it: every evolving
iteration it does two things — turn fresh evaluation feedback into graph nodes (the write path,
`generate_knowledge`), and retrieve three independent flavors of relevant memory for the next generation
attempt (the read path, `query`). The three flavors are not redundant: they answer "what did *this task*
already try," "who solved a task touching the same *component*," and "who has hit this exact *error*
before" — three different similarity axes over the same graph.

## Diagram

```mermaid
sequenceDiagram
    participant Trace as evolving_trace (EvoStep list)
    participant RAG as CoSTEERRAGStrategyV2
    participant KB as CoSTEERKnowledgeBaseV2

    Trace->>RAG: generate_knowledge(evolving_trace)
    RAG->>KB: analyze_component() / update_success_task() (write path)
    Note over RAG,KB: success -> graph node; failure -> error analysis

    RAG->>RAG: query(evo, evolving_trace)
    RAG->>RAG: former_trace_query() — this task's own history
    RAG->>RAG: component_query() — sibling tasks, same component
    RAG->>RAG: error_query() — prior fixes for this exact error
    RAG-->>Trace: CoSTEERQueriedKnowledge fed into next implement_one_task()
```

## Design rationale (why it's built this way)

Retrieval is split into three specialist passes inside
[`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query)
rather than one similarity search because each answers a different question:
[`former_trace_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query)
captures "what has *this exact task* already tried and failed" (a local, recency-biased signal);
[`component_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query)
captures "who else solved a task that touches the same component" (cross-task generalization via an
LLM-assigned component tag); [`error_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query)
captures "who else hit *this specific error* and fixed it" (the sharpest, most targeted signal, since it
conditions on the literal failure rather than task similarity). Feeding all three into one generation
prompt lets it see both broad successful patterns and a pointed fix for the exact failure just observed.

`CoSTEERQueriedKnowledgeV2` is threaded through all three query passes as one mutable, accumulating object
rather than three independent return values — later passes can see what earlier passes already decided
(both `component_query` and `error_query` check `failed_task_info_set`, which `former_trace_query`
populates, before doing any work).

> [!inferred] `component_query`'s retrieved list is rebalanced so that knowledge validated against a ground
> truth implementation is never entirely crowded out by knowledge that wasn't. Reading the source, this
> looks like a defense against feeding the generation prompt examples whose "success" was only ever
> self-reported by a prior LLM generation and never checked against a real ground truth — but no docstring
> states this explicitly.

## Entry points

- [`generate_knowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge) —
  the write path; called once per evolving-loop iteration to fold newly evaluated feedback into the
  knowledge graph.
- [`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query) —
  the read path; its output, a
  [`CoSTEERQueriedKnowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge),
  is threaded into every domain's `implement_one_task`, e.g. `FactorMultiProcessEvolvingStrategy`'s
  [`implement_one_task`](../catalog/rdagent/components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task),
  as the retrieved context a code-generation prompt is built from.

## Mechanism (step-by-step)

1. **Incremental write.** [`generate_knowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge)
   walks only the [`EvoStep`](../catalog/rdagent/core/evolving_framework.md#EvoStep)s appended since the
   last call (it tracks how many it has already processed, so it never replays old steps). For each
   sub-task with feedback available, it checks
   [`final_decision`](../catalog/rdagent/components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision):
   on success the triple is stored in a working-trace dict and promoted into the graph; on failure it runs
   error analysis over
   [`return_checking`](../catalog/rdagent/components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking)
   or [`execution`](../catalog/rdagent/components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution)
   text, whichever is available.

2. **Folding a success into the graph.**
   [`update_success_task`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.update_success_task)
   is the only place this page's memory touches the shared
   [`graph`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph)
   instance: it creates one `task_description` node per solved task, links it to that task's pre-computed
   component nodes via
   [`add_node`](../catalog/rdagent/components/knowledge_management/graph.md#UndirectedGraph.add_node), then
   walks the task's whole attempt history, turning every intermediate attempt into a `task_trace` node
   ([`UndirectedNode`](../catalog/rdagent/components/knowledge_management/graph.md#UndirectedNode)) linked
   to any error nodes it produced, and the final attempt into a `task_success_implement` node.

3. **Tagging a task with components is an LLM call, cached per task.**
   [`analyze_component`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_component)
   sends every existing "component" node's content plus the target task's description to an LLM via
   [`APIBackend`](../catalog/rdagent/oai/llm_utils.md#APIBackend) /
   [`build_messages_and_create_chat_completion`](../catalog/rdagent/oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion)
   (rendered through the [`T`](../catalog/rdagent/utils/agent/tpl.md#T) /
   [`r`](../catalog/rdagent/utils/agent/tpl.md#RDAT.r) template helpers), asking which component indices the
   task belongs to; the result is cached in `task_to_component_nodes` so the LLM is called once per unique
   task, never once per query.

4. **Read path fan-out.** [`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query)
   is the single method the evolving strategy calls each iteration; it runs
   [`former_trace_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query),
   [`component_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query),
   and [`error_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query)
   in that fixed order over one accumulating
   [`CoSTEERQueriedKnowledgeV2`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2).

5. **Local history first.** [`former_trace_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query)
   caps a task's own working trace to a configurable recency window, first pruning "regression" steps — a
   later attempt that lost `return_checking` an earlier attempt had — read as "this rewrite made things
   worse, don't show it as an exemplar" — and separately marks a task permanently into
   `failed_task_info_set` once its trial count crosses a configured limit, so later passes stop feeding it
   any memory at all.

6. **Cross-task retrieval by shared component.**
   [`component_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query)
   looks up a task's cached component tags, walks the graph outward from each component node to find
   sibling task-description nodes and, further out, any node already marked as a successful implementation
   for those tasks — capping how many results come from any single component so the list isn't dominated
   by whichever component has the most graph traffic. It then separately folds in plain embedding
   similarity between the new task's description and every already-solved task's description, and finally
   rebalances the combined list to guarantee ground-truth-validated knowledge survives the cutoff (see
   Design rationale).

7. **Targeted retrieval by matching error.** [`error_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query)
   takes the error nodes recorded against the task's most recent queried failed trace and looks for other
   historical traces that hit the *same* error node(s) and eventually succeeded, returning each match as an
   `(error description, (failing trace, successful fix))` pair — the sharpest signal `query` produces, since
   it conditions on the literal failure mode instead of task-level similarity.

## Key data structures

- `CoSTEERKnowledgeBaseV2` —
  holds `working_trace_knowledge` (every attempt, keyed by task info string), `working_trace_error_analysis`
  (error nodes/strings aligned per attempt), `success_task_to_knowledge_dict` (one canonical success per
  task), `node_to_implementation_knowledge_dict` (graph node id → the knowledge triple it represents),
  `task_to_component_nodes` (cached LLM tagging), and one shared
  [`graph`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph)
  ([`UndirectedGraph`](../catalog/rdagent/components/knowledge_management/graph.md#UndirectedGraph)).
- [`CoSTEERQueriedKnowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge) /
  [`CoSTEERQueriedKnowledgeV2`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2) —
  the per-query result object: `success_task_to_knowledge_dict`, `failed_task_info_set`,
  `task_to_former_failed_traces`, `task_to_similar_task_successful_knowledge`, and (V2 only)
  `task_to_similar_error_successful_knowledge`.

## Dynamics (design intent)

`generate_knowledge` is safe to call every iteration because it's incremental by construction: it compares
`len(evolving_trace)` against a stored count and only processes the delta, so repeated calls within the
same iteration are cheap no-ops. `query`'s three passes run in a fixed sequence and communicate purely
through the shared `queried_knowledge_v2` object — `component_query` and `error_query` both re-check
`failed_task_info_set` before doing any retrieval work, so a task `former_trace_query` already gave up on
never reaches the more expensive graph-walk and LLM-adjacent logic in the later passes.

## Edge cases

- Once a task crosses `fail_task_trial_limit` trials, it is permanently excluded from every retrieval pass
  in this query — `component_query` and `error_query` both short-circuit to an empty result the moment they
  see it in `failed_task_info_set`. Nothing in this packet's subgraph stops a caller from still invoking
  `implement_one_task` for that task with no retrieved knowledge at all; the knowledge base simply gives up
  on assisting it.
- `former_trace_query`'s regression-pruning loop assumes the working trace is already in chronological
  order — it only deletes entries that look like a regression, it never reorders.

## Open questions

- The path by which a `CoSTEERKnowledgeBaseV2`
  gets reloaded from disk across separate RD-Agent runs (making the knowledge base "persistently growing"
  across processes, as the paper describes) is not exercised by any symbol in this packet's subgraph.
- Whether `component_query`'s dual retrieval (graph connectivity + raw embedding similarity) was chosen
  because one alone under-retrieves, or as a deliberate precision/recall tradeoff, isn't stated anywhere in
  source — see the `> [!inferred]` note above.

## See also

- [Co-STEER evaluators](rdagent-components-coder-CoSTEER-evaluators.md) — the upstream feedback this page's
  write path consumes.
- [Knowledge-management graph](rdagent-components-knowledge_management-graph.md) — the shared graph
  primitives this knowledge base is built from.
- [Factor coder](rdagent-components-coder-factor_coder-factor.md) — `FactorTask.get_task_information()`'s
  output string is the exact key this page's retrieval dicts are keyed on.
- [RD-Agent paper summary](../../../sources/rd-agent.md) — Co-STEER's retrieval-based knowledge base as the
  Development phase's memory component.
- [`research-development-loop`](../../../concepts/research-development-loop.md),
  [`closed-loop-experiment-design`](../../../concepts/closed-loop-experiment-design.md) — cross-repo
  concept pages this page connects to.
