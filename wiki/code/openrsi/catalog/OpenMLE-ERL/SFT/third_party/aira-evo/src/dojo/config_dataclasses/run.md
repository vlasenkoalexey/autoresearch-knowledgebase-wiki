---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.run`/RunConfig#
symbols:
  RunConfig: ''
  RunConfig.logger: logger.
  RunConfig.load_from_json: load_from_json().
  RunConfig.metadata: metadata.
  RunConfig.task: task.
  RunConfig.save: save().
  RunConfig.solver: solver.
  RunConfig.from_dict: from_dict().
  RunConfig.interpreter: interpreter.
  RunConfig.meta_id: meta_id.
  RunConfig.id: id.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py)

## Classes
### `RunConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py:22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L22)
- signature: `class RunConfig(BaseConfig):`
- members:
  - `from_dict(cls, data: dict)` — [`L64`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L64)
  - `load_from_json(cls, json_path: str)` — [`L55`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L55) — Load a RunConfig from a JSON file.
  - `save(self)` — [`L43`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L43) — For distributed training, be careful to only call this function on the main process.
  - `id` — [`L23`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L23)
  - `interpreter` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L41)
  - `logger` — [`L37`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L37)
  - `meta_id` — [`L27`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L27)
  - `metadata` — [`L38`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L38)
  - `solver` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L40)
  - `task` — [`L39`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/run.py#L39)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`SolverConfig`](solver/base.md#SolverConfig), [`LoggerConfig`](logger.md#LoggerConfig), [`output_dir`](logger.md#LoggerConfig.output_dir), [`InterpreterConfig`](interpreter/base.md#InterpreterConfig), [`TaskConfig`](task/base.md#TaskConfig), [`MetadataConfig`](metadata.md#MetadataConfig), [`dataclass_from_dict`](utils.md#dataclass_from_dict)
- used by: [`_main`](../main_run.md#_main), [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`_main`](../main_runner_job_array.md#_main), [`write_tree_reports`](../analysis_utils/meta_tree_analysis.md#write_tree_reports), [`_load_experiment_data`](../analysis_utils/meta_data_wrangling.md#_load_experiment_data), [`launch_jobs`](../main_runner_job_array.md#launch_jobs), [`main`](../main_run.md#main), [`get_submitit_logs2exp_mapping`](../analysis_utils/meta_data_wrangling.md#get_submitit_logs2exp_mapping), [`metaexp2ids`](../analysis_utils/meta_data_wrangling.md#metaexp2ids), [`slurm_id_to_log`](../analysis_utils/meta_error_summary.md#slurm_id_to_log), [`journal_into_tree`](../analysis_utils/journal_to_tree.md#journal_into_tree), [`generate_id`](omegaconf/resolvers.md#generate_id), [`get_competition_id_from_cmd`](../analysis_utils/meta_data_wrangling.md#get_competition_id_from_cmd), [`print_config_tree`](../utils/rich_utils.md#print_config_tree), [`get_seed_from_cmd`](../analysis_utils/meta_data_wrangling.md#get_seed_from_cmd), [`get_exp_name_from_cmd`](../analysis_utils/meta_data_wrangling.md#get_exp_name_from_cmd)

