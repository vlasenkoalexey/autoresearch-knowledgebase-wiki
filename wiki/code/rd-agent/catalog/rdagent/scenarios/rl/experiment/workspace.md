---
title: 'Module: rdagent/scenarios/rl/experiment/workspace.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/experiment/workspace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.experiment.workspace`/RLWorkspace#
symbols:
  RLWorkspace.run: run().
  RLWorkspace: ''
---
# Module: [`rdagent/scenarios/rl/experiment/workspace.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/workspace.py)

## Classes
### `RLWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/scenarios/rl/experiment/workspace.py:19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/workspace.py#L19)
- doc: RL 训练工作区
- signature: `class RLWorkspace(FBWorkspace):`
- members:
  - `run(self, env: Env, entry: str)` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/experiment/workspace.py#L22) — 在环境中执行命令
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`run`](../../../utils/env.md#Env.run), [`exit_code`](../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../utils/env.md#EnvResult.stdout), [`Env`](../../../utils/env.md#Env), [`DockerEnv`](../../../utils/env.md#DockerEnv), [`prepare`](../../../core/experiment.md#FBWorkspace.prepare), [`EnvResult`](../../../utils/env.md#EnvResult), [`running_time`](../../../utils/env.md#EnvResult.running_time)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`run`](../../../core/experiment.md#FBWorkspace.run), [`RLExperiment`](experiment.md#RLExperiment), [`__init__`](experiment.md#RLExperiment.__init__)

