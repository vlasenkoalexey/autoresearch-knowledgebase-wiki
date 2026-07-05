---
title: 'Module: rdagent/scenarios/finetune/experiment/workspace.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/experiment/workspace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.experiment.workspace`/FTWorkspace#
symbols:
  FTWorkspace.run: run().
  FTWorkspace.__init__: __init__().
  FTWorkspace: ''
---
# Module: [`rdagent/scenarios/finetune/experiment/workspace.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/workspace.py)

## Classes
### `FTWorkspace`  ·  implements/extends FBWorkspace
- def: [`rdagent/scenarios/finetune/experiment/workspace.py:27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/workspace.py#L27)
- doc: Fine-tuning workspace with minimal checkpoint strategy and unified Docker logging.
- signature: `class FTWorkspace(FBWorkspace):`
- members:
  - `run(self, env: Env, entry: str, env_vars: dict | None = None, cache_key_extra_func: CacheKeyFunc | None = None, cache_files_to_extract: list[str] | None = None)` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/workspace.py#L48) — Execute the code in the environment with unified Docker logging.
- protocol/private: `__init__`[`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/experiment/workspace.py#L37)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../core/experiment.md#FBWorkspace.workspace_path), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../../core/conf.md#RD_AGENT_SETTINGS), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`run`](../../../utils/env.md#Env.run), [`exit_code`](../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../utils/env.md#EnvResult.stdout), [`Env`](../../../utils/env.md#Env), [`DockerEnv`](../../../utils/env.md#DockerEnv), [`LocalEnv`](../../../utils/env.md#LocalEnv), [`FT_YAML_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_YAML_FILE_NAME), [`prepare`](../../../core/experiment.md#FBWorkspace.prepare), [`EnvResult`](../../../utils/env.md#EnvResult), [`running_time`](../../../utils/env.md#EnvResult.running_time), [`__init__`](../../../core/experiment.md#FBWorkspace.__init__), [`CacheKeyFunc`](../../../utils/env.md#CacheKeyFunc), [`workspace_ckp_size_limit`](../../../core/conf.md#RDAgentSettings.workspace_ckp_size_limit), [`workspace_ckp_white_list_names`](../../../core/conf.md#RDAgentSettings.workspace_ckp_white_list_names)
- used by: [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`run`](../../../core/experiment.md#FBWorkspace.run), [`run_baseline_model_evaluation`](../scen/scenario.md#LLMFinetuneScen.run_baseline_model_evaluation), [`FTExperiment`](experiment.md#FTExperiment), [`__init__`](experiment.md#FTExperiment.__init__)

