---
title: 'Module: rdagent/scenarios/qlib/developer/feedback.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/developer/feedback.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.developer.feedback`/
symbols:
  QlibFactorExperiment2Feedback.generate_feedback: QlibFactorExperiment2Feedback#generate_feedback().
  QlibModelExperiment2Feedback.generate_feedback: QlibModelExperiment2Feedback#generate_feedback().
  process_results: process_results().
  IMPORTANT_METRICS: IMPORTANT_METRICS.
  QlibFactorExperiment2Feedback: QlibFactorExperiment2Feedback#
  QlibModelExperiment2Feedback: QlibModelExperiment2Feedback#
  process_results.format_filtered_combined_df: process_results().format_filtered_combined_df().
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/scenarios/qlib/developer/feedback.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py)

## Classes
### `QlibFactorExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/qlib/developer/feedback.py:54`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L54)
- signature: `class QlibFactorExperiment2Feedback(Experiment2Feedback):`
- members:
  - `generate_feedback(self, exp: Experiment, trace: Trace)` — [`L55`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L55) — Generate feedback for the given experiment and hypothesis.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`Experiment`](../../../core/experiment.md#Experiment), [`Trace`](../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`result`](../../../core/experiment.md#Experiment.result), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`scen`](../../../core/proposal.md#Experiment2Feedback.scen), [`QlibQuantScenario`](../experiment/quant_experiment.md#QlibQuantScenario), [`get_scenario_all_desc`](../experiment/quant_experiment.md#QlibQuantScenario.get_scenario_all_desc), [`convert2bool`](../../../utils/__init__.md#convert2bool), [`process_results`](feedback.md#process_results)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

### `QlibModelExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/qlib/developer/feedback.py:121`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L121)
- signature: `class QlibModelExperiment2Feedback(Experiment2Feedback):`
- members:
  - `generate_feedback(self, exp: Experiment, trace: Trace)` — [`L122`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L122) — Generate feedback for the given experiment and hypothesis.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`Experiment`](../../../core/experiment.md#Experiment), [`Trace`](../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`result`](../../../core/experiment.md#Experiment.result), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`scen`](../../../core/proposal.md#Experiment2Feedback.scen), [`QlibQuantScenario`](../experiment/quant_experiment.md#QlibQuantScenario), [`get_scenario_all_desc`](../experiment/quant_experiment.md#QlibQuantScenario.get_scenario_all_desc), [`get_sota_hypothesis_and_experiment`](../../../core/proposal.md#Trace.get_sota_hypothesis_and_experiment), [`convert2bool`](../../../utils/__init__.md#convert2bool), [`IMPORTANT_METRICS`](feedback.md#IMPORTANT_METRICS)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

## Functions
- `format_filtered_combined_df(filtered_combined_df: pd.DataFrame)` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L43)
- `process_results(current_result, sota_result)` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L24)

## Module values
- `DIRNAME` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L15)
- `IMPORTANT_METRICS` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/developer/feedback.py#L17)

