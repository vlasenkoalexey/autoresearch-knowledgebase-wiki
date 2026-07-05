---
title: 'Module: rdagent/scenarios/data_science/dev/runner/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/dev/runner/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.dev.runner.eval`/D
symbols:
  DSRunnerEvaluator.evaluate: SRunnerEvaluator#evaluate().
  DSRunnerFeedback.__str__: SRunnerFeedback#__str__().
  DSRunnerFeedback.acceptable: SRunnerFeedback#acceptable.
  DSRunnerFeedback: SRunnerFeedback#
  DSRunnerFeedback.is_acceptable: SRunnerFeedback#is_acceptable().
  DSRunnerEvaluator: SRunnerEvaluator#
  DSRunnerFeedback.score: SRunnerFeedback#score.
  DSCoSTEEREvalFeedback: SCoSTEEREvalFeedback.
  DSRunnerFeedback.hyperparameter_tuning_decision: SRunnerFeedback#hyperparameter_tuning_decision.
  DSRunnerFeedback.hyperparameter_tuning_suggestion: SRunnerFeedback#hyperparameter_tuning_suggestion.
  DIRNAME: IRNAME.
---
# Module: [`rdagent/scenarios/data_science/dev/runner/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py)

## Classes
### `DSRunnerEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/scenarios/data_science/dev/runner/eval.py:72`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L72)
- signature: `class DSRunnerEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L74`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L74) — documented in [rdagent-app-data_science-conf](../../../../../../concepts/rdagent-app-data_science-conf.md)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`warning`](../../../../log/logger.md#RDAgentLog.warning), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`conf`](../../../../utils/env.md#Env.conf), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../../../../components/coder/data_science/conf.md#get_ds_env), [`CoSTEEREvaluator`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`scen`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../../utils/env.md#EnvResult.exit_code), [`error`](../../../../log/logger.md#RDAgentLog.error), [`stdout`](../../../../utils/env.md#EnvResult.stdout), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`run`](../../../../core/experiment.md#FBWorkspace.run), [`RD_Agent_TIMER_wrapper`](../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../../core/evolving_framework.md#QueriedKnowledge), [`local_data_path`](../../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`remain_time`](../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../log/timer.md#RDAgentTimerWrapper.timer), [`code`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`all_codes`](../../../../core/experiment.md#FBWorkspace.all_codes), [`all_duration`](../../../../log/timer.md#RDAgentTimer.all_duration), [`remove_eda_part`](../../../../components/coder/data_science/utils.md#remove_eda_part), [`coder_on_whole_pipeline`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`get_clear_ws_cmd`](../../../../components/coder/data_science/conf.md#get_clear_ws_cmd), [`running_info`](../../../../core/experiment.md#Workspace.running_info), [`merge_hours`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`DSRunnerCoSTEERSettings`](__init__.md#DSRunnerCoSTEERSettings), [`acceptable`](eval.md#DSRunnerFeedback.acceptable)  (+13 more; 3 test-only)
- used by: [`CoSTEEREvaluator`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#DSCoSTEERRunner.__init__)

### `DSRunnerFeedback`  ·  implements/extends CoSTEERSingleFeedback
- def: [`rdagent/scenarios/data_science/dev/runner/eval.py:34`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L34)
- doc: Feedback for Data Science CoSTEER evaluation.
- signature: `class DSRunnerFeedback(CoSTEERSingleFeedback):`
- members:
  - `is_acceptable(self)` — [`L45`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L45)
  - `acceptable` — [`L40`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L40)
  - `hyperparameter_tuning_decision` — [`L41`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L41)
  - `hyperparameter_tuning_suggestion` — [`L42`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L42)
  - `score` — [`L43`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L43)
- protocol/private: `__str__`[`L50`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L50)
- uses (calls/refs, reference-scoped): [`CoSTEERSingleFeedback`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`return_checking`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`code`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`is_acceptable`](../../../../core/evaluation.md#Feedback.is_acceptable)
- used by: [`evaluate`](eval.md#DSRunnerEvaluator.evaluate), [`CoSTEERSingleFeedback`](../../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`is_acceptable`](../../../../core/evaluation.md#Feedback.is_acceptable), [`DSCoSTEEREvalFeedback`](eval.md#DSCoSTEEREvalFeedback)

## Module values
- `DIRNAME` — [`L30`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L30)
- `DSCoSTEEREvalFeedback` — [`L69`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/runner/eval.py#L69)

