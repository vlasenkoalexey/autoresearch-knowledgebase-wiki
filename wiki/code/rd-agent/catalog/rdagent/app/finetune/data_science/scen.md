---
title: 'Module: rdagent/app/finetune/data_science/scen.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/data_science/scen.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.data_science.scen`/DSFinetuneScen#
symbols:
  DSFinetuneScen._get_data_folder_description: _get_data_folder_description().
  DSFinetuneScen: ''
---
# Module: [`rdagent/app/finetune/data_science/scen.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/scen.py)

## Classes
### `DSFinetuneScen`  ·  implements/extends DataScienceScen
- def: [`rdagent/app/finetune/data_science/scen.py:11`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/scen.py#L11)
- doc: DSFinetuneScen Scenario
- signature: `class DSFinetuneScen(DataScienceScen):`
- protocol/private: `_get_data_folder_description`[`L14`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/scen.py#L14)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../data_science/conf.md#DS_RD_SETTING), [`local_data_path`](../../kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`DataScienceScen`](../../../scenarios/data_science/scen/__init__.md#DataScienceScen), [`competition`](../../../scenarios/data_science/scen/__init__.md#DataScienceScen.competition), [`describe_data_folder_v2`](../../../scenarios/data_science/scen/utils.md#describe_data_folder_v2), [`show_nan_columns`](../../data_science/conf.md#DataScienceBasePropSetting.show_nan_columns)
- used by: [`DataScienceScen`](../../../scenarios/data_science/scen/__init__.md#DataScienceScen), [`_get_data_folder_description`](../../../scenarios/data_science/scen/__init__.md#DataScienceScen._get_data_folder_description)

