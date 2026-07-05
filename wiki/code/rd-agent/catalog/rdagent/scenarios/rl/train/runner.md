---
title: 'Module: rdagent/scenarios/rl/train/runner.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/train/runner.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.train.runner`/RLPostTrainingRunner#
symbols:
  RLPostTrainingRunner.develop: develop().
  RLPostTrainingRunner.__init__: __init__().
  RLPostTrainingRunner.timeout: timeout.
  RLPostTrainingRunner: ''
  RLPostTrainingRunner._find_latest_model: _find_latest_model().
---
# Module: [`rdagent/scenarios/rl/train/runner.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py)

## Classes
### `RLPostTrainingRunner`  ·  implements/extends Developer
- def: [`rdagent/scenarios/rl/train/runner.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py#L23)
- doc: RL Runner - 本地执行训练 + HTTP API 评测
- signature: `class RLPostTrainingRunner(Developer):`
- members:
  - `_find_latest_model(output_dir: Path)` — [`L131`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py#L131) — 找到 output/ 下的模型路径。
  - `develop(self, exp: Experiment)` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py#L30) — 执行训练代码并提交评测
  - `timeout` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py#L28)
- protocol/private: `__init__`[`L26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/train/runner.py#L26)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`Scenario`](../../../core/scenario.md#Scenario), [`Experiment`](../../../core/experiment.md#Experiment), [`error`](../../../log/logger.md#RDAgentLog.error), [`Developer`](../../../core/developer.md#Developer), [`result`](../../../core/experiment.md#Experiment.result), [`scen`](../../../core/developer.md#Developer.scen)
- used by: [`Developer`](../../../core/developer.md#Developer), [`develop`](../../../core/developer.md#Developer.develop)

