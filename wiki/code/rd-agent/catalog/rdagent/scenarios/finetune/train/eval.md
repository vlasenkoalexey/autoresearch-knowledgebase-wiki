---
title: 'Module: rdagent/scenarios/finetune/train/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/train/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.train.eval`/
symbols:
  FTRunnerEvaluator.evaluate: FTRunnerEvaluator#evaluate().
  FTRunnerEvaluator._generate_llm_feedback: FTRunnerEvaluator#_generate_llm_feedback().
  FTRunnerEvaluator._run_full_data_processing: FTRunnerEvaluator#_run_full_data_processing().
  extract_loss_history: extract_loss_history().
  FTRunnerEvaluator: FTRunnerEvaluator#
---
# Module: [`rdagent/scenarios/finetune/train/eval.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py)

## Classes
### `FTRunnerEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/scenarios/finetune/train/eval.py:78`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py#L78)
- doc: LLM Fine-tuning specific evaluator that uses LLM Docker environment.
- signature: `class FTRunnerEvaluator(CoSTEEREvaluator):`
- members:
  - `_generate_llm_feedback(self, target_task: FTTask, implementation: FBWorkspace, raw_stdout: str, exit_code: int, model_files_exist: bool, benchmark_result: Optional[Dict] = None, loss_history: Optional[Dict[str, List[Dict]]] = None, failed_stage: Optional[str] = None)` — [`L239`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py#L239) — Generate LLM-based feedback for runner evaluation. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `_run_full_data_processing(self, implementation: FBWorkspace)` — [`L303`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py#L303) — Execute full data processing (without --debug flag) to generate complete data.json.
  - `evaluate(self, target_task: FTTask, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: Optional[QueriedKnowledge] = None, **kwargs)` — [`L81`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py#L81) — Evaluate LLM fine-tuning implementation using dedicated LLM environment.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`CoSTEERSingleFeedback`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`CoSTEEREvaluator`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`get_ft_env`](../../../components/coder/finetune/conf.md#get_ft_env), [`final_decision`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`scen`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../utils/env.md#EnvResult.exit_code), [`error`](../../../log/logger.md#RDAgentLog.error), [`stdout`](../../../utils/env.md#EnvResult.stdout), [`run`](../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`return_checking`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`FT_YAML_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_YAML_FILE_NAME), [`clear_workspace`](../../../components/coder/finetune/conf.md#clear_workspace), [`code`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`get_workspace_prefix`](../../../components/coder/finetune/conf.md#get_workspace_prefix), [`get_data_processing_env`](../../../components/coder/finetune/conf.md#get_data_processing_env), [`inject_data_stats`](../../../components/coder/finetune/conf.md#inject_data_stats), [`FT_DATA_SCRIPT_NAME`](../../../components/coder/finetune/conf.md#FT_DATA_SCRIPT_NAME), [`running_info`](../../../core/experiment.md#Workspace.running_info), [`val_and_update_init_dict`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`get_task_information`](../../../components/coder/finetune/exp.md#FTTask.get_task_information), [`FTTask`](../../../components/coder/finetune/exp.md#FTTask), [`extract_loss_history`](eval.md#extract_loss_history), [`FT_DATA_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_DATA_FILE_NAME), [`running_time`](../../../core/experiment.md#RunningInfo.running_time), [`running_time`](../../../utils/env.md#EnvResult.running_time), [`feedback`](../../../core/experiment.md#Workspace.feedback), [`get_data_processing_cache_key`](../../../components/coder/finetune/conf.md#get_data_processing_cache_key), [`LLMConfigValidator`](../../../components/coder/finetune/unified_validator.md#LLMConfigValidator)  (+7 more; 2 test-only)
- used by: [`CoSTEEREvaluator`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](runner.md#LLMFinetuneRunner.__init__)

## Functions
- `extract_loss_history(output_path)` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/eval.py#L30) — Extract training and evaluation loss history from LlamaFactory's trainer_state.json.

