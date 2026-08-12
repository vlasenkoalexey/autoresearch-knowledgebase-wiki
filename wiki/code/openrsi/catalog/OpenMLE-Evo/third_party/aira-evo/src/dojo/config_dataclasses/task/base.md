---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.task.base`/TaskConfig#
symbols:
  TaskConfig: ''
  TaskConfig.name: name.
  TaskConfig.validate: validate().
  TaskConfig.data_dir: data_dir.
  TaskConfig.benchmark: benchmark.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py)

## Classes
### `TaskConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py#L15)
- signature: `class TaskConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L36`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py#L36)
  - `benchmark` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py#L22)
  - `data_dir` — [`L28`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py#L28)
  - `name` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/base.py#L16)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`MLEBenchTaskConfig`](mlebench.md#MLEBenchTaskConfig), [`validate`](mlebench.md#MLEBenchTaskConfig.validate)
- used by: [`_main`](../../main_run.md#_main), [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`execute_code`](../../grade_code.md#execute_code), [`step_task`](../../tasks/mlebench/task.md#MLEBenchTask.step_task), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`write_tree_reports`](../../analysis_utils/meta_tree_analysis.md#write_tree_reports), [`evaluate_fitness`](../../tasks/mlebench/task.md#MLEBenchTask.evaluate_fitness), [`_load_experiment_data`](../../analysis_utils/meta_data_wrangling.md#_load_experiment_data), [`to_cfg_list`](../benchmark.md#BenchmarkConfig.to_cfg_list), [`MLEBenchTaskConfig`](mlebench.md#MLEBenchTaskConfig), [`get_competition_id_from_cmd`](../../analysis_utils/meta_data_wrangling.md#get_competition_id_from_cmd), [`task`](../run.md#RunConfig.task), [`competition`](../../tasks/mlebench/task.md#MLEBenchTask.competition), [`__init__`](../../core/tasks/base.md#Task.__init__), [`validate`](mlebench.md#MLEBenchTaskConfig.validate)

