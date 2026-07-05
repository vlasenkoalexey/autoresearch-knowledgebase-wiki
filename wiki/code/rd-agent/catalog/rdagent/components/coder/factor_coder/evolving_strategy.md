---
title: 'Module: rdagent/components/coder/factor_coder/evolving_strategy.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/evolving_strategy.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder.evolving_strategy`/FactorMultiProcessEvolvingStrategy#
symbols:
  FactorMultiProcessEvolvingStrategy.implement_one_task: implement_one_task().
  FactorMultiProcessEvolvingStrategy.error_summary: error_summary().
  FactorMultiProcessEvolvingStrategy: ''
  FactorMultiProcessEvolvingStrategy.__init__: __init__().
  FactorMultiProcessEvolvingStrategy.assign_code_list_to_evo: assign_code_list_to_evo().
  FactorMultiProcessEvolvingStrategy.num_loop: num_loop.
  FactorMultiProcessEvolvingStrategy.haveSelected: haveSelected.
---
# Module: [`rdagent/components/coder/factor_coder/evolving_strategy.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py)

## Classes
### `FactorMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/factor_coder/evolving_strategy.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L23)
- signature: `class FactorMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list, evo)` — [`L166`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L166)
  - `error_summary(self, target_task: FactorTask, queried_former_failed_knowledge_to_render: list, queried_similar_error_knowledge_to_render: list)` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L29)
  - `implement_one_task(self, target_task: FactorTask, queried_knowledge: CoSTEERQueriedKnowledge, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L60) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `haveSelected` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L27)
  - `num_loop` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L26)
- protocol/private: `__init__`[`L24`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evolving_strategy.py#L24)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`FactorTask`](factor.md#FactorTask), [`CoSTEERQueriedKnowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`FactorFBWorkspace`](factor.md#FactorFBWorkspace), [`FACTOR_COSTEER_SETTINGS`](config.md#FACTOR_COSTEER_SETTINGS), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`scen`](../../../core/evolving_framework.md#EvolvingStrategy.scen), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`get_task_information`](factor.md#FactorTask.get_task_information), [`CoSTEERQueriedKnowledgeV2`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`__init__`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.__init__), [`task_to_similar_error_successful_knowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2.task_to_similar_error_successful_knowledge), [`task_to_former_failed_traces`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV1.task_to_former_failed_traces), [`coder_use_cache`](../CoSTEER/config.md#CoSTEERSettings.coder_use_cache), [`v2_error_summary`](../CoSTEER/config.md#CoSTEERSettings.v2_error_summary)
- used by: [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#FactorCoSTEER.__init__)

