---
title: 'Module: rdagent/components/coder/model_coder/eva_utils.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/eva_utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.eva_utils`/
symbols:
  ModelCodeEvaluator.evaluate: ModelCodeEvaluator#evaluate().
  ModelFinalEvaluator.evaluate: ModelFinalEvaluator#evaluate().
  ModelCodeEvaluator: ModelCodeEvaluator#
  ModelFinalEvaluator: ModelFinalEvaluator#
  shape_evaluator: shape_evaluator().
  value_evaluator: value_evaluator().
---
# Module: [`rdagent/components/coder/model_coder/eva_utils.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py)

## Classes
### `ModelCodeEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/model_coder/eva_utils.py:52`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L52)
- signature: `class ModelCodeEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: Workspace, gt_implementation: Workspace, model_execution_feedback: str = "", model_value_feedback: str = "")` — [`L53`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L53)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`Workspace`](../../../core/experiment.md#Workspace), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`ModelTask`](model.md#ModelTask), [`ModelFBWorkspace`](model.md#ModelFBWorkspace), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`get_task_information`](model.md#ModelTask.get_task_information), [`all_codes`](../../../core/experiment.md#FBWorkspace.all_codes), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`model_type`](model.md#ModelTask.model_type)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`evaluate`](evaluators.md#ModelCoSTEEREvaluator.evaluate)

### `ModelFinalEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/model_coder/eva_utils.py:105`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L105)
- signature: `class ModelFinalEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: Workspace, gt_implementation: Workspace, model_execution_feedback: str, model_shape_feedback: str, model_value_feedback: str, model_code_feedback: str)` — [`L106`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L106)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`Workspace`](../../../core/experiment.md#Workspace), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`ModelTask`](model.md#ModelTask), [`ModelFBWorkspace`](model.md#ModelFBWorkspace), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`get_task_information`](model.md#ModelTask.get_task_information), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`model_type`](model.md#ModelTask.model_type)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`evaluate`](evaluators.md#ModelCoSTEEREvaluator.evaluate)

## Functions
- `shape_evaluator(prediction: np.ndarray, target_shape: Tuple = None)` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L15)
- `value_evaluator(prediction: np.ndarray, target: np.ndarray)` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/eva_utils.py#L32)

