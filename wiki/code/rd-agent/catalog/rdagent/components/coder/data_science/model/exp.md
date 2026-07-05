---
title: 'Module: rdagent/components/coder/data_science/model/exp.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/model/exp.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.model.exp`/ModelTask#
symbols:
  ModelTask: ''
  ModelTask.get_task_information: get_task_information().
  ModelTask.__init__: __init__().
---
# Module: [`rdagent/components/coder/data_science/model/exp.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/exp.py)

## Classes
### `ModelTask`  ·  implements/extends CoSTEERTask
- def: [`rdagent/components/coder/data_science/model/exp.py:7`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/exp.py#L7)
- signature: `class ModelTask(CoSTEERTask):`
- members:
  - `get_task_information(self)` — [`L17`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/exp.py#L17)
- protocol/private: `__init__`[`L8`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/model/exp.py#L8)
- uses (calls/refs, reference-scoped): [`CoSTEERTask`](../../CoSTEER/task.md#CoSTEERTask), [`name`](../../../../core/experiment.md#AbsTask.name), [`description`](../../../../core/experiment.md#Task.description), [`__init__`](../../CoSTEER/task.md#CoSTEERTask.__init__)
- used by: [`gen`](../../../../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftExpGen.gen), [`implement_one_task`](__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`coding`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.coding), [`CoSTEERTask`](../../CoSTEER/task.md#CoSTEERTask), [`develop_one_competition`](test.md#develop_one_competition), [`_COMPONENT_META`](../../../../scenarios/data_science/proposal/exp_gen/proposal.md#_COMPONENT_META._COMPONENT_META), [`_COMPONENT_META`](../../../../scenarios/data_science/proposal/exp_gen/utils.md#_COMPONENT_META._COMPONENT_META)

