---
title: 'Module: rdagent/scenarios/rl/experiment/experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/experiment/experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.experiment.experiment`/RL
symbols:
  RLExperiment: Experiment#
  RLExperiment.__init__: Experiment#__init__().
  RLTask: Task#
---
# Module: [`rdagent/scenarios/rl/experiment/experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/experiment.py)

## Classes
### `RLExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/rl/experiment/experiment.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/experiment.py#L16)
- doc: RL post-training experiment with workspace initialization.
- signature: `class RLExperiment(Experiment[RLTask, RLWorkspace, RLWorkspace]):`
- protocol/private: `__init__`[`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/experiment.py#L19)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../core/experiment.md#Experiment), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`RLTask`](experiment.md#RLTask), [`RLWorkspace`](workspace.md#RLWorkspace)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`gen`](../proposal/proposal.md#RLPostTrainingExpGen.gen)

### `RLTask`  ·  implements/extends Task
- def: [`rdagent/scenarios/rl/experiment/experiment.py:7`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/experiment.py#L7)
- doc: RDLoop 内部的任务描述（每次迭代一个）。
- signature: `class RLTask(Task):`
- uses (calls/refs, reference-scoped): [`Task`](../../../core/experiment.md#Task)
- used by: [`Task`](../../../core/experiment.md#Task), [`gen`](../proposal/proposal.md#RLPostTrainingExpGen.gen), [`RLExperiment`](experiment.md#RLExperiment), [`__init__`](experiment.md#RLExperiment.__init__)

