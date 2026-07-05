---
title: 'Module: rdagent/scenarios/finetune/dev/feedback.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/dev/feedback.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.dev.feedback`/FTExperiment2Feedback#
symbols:
  FTExperiment2Feedback.generate_feedback: generate_feedback().
  FTExperiment2Feedback.__init__: __init__().
  FTExperiment2Feedback: ''
  FTExperiment2Feedback.version: version.
---
# Module: [`rdagent/scenarios/finetune/dev/feedback.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/dev/feedback.py)

## Classes
### `FTExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/finetune/dev/feedback.py:28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/dev/feedback.py#L28)
- doc: Generate feedback for LLM fine-tuning experiments
- signature: `class FTExperiment2Feedback(Experiment2Feedback):`
- members:
  - `generate_feedback(self, exp: FTExperiment, trace: FTTrace | None = None, exception: Exception | None = None)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/dev/feedback.py#L35) — Generate comprehensive feedback for LLM fine-tuning experiment. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `version` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/dev/feedback.py#L33)
- protocol/private: `__init__`[`L31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/dev/feedback.py#L31)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../core/scenario.md#Scenario), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`ExperimentFeedback`](../../../core/proposal.md#ExperimentFeedback), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`FTExperiment`](../experiment/experiment.md#FTExperiment), [`dict_get_with_warning`](../../../log/utils/__init__.md#dict_get_with_warning), [`scen`](../../../core/proposal.md#Experiment2Feedback.scen), [`running_info`](../../../core/experiment.md#Workspace.running_info), [`FTTrace`](../proposal/trace.md#FTTrace), [`convert2bool`](../../../utils/__init__.md#convert2bool), [`running_time`](../../../core/experiment.md#RunningInfo.running_time), [`feedback`](../../../core/experiment.md#Workspace.feedback), [`force_think_token`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.force_think_token), [`sota_benchmark`](../proposal/trace.md#FTTrace.sota_benchmark), [`__init__`](../../../core/proposal.md#Experiment2Feedback.__init__), [`result`](../../../core/experiment.md#RunningInfo.result)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

