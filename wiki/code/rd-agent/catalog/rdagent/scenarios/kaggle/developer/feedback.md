---
title: 'Module: rdagent/scenarios/kaggle/developer/feedback.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/developer/feedback.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.developer.feedback`/KGExperiment2Feedback#
symbols:
  KGExperiment2Feedback.generate_feedback: generate_feedback().
  KGExperiment2Feedback.process_results: process_results().
  KGExperiment2Feedback: ''
---
# Module: [`rdagent/scenarios/kaggle/developer/feedback.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/feedback.py)

## Classes
### `KGExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/kaggle/developer/feedback.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/feedback.py#L16)
- signature: `class KGExperiment2Feedback(Experiment2Feedback):`
- members:
  - `generate_feedback(self, exp: Experiment, trace: Trace)` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/feedback.py#L40) — The `ti` should be executed and the results should be included, as well as the comparison between previous results (done by LLM). — documented in [rdagent-core-experiment](../../../../../concepts/rdagent-core-experiment.md)
  - `process_results(self, current_result, sota_result)` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/feedback.py#L17)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`hist`](../../../core/proposal.md#Trace.hist), [`Experiment`](../../../core/experiment.md#Experiment), [`Trace`](../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`UndirectedNode`](../../../components/knowledge_management/graph.md#UndirectedNode), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`result`](../../../core/experiment.md#Experiment.result), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`knowledge_base`](../../../core/proposal.md#Trace.knowledge_base), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`scen`](../../../core/proposal.md#Experiment2Feedback.scen), [`KG_SELECT_MAPPING`](../experiment/kaggle_experiment.md#KG_SELECT_MAPPING), [`reason`](../../../core/proposal.md#Hypothesis.reason), [`convert2bool`](../../../utils/__init__.md#convert2bool), [`sub_results`](../../../core/experiment.md#Experiment.sub_results)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

