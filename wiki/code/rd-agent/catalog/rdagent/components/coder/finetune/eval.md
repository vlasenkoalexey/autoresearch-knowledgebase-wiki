---
title: 'Module: rdagent/components/coder/finetune/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/finetune/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.finetune.eval`/
symbols:
  FTCoderEvaluator.evaluate: FTCoderEvaluator#evaluate().
  FTDataEvaluator.evaluate: FTDataEvaluator#evaluate().
  FTDataEvaluator._generate_llm_feedback: FTDataEvaluator#_generate_llm_feedback().
  FTDataEvaluator._update_dataset_info: FTDataEvaluator#_update_dataset_info().
  FTDataEvaluator: FTDataEvaluator#
  FTCoderEvaluator: FTCoderEvaluator#
  FTCoderEvaluator.__init__: FTCoderEvaluator#__init__().
  FTDataEvaluator._validate_data_json: FTDataEvaluator#_validate_data_json().
  FTDataEvaluator._sample_data: FTDataEvaluator#_sample_data().
  FTDataEvaluator._analyze_data_quality: FTDataEvaluator#_analyze_data_quality().
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/finetune/eval.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py)

## Classes
### `FTCoderEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/finetune/eval.py:307`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L307)
- doc: Evaluator for LLM fine-tuning implementations with simplified validation
- signature: `class FTCoderEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L313`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L313) — Evaluate LLM fine-tuning implementation with two-step validation
- protocol/private: `__init__`[`L310`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L310)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`get_ft_env`](conf.md#get_ft_env), [`final_decision`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`build_cls_from_json_with_retry`](../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`return_checking`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`FT_YAML_FILE_NAME`](conf.md#FT_YAML_FILE_NAME), [`code`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`validate_and_test`](unified_validator.md#LLMConfigValidator.validate_and_test), [`val_and_update_init_dict`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`source_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.source_feedback), [`__init__`](../CoSTEER/evaluators.md#CoSTEEREvaluator.__init__), [`success`](unified_validator.md#ValidationResult.success), [`LLMConfigValidator`](unified_validator.md#LLMConfigValidator), [`SYSTEM_MANAGED_PARAMS`](unified_validator.md#SYSTEM_MANAGED_PARAMS), [`execution_output`](unified_validator.md#ValidationResult.execution_output), [`filtered_config`](unified_validator.md#ValidationResult.filtered_config), [`raw_execution`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.raw_execution), [`raw_stdout`](unified_validator.md#ValidationResult.raw_stdout)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#LLMFinetuneCoSTEER.__init__)

### `FTDataEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/finetune/eval.py:42`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L42)
- doc: Evaluator for data processing results.
- signature: `class FTDataEvaluator(CoSTEEREvaluator):`
- members:
  - `_analyze_data_quality(self, data: list)` — [`L277`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L277) — Analyze data quality statistics for all fields.
  - `_generate_llm_feedback(self, target_task: Task, script_code: str, stdout: str, exit_code: int, data: Optional[list], error_msg: Optional[str], queried_knowledge: Optional[QueriedKnowledge], raw_stdout: str = "")` — [`L134`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L134) — Generate LLM-based feedback for data processing evaluation.
  - `_sample_data(self, data: list, n: int = 5)` — [`L271`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L271) — Random sampling for LLM evaluation.
  - `_update_dataset_info(self, implementation: FBWorkspace, sample_count: int)` — [`L246`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L246) — Generate dataset_info.json for LlamaFactory to use the processed data.
  - `_validate_data_json(self, data_json_path: Path)` — [`L207`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L207) — Validate data.json file format and content.
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: Optional[QueriedKnowledge] = None, **kwargs)` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L51) — Evaluate data processing implementation with LLM feedback.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`run`](../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`return_checking`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`clear_workspace`](conf.md#clear_workspace), [`code`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`get_workspace_prefix`](conf.md#get_workspace_prefix), [`get_data_processing_env`](conf.md#get_data_processing_env), [`inject_data_stats`](conf.md#inject_data_stats), [`FT_DATA_SCRIPT_NAME`](conf.md#FT_DATA_SCRIPT_NAME), [`val_and_update_init_dict`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`source_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.source_feedback), [`FT_DATA_FILE_NAME`](conf.md#FT_DATA_FILE_NAME), [`get_data_processing_cache_key`](conf.md#get_data_processing_cache_key), [`force_think_token`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.force_think_token), [`upper_data_size_limit`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.upper_data_size_limit), [`raw_execution`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.raw_execution)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#LLMFinetuneCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/eval.py#L39)

