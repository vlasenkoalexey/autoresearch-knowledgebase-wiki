---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.metadata`/MetadataConfig#
symbols:
  MetadataConfig: ''
  MetadataConfig.slurm_id: slurm_id.
  MetadataConfig.seed: seed.
  MetadataConfig.script_id: script_id.
  MetadataConfig.git_issue_id: git_issue_id.
  MetadataConfig.description: description.
  MetadataConfig.launch_time: launch_time.
  MetadataConfig.base_path: base_path.
  MetadataConfig.user: user.
  MetadataConfig.git_commit_id: git_commit_id.
  MetadataConfig.torch_version: torch_version.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py)

## Classes
### `MetadataConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L15)
- signature: `class MetadataConfig(BaseConfig):`
- members:
  - `base_path` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L40)
  - `description` — [`L26`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L26)
  - `git_commit_id` — [`L53`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L53)
  - `git_issue_id` — [`L20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L20)
  - `launch_time` — [`L33`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L33)
  - `script_id` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L16)
  - `seed` — [`L30`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L30)
  - `slurm_id` — [`L66`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L66)
  - `torch_version` — [`L60`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L60)
  - `user` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/metadata.py#L44)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../aira_core/config/base.md#BaseConfig)
- used by: [`_main`](../main_run.md#_main), [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`_load_experiment_data`](../analysis_utils/meta_data_wrangling.md#_load_experiment_data), [`get_submitit_logs2exp_mapping`](../analysis_utils/meta_data_wrangling.md#get_submitit_logs2exp_mapping), [`metaexp2ids`](../analysis_utils/meta_data_wrangling.md#metaexp2ids), [`slurm_id_to_log`](../analysis_utils/meta_error_summary.md#slurm_id_to_log), [`metadata`](run.md#RunConfig.metadata), [`get_seed_from_cmd`](../analysis_utils/meta_data_wrangling.md#get_seed_from_cmd), [`metadata`](runner.md#RunnerConfig.metadata)

