---
title: 'Module: rdagent/log/ui/conf.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.conf`/UI
symbols:
  UI_SETTING: _SETTING.
  UIBasePropSetting.enable_cache: BasePropSetting#enable_cache.
  UIBasePropSetting.static_path: BasePropSetting#static_path.
  UIBasePropSetting: BasePropSetting#
  UIBasePropSetting.amlt_path: BasePropSetting#amlt_path.
  UIBasePropSetting.trace_folder: BasePropSetting#trace_folder.
  UIBasePropSetting.default_log_folders: BasePropSetting#default_log_folders.
  UIBasePropSetting.baseline_result_path: BasePropSetting#baseline_result_path.
  UIBasePropSetting.aide_path: BasePropSetting#aide_path.
  UIBasePropSetting.model_config: BasePropSetting#model_config.
---
# Module: [`rdagent/log/ui/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py)

## Classes
### `UIBasePropSetting`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/log/ui/conf.py:6`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L6)
- signature: `class UIBasePropSetting(ExtendedBaseSettings):`
- members:
  - `aide_path` — [`L13`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L13)
  - `amlt_path` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L15)
  - `baseline_result_path` — [`L11`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L11)
  - `default_log_folders` — [`L9`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L9)
  - `enable_cache` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L21)
  - `model_config` — [`L7`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L7)
  - `static_path` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L17)
  - `trace_folder` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L19)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings)
- used by: [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings), [`app`](../server/app.md#app), [`UI_SETTING`](conf.md#UI_SETTING), [`get_summary_df`](utils.md#get_summary_df), [`update_trace`](../server/app.md#update_trace), [`app`](../server/debug_app.md#app), [`log`](storage.md#WebStorage.log), [`log_folder_path`](../server/app.md#log_folder_path), [`aide_path`](aide.md#aide_path), [`compare`](utils.md#compare), [`convert_log_folder_str`](dsapp.md#convert_log_folder_str), [`_normalize_static_request_path`](../server/app.md#_normalize_static_request_path)

## Module values
- `UI_SETTING` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/conf.py#L24)

