---
title: 'Module: rdagent/scenarios/rl/scen/scenario.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/scen/scenario.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.scen.scenario`/RLPostTrainingScen#
symbols:
  RLPostTrainingScen.grading_server_url: grading_server_url.
  RLPostTrainingScen.background: background().
  RLPostTrainingScen.task_description: task_description.
  RLPostTrainingScen.benchmark: benchmark.
  RLPostTrainingScen.base_model: base_model.
  RLPostTrainingScen.__init__: __init__().
  RLPostTrainingScen.get_runtime_environment: get_runtime_environment().
  RLPostTrainingScen: ''
  RLPostTrainingScen.workspace: workspace.
  RLPostTrainingScen.model_path: model_path.
  RLPostTrainingScen.data_path: data_path.
  RLPostTrainingScen.output_dir: output_dir.
---
# Module: [`rdagent/scenarios/rl/scen/scenario.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py)

## Classes
### `RLPostTrainingScen`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/rl/scen/scenario.py:21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L21)
- doc: RL Post-training Scenario
- signature: `class RLPostTrainingScen(Scenario):`
- members:
  - `background(self)` — [`L59`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L59) — Background information for LLM prompts
  - `get_runtime_environment(self)` — [`L77`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L77) — Get runtime environment info
  - `base_model` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L31)
  - `benchmark` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L32)
  - `data_path` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L35)
  - `grading_server_url` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L37)
  - `model_path` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L34)
  - `output_dir` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L36)
  - `task_description` — [`L52`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L52)
  - `workspace` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L33)
- protocol/private: `__init__`[`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/scen/scenario.py#L27)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`Scenario`](../../../core/scenario.md#Scenario), [`RL_RD_SETTING`](../../../app/rl/conf.md#RL_RD_SETTING), [`base_model`](../../../app/rl/conf.md#RLPostTrainingPropSetting.base_model), [`benchmark`](../../../app/rl/conf.md#RLPostTrainingPropSetting.benchmark)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`get_runtime_environment`](../../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../../core/scenario.md#Scenario.background), [`__init__`](../loop.md#RLPostTrainingRDLoop.__init__)

