---
title: 'Module: rdagent/scenarios/finetune/experiment/experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/experiment/experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.experiment.experiment`/
symbols:
  FTExperiment: FTExperiment#
  FTExperiment.__init__: FTExperiment#__init__().
  FTExperiment.is_ready_to_run: FTExperiment#is_ready_to_run().
  COMPONENT: COMPONENT.
  FTExperiment.format_check_result: FTExperiment#format_check_result.
---
# Module: [`rdagent/scenarios/finetune/experiment/experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py)

## Classes
### `FTExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/finetune/experiment/experiment.py:13`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py#L13)
- signature: `class FTExperiment(Experiment[Task, FTWorkspace, FTWorkspace]):`
- members:
  - `is_ready_to_run(self)` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py#L27) — ready to run does not indicate the experiment is runnable
  - `format_check_result` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py#L23)
- protocol/private: `__init__`[`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py#L14)
- uses (calls/refs, reference-scoped): [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../core/experiment.md#Experiment), [`Task`](../../../core/experiment.md#Task), [`FT_YAML_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_YAML_FILE_NAME), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`FTWorkspace`](workspace.md#FTWorkspace)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`_gen_hypothesis`](../proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`generate_feedback`](../dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`gen`](../proposal/proposal.md#LLMFinetuneExpGen.gen), [`get_experiment_info`](../proposal/trace.md#FTTrace.get_experiment_info), [`hist`](../proposal/trace.md#FTTrace.hist)  (1 test-only)

## Module values
- `COMPONENT` — [`L10`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/experiment.py#L10)

