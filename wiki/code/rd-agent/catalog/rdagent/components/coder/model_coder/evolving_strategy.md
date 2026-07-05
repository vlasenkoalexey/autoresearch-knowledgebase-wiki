---
title: 'Module: rdagent/components/coder/model_coder/evolving_strategy.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/evolving_strategy.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.evolving_strategy`/ModelMultiProcessEvolvingStrategy#
symbols:
  ModelMultiProcessEvolvingStrategy.implement_one_task: implement_one_task().
  ModelMultiProcessEvolvingStrategy: ''
  ModelMultiProcessEvolvingStrategy.assign_code_list_to_evo: assign_code_list_to_evo().
---
# Module: [`rdagent/components/coder/model_coder/evolving_strategy.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evolving_strategy.py)

## Classes
### `ModelMultiProcessEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/components/coder/model_coder/evolving_strategy.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evolving_strategy.py#L20)
- signature: `class ModelMultiProcessEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `assign_code_list_to_evo(self, code_list, evo)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evolving_strategy.py#L82)
  - `implement_one_task(self, target_task: ModelTask, queried_knowledge: CoSTEERQueriedKnowledge = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evolving_strategy.py#L21)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`ModelTask`](model.md#ModelTask), [`CoSTEERQueriedKnowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`ModelFBWorkspace`](model.md#ModelFBWorkspace), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`get_task_information`](model.md#ModelTask.get_task_information), [`scen`](../../../core/evolving_framework.md#EvolvingStrategy.scen), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`CoSTEERQueriedKnowledgeV2`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`CoSTEER_SETTINGS`](../CoSTEER/config.md#CoSTEER_SETTINGS), [`coder_use_cache`](../CoSTEER/config.md#CoSTEERSettings.coder_use_cache)
- used by: [`MultiProcessEvolvingStrategy`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`assign_code_list_to_evo`](../CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`__init__`](__init__.md#ModelCoSTEER.__init__)

