---
title: 'Module: rdagent/log/server/app.py'
type: catalog
provenance: extracted
module: rdagent/log/server/app.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.server.app`/
symbols:
  RDAgentTask._run: RDAgentTask#_run().
  app: app.
  update_trace: update_trace().
  read_trace: read_trace().
  control_process: control_process().
  RDAgentTask.messages: RDAgentTask#messages.
  log_folder_path: log_folder_path.
  RDAgentTask.process: RDAgentTask#process.
  rdagent_processes.rdagent_processes: rdagent_processes.rdagent_processes.
  RDAgentTask.user_response_q: RDAgentTask#user_response_q.
  upload_file: upload_file().
  main: main().
  _get_or_create_task: _get_or_create_task().
  submit_user_interaction_response: submit_user_interaction_response().
  test: test().
  RDAgentTask.stop: RDAgentTask#stop().
  _drain_user_requests_into_messages: _drain_user_requests_into_messages().
  _resolve_stdout_path: _resolve_stdout_path().
  _load_existing_traces: _load_existing_traces().
  RDAgentTask.target_name: RDAgentTask#target_name.
  list_traces: list_traces().
  receive_msgs: receive_msgs().
  RDAgentTask.kwargs: RDAgentTask#kwargs.
  _configure_app_logger: _configure_app_logger().
  _normalize_static_request_path: _normalize_static_request_path().
  _YellowWarningFormatter.format: _YellowWarningFormatter#format().
  RDAgentTask: RDAgentTask#
  download_stdout_file: download_stdout_file().
  server_static_files: server_static_files().
  RDAgentTask.is_alive: RDAgentTask#is_alive().
  RDAgentTask.stdout_path: RDAgentTask#stdout_path.
  RDAgentTask.pointers: RDAgentTask#pointers.
  RDAgentTask.start: RDAgentTask#start().
  RDAgentTask.get_end_code: RDAgentTask#get_end_code().
  RDAgentTask.user_request_q: RDAgentTask#user_request_q.
  favicon: favicon().
  index: index().
  _collect_existing_trace_ids: _collect_existing_trace_ids().
  _YELLOW: _YELLOW.
  _RESET: _RESET.
  _YellowWarningFormatter: _YellowWarningFormatter#
  _TARGETS_WITHOUT_USER_INTERACTION: _TARGETS_WITHOUT_USER_INTERACTION.
  RDAgentTask.log_trace_path: RDAgentTask#log_trace_path.
  RDAgentTask.scenario: RDAgentTask#scenario.
  RDAgentTask.trace_name: RDAgentTask#trace_name.
  RDAgentTask.ui_server_port: RDAgentTask#ui_server_port.
  RDAgentTask.__init__: RDAgentTask#__init__().
---
# Module: [`rdagent/log/server/app.py`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py)

## Classes
### `RDAgentTask`
- def: [`rdagent/log/server/app.py:52`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L52)
- signature: `class RDAgentTask:`
- members:
  - `get_end_code(self)` — [`L95`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L95)
  - `is_alive(self)` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L92)
  - `start(self)` — [`L88`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L88)
  - `stop(self)` — [`L100`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L100)
  - `kwargs` — [`L65`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L65)
  - `log_trace_path` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L67)
  - `messages` — [`L85`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L85)
  - `pointers` — [`L86`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L86)
  - `process` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L71)
  - `scenario` — [`L68`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L68)
  - `stdout_path` — [`L66`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L66)
  - `target_name` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L64)
  - `trace_name` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L69)
  - `ui_server_port` — [`L70`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L70)
  - `user_request_q` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L77)
  - `user_response_q` — [`L78`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L78)
- protocol/private: `__init__`[`L53`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L53), `_run`[`L116`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L116)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../__init__.md#rdagent_logger.rdagent_logger), [`main`](../../app/data_science/loop.md#main), [`extract_models_and_implement`](../../app/general_model/general_model.md#extract_models_and_implement), [`main`](../../app/qlib_rd_loop/factor.md#main), [`main`](../../app/qlib_rd_loop/model.md#main), [`main`](../../app/qlib_rd_loop/quant.md#main), [`LOG_SETTINGS`](../conf.md#LOG_SETTINGS), [`main`](../../app/qlib_rd_loop/factor_from_report.md#main), [`refresh_storages_from_settings`](../logger.md#RDAgentLog.refresh_storages_from_settings), [`set_storages_path`](../logger.md#RDAgentLog.set_storages_path), [`set_ui_server_port`](../conf.md#LogSettings.set_ui_server_port), [`rebind_console_to_current_streams`](../logger.md#RDAgentLog.rebind_console_to_current_streams), [`_TARGETS_WITHOUT_USER_INTERACTION`](app.md#_TARGETS_WITHOUT_USER_INTERACTION)
- used by: [`update_trace`](app.md#update_trace), [`read_trace`](app.md#read_trace), [`control_process`](app.md#control_process), [`rdagent_processes`](app.md#rdagent_processes.rdagent_processes), [`upload_file`](app.md#upload_file), [`_get_or_create_task`](app.md#_get_or_create_task), [`submit_user_interaction_response`](app.md#submit_user_interaction_response), [`test`](app.md#test), [`_drain_user_requests_into_messages`](app.md#_drain_user_requests_into_messages), [`_resolve_stdout_path`](app.md#_resolve_stdout_path), [`receive_msgs`](app.md#receive_msgs)

### `_YellowWarningFormatter`  ·  implements/extends Formatter
- def: [`rdagent/log/server/app.py:30`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L30)
- signature: `class _YellowWarningFormatter(logging.Formatter):`
- members:
  - `format(self, record: logging.LogRecord)` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L31)
- uses (calls/refs, reference-scoped): [`_RESET`](app.md#_RESET), [`_YELLOW`](app.md#_YELLOW)
- used by: [`_configure_app_logger`](app.md#_configure_app_logger)

## Functions
- `_collect_existing_trace_ids(trace_root: Path)` — [`L278`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L278) — Return trace ids that should be visible in the UI history panel.
- `_configure_app_logger()` — [`L37`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L37)
- `_drain_user_requests_into_messages(task: RDAgentTask)` — [`L175`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L175) — Move a single pending user-interaction request into `task.messages`.
- `_get_or_create_task(trace_id: str)` — [`L213`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L213)
- `_load_existing_traces(trace_root: Path)` — [`L298`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L298) — Load persisted traces into memory so the UI survives a server restart.
- `_normalize_static_request_path(fn: str)` — [`L206`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L206)
- `_resolve_stdout_path(trace_id: str)` — [`L230`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L230)
- `control_process()` — [`L532`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L532)
- `download_stdout_file()` — [`L360`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L360)
- `favicon()` — [`L202`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L202)
- `index()` — [`L580`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L580)
- `list_traces()` — [`L378`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L378) — Return trace ids that are available for history browsing.
- `main(port: int = 19899)` — [`L591`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L591)
- `read_trace(log_path: Path, id: str = "")` — [`L250`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L250)
- `receive_msgs()` — [`L489`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L489)
- `server_static_files(fn)` — [`L587`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L587)
- `submit_user_interaction_response()` — [`L509`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L509) — Frontend submits a user response; server forwards it to the rdagent subprocess via IPC queue.
- `test()` — [`L572`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L572)
- `update_trace()` — [`L311`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L311)
- `upload_file()` — [`L386`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L386)

## Module values
- `_RESET` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L27)
- `_TARGETS_WITHOUT_USER_INTERACTION` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L49)
- `_YELLOW` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L26)
- `app` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L22)
- `log_folder_path` — [`L172`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L172)
- `rdagent_processes` — [`L171`](../../../../../../../raw/code/rd-agent/rdagent/log/server/app.py#L171)

