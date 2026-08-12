---
title: 'Module: rlm/environments/modal_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/modal_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.modal_repl`/
symbols:
  ModalREPL._handle_llm_request: ModalREPL#_handle_llm_request().
  ModalREPL.setup: ModalREPL#setup().
  ModalREPL.execute_code: ModalREPL#execute_code().
  ModalREPL: ModalREPL#
  ModalREPL._calls_lock: ModalREPL#_calls_lock.
  ModalREPL.cleanup: ModalREPL#cleanup().
  ModalREPL._poll_broker: ModalREPL#_poll_broker().
  ModalREPL.pending_llm_calls: ModalREPL#pending_llm_calls.
  ModalREPL.sandbox: ModalREPL#sandbox.
  get_default_image: get_default_image().
  ModalREPL.poller_thread: ModalREPL#poller_thread.
  ModalREPL.BROKER_PORT: ModalREPL#BROKER_PORT.
  ModalREPL.broker_url: ModalREPL#broker_url.
  ModalREPL.image: ModalREPL#image.
  ModalREPL.load_context: ModalREPL#load_context().
  ModalREPL.lm_handler_address: ModalREPL#lm_handler_address.
  ModalREPL.poller_stop: ModalREPL#poller_stop.
  ModalREPL.__init__: ModalREPL#__init__().
  ModalREPL.__exit__: ModalREPL#__exit__().
  ModalREPL.__del__: ModalREPL#__del__().
  ModalREPL.app: ModalREPL#app.
  _BROKER_SCRIPT: _BROKER_SCRIPT.
  _build_exec_script: _build_exec_script().
  ModalREPL.app_name: ModalREPL#app_name.
  ModalREPL.timeout: ModalREPL#timeout.
  ModalREPL.broker_process: ModalREPL#broker_process.
  ModalREPL.__enter__: ModalREPL#__enter__().
---
# Module: [`rlm/environments/modal_repl.py`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py)

## Classes
### `ModalREPL`  ·  implements/extends IsolatedEnv
- def: [`rlm/environments/modal_repl.py:278`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L278) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Modal REPL environment that runs Python code in a Modal Sandbox.
- signature: `class ModalREPL(IsolatedEnv):`
- members:
  - `_handle_llm_request(self, req_data: dict)` — [`L396`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L396) — Handle an LLM request from the sandbox. — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
  - `_poll_broker(self)` — [`L364`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L364) — Poll the broker for pending LLM requests and handle them.
  - `cleanup(self)` — [`L492`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L492) — Terminate the sandbox and stop polling.
  - `execute_code(self, code: str)` — [`L446`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L446) — Execute code in the Modal sandbox and return result.
  - `load_context(self, context_payload: dict | list | str)` — [`L434`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L434) — Load context into the sandbox environment.
  - `setup(self)` — [`L331`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L331) — Create the Modal app, sandbox, broker, and start polling.
  - `BROKER_PORT` — [`L288`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L288)
  - `app` — [`L314`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L314)
  - `app_name` — [`L308`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L308)
  - `broker_process` — [`L316`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L316)
  - `broker_url` — [`L317`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L317)
  - `image` — [`L312`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L312)
  - `lm_handler_address` — [`L310`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L310)
  - `pending_llm_calls` — [`L320`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L320)
  - `poller_stop` — [`L319`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L319)
  - `poller_thread` — [`L318`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L318)
  - `sandbox` — [`L315`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L315)
  - `timeout` — [`L309`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L309)
- protocol/private: `__del__`[`L514`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L514), `__enter__`[`L507`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L507), `__exit__`[`L510`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L510), `__init__`[`L290`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L290), `_calls_lock`[`L321`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L321)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`depth`](base_env.md#BaseEnv.depth), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`depth`](../core/comms_utils.md#LMRequest.depth), [`__init__`](base_env.md#IsolatedEnv.__init__), [`get_default_image`](modal_repl.md#get_default_image), [`_BROKER_SCRIPT`](modal_repl.md#_BROKER_SCRIPT), [`_build_exec_script`](modal_repl.md#_build_exec_script)
- used by: [`get_environment`](__init__.md#get_environment), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`execute_code`](base_env.md#IsolatedEnv.execute_code), [`load_context`](base_env.md#IsolatedEnv.load_context), [`setup`](base_env.md#IsolatedEnv.setup)  (3 test-only)

## Functions
- `_build_exec_script(code: str, broker_port: int = 8080, depth: int = 1)` — [`L115`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L115) — Build a script that executes code with state persistence.
- `get_default_image()` — [`L20`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L20) — Build a default Modal image with common libraries for data science,

## Module values
- `_BROKER_SCRIPT` — [`L36`](../../../../../../raw/code/rlm/rlm/environments/modal_repl.py#L36)

