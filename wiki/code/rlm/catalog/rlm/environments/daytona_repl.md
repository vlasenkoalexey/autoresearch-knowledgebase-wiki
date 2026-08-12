---
title: 'Module: rlm/environments/daytona_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/daytona_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.daytona_repl`/
symbols:
  DaytonaREPL.setup: DaytonaREPL#setup().
  DaytonaREPL._handle_llm_request: DaytonaREPL#_handle_llm_request().
  DaytonaREPL.execute_code: DaytonaREPL#execute_code().
  DaytonaREPL._preview_token: DaytonaREPL#_preview_token.
  DaytonaREPL.sandbox: DaytonaREPL#sandbox.
  DaytonaREPL.cleanup: DaytonaREPL#cleanup().
  DaytonaREPL._calls_lock: DaytonaREPL#_calls_lock.
  DaytonaREPL._poll_broker: DaytonaREPL#_poll_broker().
  DaytonaREPL: DaytonaREPL#
  DaytonaREPL.pending_llm_calls: DaytonaREPL#pending_llm_calls.
  DaytonaREPL.broker_url: DaytonaREPL#broker_url.
  DaytonaREPL.custom_sub_tools: DaytonaREPL#custom_sub_tools.
  DaytonaREPL.poller_thread: DaytonaREPL#poller_thread.
  DaytonaREPL._get_headers: DaytonaREPL#_get_headers().
  _build_exec_script: _build_exec_script().
  DaytonaREPL.image: DaytonaREPL#image.
  DaytonaREPL.load_context: DaytonaREPL#load_context().
  DaytonaREPL.lm_handler_address: DaytonaREPL#lm_handler_address.
  DaytonaREPL.custom_tools: DaytonaREPL#custom_tools.
  DaytonaREPL.broker_session_id: DaytonaREPL#broker_session_id.
  DaytonaREPL.poller_stop: DaytonaREPL#poller_stop.
  DaytonaREPL.__init__: DaytonaREPL#__init__().
  DaytonaREPL.__exit__: DaytonaREPL#__exit__().
  DaytonaREPL.__del__: DaytonaREPL#__del__().
  DaytonaREPL.BROKER_PORT: DaytonaREPL#BROKER_PORT.
  DaytonaREPL.api_key: DaytonaREPL#api_key.
  DaytonaREPL.daytona: DaytonaREPL#daytona.
  get_default_image: get_default_image().
  _BROKER_SCRIPT: _BROKER_SCRIPT.
  DaytonaREPL.target: DaytonaREPL#target.
  DaytonaREPL.name: DaytonaREPL#name.
  DaytonaREPL.timeout: DaytonaREPL#timeout.
  DaytonaREPL.cpu: DaytonaREPL#cpu.
  DaytonaREPL.memory: DaytonaREPL#memory.
  DaytonaREPL.disk: DaytonaREPL#disk.
  DaytonaREPL.auto_stop_interval: DaytonaREPL#auto_stop_interval.
  DaytonaREPL.__enter__: DaytonaREPL#__enter__().
---
# Module: [`rlm/environments/daytona_repl.py`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py)

## Classes
### `DaytonaREPL`  ·  implements/extends IsolatedEnv
- def: [`rlm/environments/daytona_repl.py:366`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L366) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Daytona REPL environment that runs Python code in a Daytona Sandbox.
- signature: `class DaytonaREPL(IsolatedEnv):`
- members:
  - `__init__(self, api_key: str | None = None, target: str = "us", name: str = "rlm-sandbox", timeout: int = 600, cpu: int = 1, memory: int = 2, disk: int = 5, auto_stop_interval: int = 0, image: Image | None = None, lm_handler_address: tuple[str, int] | None = None, context_payload: dict | list | str | None = None, setup_code: str | None = None, persistent: bool = False, depth: int = 1, custom_tools: dict[str, Any] | None = None, custom_sub_tools: dict[str, Any] | None = None, **kwargs)` — [`L378`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L378) — Initialize a Daytona REPL environment.
  - `_get_headers(self)` — [`L527`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L527) — Get headers for broker requests including auth token.
  - `_handle_llm_request(self, req_data: dict)` — [`L568`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L568) — Handle an LLM request from the sandbox. — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
  - `_poll_broker(self)` — [`L534`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L534) — Poll the broker for pending LLM requests and handle them.
  - `cleanup(self)` — [`L675`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L675) — Terminate the sandbox and stop polling.
  - `execute_code(self, code: str)` — [`L618`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L618) — Execute code in the Daytona sandbox and return result.
  - `load_context(self, context_payload: dict | list | str)` — [`L606`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L606) — Load context into the sandbox environment.
  - `setup(self)` — [`L465`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L465) — Create the Daytona sandbox, broker, and start polling.
  - `BROKER_PORT` — [`L376`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L376)
  - `api_key` — [`L428`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L428)
  - `auto_stop_interval` — [`L435`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L435)
  - `broker_session_id` — [`L450`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L450)
  - `broker_url` — [`L451`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L451)
  - `cpu` — [`L432`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L432)
  - `custom_sub_tools` — [`L441`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L441)
  - `custom_tools` — [`L440`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L440)
  - `daytona` — [`L448`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L448)
  - `disk` — [`L434`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L434)
  - `image` — [`L436`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L436)
  - `lm_handler_address` — [`L437`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L437)
  - `memory` — [`L433`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L433)
  - `name` — [`L430`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L430)
  - `pending_llm_calls` — [`L454`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L454)
  - `poller_stop` — [`L453`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L453)
  - `poller_thread` — [`L452`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L452)
  - `sandbox` — [`L449`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L449)
  - `target` — [`L429`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L429)
  - `timeout` — [`L431`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L431)
- protocol/private: `__del__`[`L704`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L704), `__enter__`[`L697`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L697), `__exit__`[`L700`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L700), `_calls_lock`[`L455`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L455), `_preview_token`[`L516`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L516)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`validate_custom_tools`](base_env.md#validate_custom_tools), [`depth`](base_env.md#BaseEnv.depth), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`depth`](../core/comms_utils.md#LMRequest.depth), [`__init__`](base_env.md#IsolatedEnv.__init__), [`_build_exec_script`](daytona_repl.md#_build_exec_script), [`_BROKER_SCRIPT`](daytona_repl.md#_BROKER_SCRIPT), [`get_default_image`](daytona_repl.md#get_default_image)
- used by: [`get_environment`](__init__.md#get_environment), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`execute_code`](base_env.md#IsolatedEnv.execute_code), [`load_context`](base_env.md#IsolatedEnv.load_context), [`setup`](base_env.md#IsolatedEnv.setup)  (1 test-only)

## Functions
- `_build_exec_script(code: str, broker_port: int = 8080, depth: int = 1, custom_tools: dict[str, Any] | None = None)` — [`L156`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L156) — Build a script that executes code with state persistence. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `get_default_image()` — [`L34`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L34) — Build a default Daytona image with common libraries for data science,

## Module values
- `_BROKER_SCRIPT` — [`L77`](../../../../../../raw/code/rlm/rlm/environments/daytona_repl.py#L77)

