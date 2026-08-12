---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.launcher.base`/LauncherConfig#
symbols:
  LauncherConfig: ''
  LauncherConfig.validate: validate().
  LauncherConfig.debug: debug.
  LauncherConfig.monitor_jobs: monitor_jobs.
  LauncherConfig.await_completion: await_completion.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py)

## Classes
### `LauncherConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py:15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py#L15)
- signature: `class LauncherConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L43`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py#L43)
  - `await_completion` — [`L16`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py#L16)
  - `debug` — [`L25`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py#L25)
  - `monitor_jobs` — [`L34`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/base.py#L34)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`SlurmConfig`](slurm.md#SlurmConfig), [`validate`](slurm.md#SlurmConfig.validate)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`_main`](../../main_runner_job_array.md#_main), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`launch_jobs`](../../main_runner_job_array.md#launch_jobs), [`main`](../../main_runner_job_array.md#main), [`launcher`](../runner.md#RunnerConfig.launcher), [`SlurmConfig`](slurm.md#SlurmConfig), [`validate`](slurm.md#SlurmConfig.validate)

