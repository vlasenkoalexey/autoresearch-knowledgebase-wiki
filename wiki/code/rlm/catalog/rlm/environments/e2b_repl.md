---
title: 'Module: rlm/environments/e2b_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/e2b_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.e2b_repl`/
symbols:
  E2BREPL.setup: E2BREPL#setup().
  E2BREPL._handle_llm_request: E2BREPL#_handle_llm_request().
  E2BREPL.execute_code: E2BREPL#execute_code().
  E2BREPL.sandbox: E2BREPL#sandbox.
  E2BREPL._calls_lock: E2BREPL#_calls_lock.
  E2BREPL.cleanup: E2BREPL#cleanup().
  E2BREPL._poll_broker: E2BREPL#_poll_broker().
  E2BREPL.pending_llm_calls: E2BREPL#pending_llm_calls.
  E2BREPL._wait_for_broker: E2BREPL#_wait_for_broker().
  E2BREPL.poller_thread: E2BREPL#poller_thread.
  E2BREPL: E2BREPL#
  E2BREPL.broker_url: E2BREPL#broker_url.
  E2BREPL.load_context: E2BREPL#load_context().
  E2BREPL.BROKER_PORT: E2BREPL#BROKER_PORT.
  E2BREPL.lm_handler_address: E2BREPL#lm_handler_address.
  E2BREPL.poller_stop: E2BREPL#poller_stop.
  E2BREPL.__init__: E2BREPL#__init__().
  E2BREPL.__exit__: E2BREPL#__exit__().
  E2BREPL.__del__: E2BREPL#__del__().
  _BROKER_SCRIPT: _BROKER_SCRIPT.
  _build_exec_script: _build_exec_script().
  E2BREPL.timeout: E2BREPL#timeout.
  E2BREPL.sandbox_id: E2BREPL#sandbox_id.
  E2BREPL.broker_process: E2BREPL#broker_process.
  E2BREPL.__enter__: E2BREPL#__enter__().
---
# Module: [`rlm/environments/e2b_repl.py`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py)

## Classes
### `E2BREPL`  ·  implements/extends IsolatedEnv
- def: [`rlm/environments/e2b_repl.py:261`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L261) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: E2B REPL environment that runs Python code in E2B sandboxes.
- signature: `class E2BREPL(IsolatedEnv):`
- members:
  - `_handle_llm_request(self, req_data: dict)` — [`L393`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L393) — Handle an LLM request from the sandbox.
  - `_poll_broker(self)` — [`L361`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L361) — Poll the broker for pending LLM requests and handle them.
  - `_wait_for_broker(self, max_attempts: int = 30)` — [`L342`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L342) — Wait for the broker to be ready by checking health endpoint.
  - `cleanup(self)` — [`L488`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L488) — Terminate the sandbox and stop polling.
  - `execute_code(self, code: str)` — [`L441`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L441) — Execute code in the E2B sandbox and return result.
  - `load_context(self, context_payload: dict | list | str)` — [`L429`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L429) — Load context into the sandbox environment.
  - `setup(self)` — [`L311`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L311) — Create the E2B sandbox, broker, and start polling.
  - `BROKER_PORT` — [`L271`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L271)
  - `broker_process` — [`L295`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L295)
  - `broker_url` — [`L294`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L294)
  - `lm_handler_address` — [`L289`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L289)
  - `pending_llm_calls` — [`L300`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L300)
  - `poller_stop` — [`L299`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L299)
  - `poller_thread` — [`L298`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L298)
  - `sandbox` — [`L292`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L292)
  - `sandbox_id` — [`L293`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L293)
  - `timeout` — [`L288`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L288)
- protocol/private: `__del__`[`L511`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L511), `__enter__`[`L504`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L504), `__exit__`[`L507`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L507), `__init__`[`L273`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L273), `_calls_lock`[`L301`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L301)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`__init__`](base_env.md#IsolatedEnv.__init__), [`_BROKER_SCRIPT`](e2b_repl.md#_BROKER_SCRIPT), [`_build_exec_script`](e2b_repl.md#_build_exec_script)
- used by: [`get_environment`](__init__.md#get_environment), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`execute_code`](base_env.md#IsolatedEnv.execute_code), [`load_context`](base_env.md#IsolatedEnv.load_context), [`setup`](base_env.md#IsolatedEnv.setup)

## Functions
- `_build_exec_script(code: str, broker_port: int = 8888)` — [`L105`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L105) — Build a script that executes code with state persistence.

## Module values
- `_BROKER_SCRIPT` — [`L26`](../../../../../../raw/code/rlm/rlm/environments/e2b_repl.py#L26)

