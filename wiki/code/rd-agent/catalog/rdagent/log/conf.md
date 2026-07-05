---
title: 'Module: rdagent/log/conf.py'
type: catalog
provenance: extracted
module: rdagent/log/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.conf`/L
symbols:
  LOG_SETTINGS: OG_SETTINGS.
  LogSettings.set_ui_server_port: ogSettings#set_ui_server_port().
  LogSettings.model_post_init: ogSettings#model_post_init().
  LogSettings.trace_path: ogSettings#trace_path.
  LogSettings: ogSettings#
  LogSettings.storages: ogSettings#storages.
  LogSettings.format_console: ogSettings#format_console.
  LogSettings.ui_server_port: ogSettings#ui_server_port.
  LogSettings.model_config: ogSettings#model_config.
---
# Module: [`rdagent/log/conf.py`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py)

## Classes
### `LogSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/log/conf.py:10`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L10)
- signature: `class LogSettings(ExtendedBaseSettings):`
- members:
  - `model_post_init(self, _context: Any,)` — [`L30`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L30)
  - `set_ui_server_port(self, port: int | None)` — [`L22`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L22)
  - `format_console` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L15) — ---
  - `model_config` — [`L11`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L11)
  - `storages` — [`L20`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L20)
  - `trace_path` — [`L13`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L13)
  - `ui_server_port` — [`L18`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L18)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../core/conf.md#ExtendedBaseSettings)
- used by: [`ExtendedBaseSettings`](../core/conf.md#ExtendedBaseSettings), [`_run`](server/app.md#RDAgentTask._run), [`LOG_SETTINGS`](conf.md#LOG_SETTINGS), [`session_folder`](../utils/workflow/loop.md#LoopBase.session_folder), [`refresh_storages_from_settings`](logger.md#RDAgentLog.refresh_storages_from_settings), [`storage`](logger.md#RDAgentLog.storage), [`_configure_console_sinks`](logger.md#RDAgentLog._configure_console_sinks), [`file_path`](../app/utils/ape.md#file_path)

## Module values
- `LOG_SETTINGS` — [`L34`](../../../../../../raw/code/rd-agent/rdagent/log/conf.py#L34)

