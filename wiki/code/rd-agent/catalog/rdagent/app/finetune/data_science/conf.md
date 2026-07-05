---
title: 'Module: rdagent/app/finetune/data_science/conf.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/data_science/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.data_science.conf`/
symbols:
  update_settings: update_settings().
  DSFinetuneScen: DSFinetuneScen#
  DSFinetuneScen.app_tpl: DSFinetuneScen#app_tpl.
  DSFinetuneScen.model_config: DSFinetuneScen#model_config.
  DSFinetuneScen.scen: DSFinetuneScen#scen.
  DSFinetuneScen.debug_timeout: DSFinetuneScen#debug_timeout.
  DSFinetuneScen.full_timeout: DSFinetuneScen#full_timeout.
  DSFinetuneScen.coder_on_whole_pipeline: DSFinetuneScen#coder_on_whole_pipeline.
  DSFinetuneScen.enable_model_dump: DSFinetuneScen#enable_model_dump.
---
# Module: [`rdagent/app/finetune/data_science/conf.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py)

## Classes
### `DSFinetuneScen`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/app/finetune/data_science/conf.py:9`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L9)
- signature: `class DSFinetuneScen(ExtendedBaseSettings):`
- members:
  - `app_tpl` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L27)
  - `coder_on_whole_pipeline` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L25)
  - `debug_timeout` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L20) — ---
  - `enable_model_dump` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L26)
  - `full_timeout` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L22) — ---
  - `model_config` — [`L10`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L10)
  - `scen` — [`L11`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L11) — ---
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings)
- used by: [`ExtendedBaseSettings`](../../../core/conf.md#ExtendedBaseSettings), [`update_settings`](conf.md#update_settings)

## Functions
- `update_settings(competition: str)` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/data_science/conf.py#L30) — Update the RD_AGENT_SETTINGS with the values from DS_FINETUNE_SETTINGS.

