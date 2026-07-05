---
title: 'Module: rdagent/scenarios/data_science/dev/feedback.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/dev/feedback.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.dev.feedback`/DSExperiment2Feedback#
symbols:
  DSExperiment2Feedback.generate_feedback: generate_feedback().
  DSExperiment2Feedback.__init__: __init__().
  DSExperiment2Feedback: ''
  DSExperiment2Feedback.version: version.
---
# Module: [`rdagent/scenarios/data_science/dev/feedback.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/feedback.py)

## Classes
### `DSExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/data_science/dev/feedback.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/feedback.py#L23)
- signature: `class DSExperiment2Feedback(Experiment2Feedback):`
- members:
  - `generate_feedback(self, exp: DSExperiment, trace: DSTrace)` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/feedback.py#L28) — documented in [rdagent-oai-backend-base](../../../../../concepts/rdagent-oai-backend-base.md)
  - `version` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/feedback.py#L26)
- protocol/private: `__init__`[`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/dev/feedback.py#L24)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../core/scenario.md#Scenario), [`DSExperiment`](../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`DSTrace`](../proposal/exp_gen/base.md#DSTrace), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`result`](../../../core/experiment.md#Experiment.result), [`ExperimentFeedback`](../../../core/proposal.md#ExperimentFeedback), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`knowledge_base`](../../../core/proposal.md#Trace.knowledge_base), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`dict_get_with_warning`](../../../log/utils/__init__.md#dict_get_with_warning), [`scen`](../../../core/proposal.md#Experiment2Feedback.scen), [`sota_experiment`](../proposal/exp_gen/base.md#DSTrace.sota_experiment), [`convert2bool`](../../../utils/__init__.md#convert2bool), [`pending_tasks_list`](../experiment/experiment.md#DSExperiment.pending_tasks_list), [`last_exp_fb`](../proposal/exp_gen/base.md#DSTrace.last_exp_fb), [`enable_knowledge_base`](../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_knowledge_base), [`generate_diff_from_dict`](../../../utils/repo/diff.md#generate_diff_from_dict), [`DSIdea`](../proposal/exp_gen/idea_pool.md#DSIdea), [`__init__`](../../../core/proposal.md#Experiment2Feedback.__init__)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

