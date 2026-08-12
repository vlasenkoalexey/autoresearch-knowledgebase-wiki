---
title: 'Module: rlm/environments/prime_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/prime_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.prime_repl`/
symbols:
  PrimeREPL.setup: PrimeREPL#setup().
  PrimeREPL._handle_llm_request: PrimeREPL#_handle_llm_request().
  PrimeREPL.execute_code: PrimeREPL#execute_code().
  PrimeREPL.sandbox_id: PrimeREPL#sandbox_id.
  PrimeREPL.client: PrimeREPL#client.
  PrimeREPL.cleanup: PrimeREPL#cleanup().
  PrimeREPL._calls_lock: PrimeREPL#_calls_lock.
  PrimeREPL._wait_for_broker: PrimeREPL#_wait_for_broker().
  PrimeREPL: PrimeREPL#
  PrimeREPL._poll_broker: PrimeREPL#_poll_broker().
  PrimeREPL.pending_llm_calls: PrimeREPL#pending_llm_calls.
  PrimeREPL.broker_url: PrimeREPL#broker_url.
  PrimeREPL.poller_thread: PrimeREPL#poller_thread.
  PrimeREPL.BROKER_PORT: PrimeREPL#BROKER_PORT.
  PrimeREPL.broker_job: PrimeREPL#broker_job.
  PrimeREPL.load_context: PrimeREPL#load_context().
  PrimeREPL.lm_handler_address: PrimeREPL#lm_handler_address.
  PrimeREPL.broker_exposure_id: PrimeREPL#broker_exposure_id.
  PrimeREPL.poller_stop: PrimeREPL#poller_stop.
  PrimeREPL.__init__: PrimeREPL#__init__().
  PrimeREPL.__exit__: PrimeREPL#__exit__().
  PrimeREPL.__del__: PrimeREPL#__del__().
  PrimeREPL.timeout_minutes: PrimeREPL#timeout_minutes.
  _BROKER_SCRIPT: _BROKER_SCRIPT.
  _build_exec_script: _build_exec_script().
  PrimeREPL.name: PrimeREPL#name.
  PrimeREPL.docker_image: PrimeREPL#docker_image.
  PrimeREPL.network_access: PrimeREPL#network_access.
  PrimeREPL.__enter__: PrimeREPL#__enter__().
---
# Module: [`rlm/environments/prime_repl.py`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py)

## Classes
### `PrimeREPL`  ·  implements/extends IsolatedEnv
- def: [`rlm/environments/prime_repl.py:277`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L277) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Prime Intellect REPL environment that runs Python code in Prime Sandboxes.
- signature: `class PrimeREPL(IsolatedEnv):`
- members:
  - `_handle_llm_request(self, req_data: dict)` — [`L463`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L463) — Handle an LLM request from the sandbox. — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
  - `_poll_broker(self)` — [`L431`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L431) — Poll the broker for pending LLM requests and handle them.
  - `_wait_for_broker(self, max_attempts: int = 30)` — [`L393`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L393) — Wait for the broker to be ready by checking health endpoint.
  - `cleanup(self)` — [`L566`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L566) — Terminate the sandbox and stop polling.
  - `execute_code(self, code: str)` — [`L513`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L513) — Execute code in the Prime sandbox and return result.
  - `load_context(self, context_payload: dict | list | str)` — [`L501`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L501) — Load context into the sandbox environment.
  - `setup(self)` — [`L336`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L336) — Create the Prime sandbox, broker, and start polling.
  - `BROKER_PORT` — [`L287`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L287)
  - `broker_exposure_id` — [`L320`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L320)
  - `broker_job` — [`L318`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L318)
  - `broker_url` — [`L319`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L319)
  - `client` — [`L316`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L316)
  - `docker_image` — [`L310`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L310)
  - `lm_handler_address` — [`L312`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L312)
  - `name` — [`L309`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L309)
  - `network_access` — [`L313`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L313)
  - `pending_llm_calls` — [`L325`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L325)
  - `poller_stop` — [`L324`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L324)
  - `poller_thread` — [`L323`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L323)
  - `sandbox_id` — [`L317`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L317)
  - `timeout_minutes` — [`L311`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L311)
- protocol/private: `__del__`[`L600`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L600), `__enter__`[`L593`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L593), `__exit__`[`L596`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L596), `__init__`[`L289`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L289), `_calls_lock`[`L326`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L326)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`depth`](base_env.md#BaseEnv.depth), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`depth`](../core/comms_utils.md#LMRequest.depth), [`__init__`](base_env.md#IsolatedEnv.__init__), [`APT_PACKAGES`](constants.md#APT_PACKAGES), [`PIP_PACKAGES`](constants.md#PIP_PACKAGES), [`_BROKER_SCRIPT`](prime_repl.md#_BROKER_SCRIPT), [`_build_exec_script`](prime_repl.md#_build_exec_script)
- used by: [`get_environment`](__init__.md#get_environment), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`execute_code`](base_env.md#IsolatedEnv.execute_code), [`load_context`](base_env.md#IsolatedEnv.load_context), [`setup`](base_env.md#IsolatedEnv.setup)  (3 test-only)

## Functions
- `_build_exec_script(code: str, broker_port: int = 8888, depth: int = 1)` — [`L114`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L114) — Build a script that executes code with state persistence.

## Module values
- `_BROKER_SCRIPT` — [`L35`](../../../../../../raw/code/rlm/rlm/environments/prime_repl.py#L35)

