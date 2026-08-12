---
title: 'Module: utils/error_handler.py'
type: catalog
provenance: extracted
module: utils/error_handler.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.error_handler`/
symbols:
  ErrorHandler.handle_error: ErrorHandler#handle_error().
  ServerRestartHandler.restart_server: ServerRestartHandler#restart_server().
  ErrorHandler.consecutive_errors: ErrorHandler#consecutive_errors.
  ErrorHandler.attempt_recovery: ErrorHandler#attempt_recovery().
  get_error_handler: get_error_handler().
  ErrorHandler.get_error_stats: ErrorHandler#get_error_stats().
  ServerRestartHandler.set_server_process: ServerRestartHandler#set_server_process().
  ServerRestartHandler.check_and_restart: ServerRestartHandler#check_and_restart().
  ErrorHandler._signal_handler: ErrorHandler#_signal_handler().
  ServerRestartHandler.server_process: ServerRestartHandler#server_process.
  ErrorHandler.reset_error_counter: ErrorHandler#reset_error_counter().
  handle_agent_error: handle_agent_error().
  reset_error_counter: reset_error_counter().
  install_shutdown_handler: install_shutdown_handler().
  ErrorHandler.on_recovery: ErrorHandler#on_recovery.
  ServerRestartHandler.failure_count: ServerRestartHandler#failure_count.
  _error_handler: _error_handler.
  ErrorHandler._install_signal_handlers: ErrorHandler#_install_signal_handlers().
  ErrorHandler.max_consecutive_errors: ErrorHandler#max_consecutive_errors.
  ErrorHandler.on_shutdown: ErrorHandler#on_shutdown.
  ServerRestartHandler.server_cmd: ServerRestartHandler#server_cmd.
  ErrorHandler.track_success: ErrorHandler#track_success().
  ErrorHandler.is_shutdown_requested: ErrorHandler#is_shutdown_requested().
  ServerRestartHandler.reset_failure_count: ServerRestartHandler#reset_failure_count().
  ErrorHandler: ErrorHandler#
  ErrorHandler.recovery_delay: ErrorHandler#recovery_delay.
  ErrorHandler.total_errors: ErrorHandler#total_errors.
  ErrorHandler.shutdown_requested: ErrorHandler#shutdown_requested.
  ServerRestartHandler.server_env: ServerRestartHandler#server_env.
  ServerRestartHandler.restart_threshold: ServerRestartHandler#restart_threshold.
  ErrorHandler.__init__: ErrorHandler#__init__().
  ServerRestartHandler: ServerRestartHandler#
  ServerRestartHandler.__init__: ServerRestartHandler#__init__().
---
# Module: [`utils/error_handler.py`](../../../../../raw/code/continual-harness/utils/error_handler.py)

## Classes
### `ErrorHandler`
- def: [`utils/error_handler.py:15`](../../../../../raw/code/continual-harness/utils/error_handler.py#L15)
- doc: Manages error recovery and graceful shutdowns
- signature: `class ErrorHandler:`
- members:
  - `__init__(self, max_consecutive_errors=3, recovery_delay=2)` — [`L18`](../../../../../raw/code/continual-harness/utils/error_handler.py#L18) — Initialize error handler.
  - `_install_signal_handlers(self)` — [`L39`](../../../../../raw/code/continual-harness/utils/error_handler.py#L39) — Install signal handlers for graceful shutdown
  - `_signal_handler(self, signum, frame)` — [`L44`](../../../../../raw/code/continual-harness/utils/error_handler.py#L44) — Handle shutdown signals
  - `attempt_recovery(self)` — [`L87`](../../../../../raw/code/continual-harness/utils/error_handler.py#L87) — Attempt to recover from errors.
  - `get_error_stats(self)` — [`L129`](../../../../../raw/code/continual-harness/utils/error_handler.py#L129) — Get error statistics
  - `handle_error(self, error: Exception, context: str = "")` — [`L59`](../../../../../raw/code/continual-harness/utils/error_handler.py#L59) — Handle an error with potential recovery.
  - `is_shutdown_requested(self)` — [`L125`](../../../../../raw/code/continual-harness/utils/error_handler.py#L125) — Check if shutdown has been requested
  - `reset_error_counter(self)` — [`L114`](../../../../../raw/code/continual-harness/utils/error_handler.py#L114) — Reset the consecutive error counter
  - `track_success(self)` — [`L120`](../../../../../raw/code/continual-harness/utils/error_handler.py#L120) — Track a successful operation to reset error counter
  - `consecutive_errors` — [`L26`](../../../../../raw/code/continual-harness/utils/error_handler.py#L26)
  - `max_consecutive_errors` — [`L27`](../../../../../raw/code/continual-harness/utils/error_handler.py#L27)
  - `on_recovery` — [`L34`](../../../../../raw/code/continual-harness/utils/error_handler.py#L34)
  - `on_shutdown` — [`L33`](../../../../../raw/code/continual-harness/utils/error_handler.py#L33)
  - `recovery_delay` — [`L28`](../../../../../raw/code/continual-harness/utils/error_handler.py#L28)
  - `shutdown_requested` — [`L30`](../../../../../raw/code/continual-harness/utils/error_handler.py#L30)
  - `total_errors` — [`L29`](../../../../../raw/code/continual-harness/utils/error_handler.py#L29)
- used by: [`get_error_handler`](error_handler.md#get_error_handler), [`handle_agent_error`](error_handler.md#handle_agent_error), [`install_shutdown_handler`](error_handler.md#install_shutdown_handler), [`reset_error_counter`](error_handler.md#reset_error_counter)

### `ServerRestartHandler`
- def: [`utils/error_handler.py:138`](../../../../../raw/code/continual-harness/utils/error_handler.py#L138)
- doc: Handles server process restart on failures
- signature: `class ServerRestartHandler:`
- members:
  - `__init__(self, restart_threshold=5)` — [`L141`](../../../../../raw/code/continual-harness/utils/error_handler.py#L141) — Initialize server restart handler.
  - `check_and_restart(self)` — [`L167`](../../../../../raw/code/continual-harness/utils/error_handler.py#L167) — Check if restart is needed and perform it.
  - `reset_failure_count(self)` — [`L228`](../../../../../raw/code/continual-harness/utils/error_handler.py#L228) — Reset the failure counter
  - `restart_server(self)` — [`L181`](../../../../../raw/code/continual-harness/utils/error_handler.py#L181) — Restart the server process.
  - `set_server_process(self, process: subprocess.Popen, cmd: list, env: dict = None)` — [`L154`](../../../../../raw/code/continual-harness/utils/error_handler.py#L154) — Set the server process to manage.
  - `failure_count` — [`L149`](../../../../../raw/code/continual-harness/utils/error_handler.py#L149)
  - `restart_threshold` — [`L148`](../../../../../raw/code/continual-harness/utils/error_handler.py#L148)
  - `server_cmd` — [`L151`](../../../../../raw/code/continual-harness/utils/error_handler.py#L151)
  - `server_env` — [`L152`](../../../../../raw/code/continual-harness/utils/error_handler.py#L152)
  - `server_process` — [`L150`](../../../../../raw/code/continual-harness/utils/error_handler.py#L150)

## Functions
- `get_error_handler()` — [`L237`](../../../../../raw/code/continual-harness/utils/error_handler.py#L237) — Get or create the global error handler
- `handle_agent_error(error: Exception, context: str = "")` — [`L245`](../../../../../raw/code/continual-harness/utils/error_handler.py#L245) — Handle an agent error using the global error handler.
- `install_shutdown_handler(callback: Optional[Callable] = None)` — [`L266`](../../../../../raw/code/continual-harness/utils/error_handler.py#L266) — Install a shutdown handler.
- `reset_error_counter()` — [`L260`](../../../../../raw/code/continual-harness/utils/error_handler.py#L260) — Reset the global error counter

## Module values
- `_error_handler` — [`L234`](../../../../../raw/code/continual-harness/utils/error_handler.py#L234)

