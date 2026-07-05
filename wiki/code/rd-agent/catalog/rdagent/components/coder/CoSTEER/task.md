---
title: 'Module: rdagent/components/coder/CoSTEER/task.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/CoSTEER/task.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.CoSTEER.task`/CoSTEERTask#
symbols:
  CoSTEERTask: ''
  CoSTEERTask.__init__: __init__().
  CoSTEERTask.base_code: base_code.
---
# Module: [`rdagent/components/coder/CoSTEER/task.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/task.py)

## Classes
### `CoSTEERTask`  ·  implements/extends Task
- def: [`rdagent/components/coder/CoSTEER/task.py:4`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/task.py#L4) — documented in [rdagent-components-coder-factor_coder-factor](../../../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- signature: `class CoSTEERTask(Task):`
- members:
  - `base_code` — [`L9`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/task.py#L9)
- protocol/private: `__init__`[`L5`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/task.py#L5)
- uses (calls/refs, reference-scoped): [`Task`](../../../core/experiment.md#Task), [`FactorTask`](../factor_coder/factor.md#FactorTask), [`ModelTask`](../model_coder/model.md#ModelTask), [`PipelineTask`](../data_science/pipeline/exp.md#PipelineTask), [`WorkflowTask`](../data_science/workflow/exp.md#WorkflowTask), [`DataLoaderTask`](../data_science/raw_data_loader/exp.md#DataLoaderTask), [`EnsembleTask`](../data_science/ensemble/exp.md#EnsembleTask), [`FeatureTask`](../data_science/feature/exp.md#FeatureTask), [`ModelTask`](../data_science/model/exp.md#ModelTask), [`FTTask`](../finetune/exp.md#FTTask), [`__init__`](../../../core/experiment.md#Task.__init__)
- used by: [`Task`](../../../core/experiment.md#Task), [`implement_one_task`](../../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`FactorTask`](../factor_coder/factor.md#FactorTask), [`ModelTask`](../model_coder/model.md#ModelTask), [`develop`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`develop_one_competition`](../data_science/model/test.md#develop_one_competition), [`develop_one_competition`](../data_science/workflow/test.md#develop_one_competition), [`PipelineTask`](../data_science/pipeline/exp.md#PipelineTask), [`WorkflowTask`](../data_science/workflow/exp.md#WorkflowTask), [`model_type`](../model_coder/model.md#ModelTask.model_type), [`DataLoaderTask`](../data_science/raw_data_loader/exp.md#DataLoaderTask), [`EnsembleTask`](../data_science/ensemble/exp.md#EnsembleTask), [`FeatureTask`](../data_science/feature/exp.md#FeatureTask), [`ModelTask`](../data_science/model/exp.md#ModelTask), [`FTTask`](../finetune/exp.md#FTTask), [`factor_implementation`](../factor_coder/factor.md#FactorTask.factor_implementation), [`__init__`](../data_science/model/exp.md#ModelTask.__init__), [`__init__`](../data_science/pipeline/exp.md#PipelineTask.__init__), [`__init__`](../data_science/workflow/exp.md#WorkflowTask.__init__), [`__init__`](../finetune/exp.md#FTTask.__init__)

