---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.launcher.slurm`/SlurmConfig#
symbols:
  SlurmConfig: ''
  SlurmConfig.account: account.
  SlurmConfig.qos: qos.
  SlurmConfig.partition: partition.
  SlurmConfig.validate: validate().
  SlurmConfig.nodes: nodes.
  SlurmConfig.ntasks_per_node: ntasks_per_node.
  SlurmConfig.gpus_per_node: gpus_per_node.
  SlurmConfig.cpus_per_task: cpus_per_task.
  SlurmConfig.time: time.
  SlurmConfig.mem: mem.
  SlurmConfig.array_parallelism: array_parallelism.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py)

## Classes
### `SlurmConfig`  ·  implements/extends LauncherConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py:20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L20)
- signature: `class SlurmConfig(LauncherConfig):`
- members:
  - `validate(self)` — [`L98`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L98)
  - `account` — [`L21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L21)
  - `array_parallelism` — [`L90`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L90)
  - `cpus_per_task` — [`L54`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L54)
  - `gpus_per_node` — [`L48`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L48)
  - `mem` — [`L75`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L75)
  - `nodes` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L35)
  - `ntasks_per_node` — [`L41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L41)
  - `partition` — [`L61`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L61)
  - `qos` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L28)
  - `time` — [`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/launcher/slurm.py#L68)
- uses (calls/refs, reference-scoped): [`LauncherConfig`](base.md#LauncherConfig), [`validate`](base.md#LauncherConfig.validate), [`get_default_slurm_account`](../../utils/environment.md#get_default_slurm_account), [`get_default_slurm_partition`](../../utils/environment.md#get_default_slurm_partition), [`get_default_slurm_qos`](../../utils/environment.md#get_default_slurm_qos)
- used by: [`launch_jobs`](../../main_runner_job_array.md#launch_jobs), [`LauncherConfig`](base.md#LauncherConfig), [`validate`](base.md#LauncherConfig.validate)

