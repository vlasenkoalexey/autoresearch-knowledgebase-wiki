---
title: 'Module: rdagent/scenarios/finetune/proposal/trace.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/proposal/trace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.proposal.trace`/FTTrace#
symbols:
  FTTrace.get_experiment_info: get_experiment_info().
  FTTrace: ''
  FTTrace.__init__: __init__().
  FTTrace.sota_benchmark: sota_benchmark().
  FTTrace.hist: hist.
  FTTrace.sota_info: sota_info().
---
# Module: [`rdagent/scenarios/finetune/proposal/trace.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py)

## Classes
### `FTTrace`  ·  implements/extends Trace
- def: [`rdagent/scenarios/finetune/proposal/trace.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L23)
- doc: Specialized Trace for LLM Fine-tuning scenario.
- signature: `class FTTrace(Trace["LLMFinetuneScen", KnowledgeBase]):`
- members:
  - `get_experiment_info(self, exp: FTExperiment)` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L49) — Return experiment's full info for hypothesis generation.
  - `sota_benchmark(self)` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L36) — Return SOTA experiment's benchmark results.
  - `sota_info(self)` — [`L75`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L75) — Return SOTA experiment's full info for hypothesis generation.
  - `hist` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L34)
- protocol/private: `__init__`[`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/trace.py#L30)
- uses (calls/refs, reference-scoped): [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Trace`](../../../core/proposal.md#Trace), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`ExperimentFeedback`](../../../core/proposal.md#ExperimentFeedback), [`FT_YAML_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_YAML_FILE_NAME), [`KnowledgeBase`](../../../core/knowledge_base.md#KnowledgeBase), [`FTExperiment`](../experiment/experiment.md#FTExperiment), [`get_sota_experiment`](../../../core/proposal.md#Trace.get_sota_experiment), [`FT_DATA_SCRIPT_NAME`](../../../components/coder/finetune/conf.md#FT_DATA_SCRIPT_NAME), [`running_info`](../../../core/experiment.md#Workspace.running_info), [`LLMFinetuneScen`](../scen/scenario.md#LLMFinetuneScen), [`__init__`](../../../core/proposal.md#Trace.__init__)
- used by: [`Trace`](../../../core/proposal.md#Trace), [`generate_feedback`](../dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`trace`](../loop.md#LLMFinetuneRDLoop.trace)

