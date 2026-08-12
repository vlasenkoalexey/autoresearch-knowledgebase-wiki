---
title: 'Module: rlm/environments/docker_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/docker_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.docker_repl`/
symbols:
  DockerREPL.execute_code: DockerREPL#execute_code().
  DockerREPL.setup: DockerREPL#setup().
  LLMProxyHandler._handle_single: LLMProxyHandler#_handle_single().
  LLMProxyHandler._handle_batched: LLMProxyHandler#_handle_batched().
  DockerREPL: DockerREPL#
  DockerREPL.cleanup: DockerREPL#cleanup().
  LLMProxyHandler._handle_rlm_batched: LLMProxyHandler#_handle_rlm_batched().
  DockerREPL._calls_lock: DockerREPL#_calls_lock.
  LLMProxyHandler._handle_rlm_single: LLMProxyHandler#_handle_rlm_single().
  LLMProxyHandler.do_POST: LLMProxyHandler#do_POST().
  DockerREPL.container_id: DockerREPL#container_id.
  DockerREPL.proxy_server: DockerREPL#proxy_server.
  DockerREPL.add_history: DockerREPL#add_history().
  DockerREPL.temp_dir: DockerREPL#temp_dir.
  DockerREPL.update_handler_address: DockerREPL#update_handler_address().
  DockerREPL.add_context: DockerREPL#add_context().
  DockerREPL.append_compaction_entry: DockerREPL#append_compaction_entry().
  LLMProxyHandler._run: LLMProxyHandler#_run().
  DockerREPL._inject_history: DockerREPL#_inject_history().
  LLMProxyHandler.pending_calls: LLMProxyHandler#pending_calls.
  LLMProxyHandler.subcall_fn: LLMProxyHandler#subcall_fn.
  DockerREPL.pending_calls: DockerREPL#pending_calls.
  DockerREPL.__init__: DockerREPL#__init__().
  DockerREPL.custom_sub_tools: DockerREPL#custom_sub_tools.
  LLMProxyHandler._resolve_address: LLMProxyHandler#_resolve_address().
  LLMProxyHandler.lock: LLMProxyHandler#lock.
  LLMProxyHandler._respond: LLMProxyHandler#_respond().
  DockerREPL.lm_handler_address: DockerREPL#lm_handler_address.
  DockerREPL.compaction: DockerREPL#compaction.
  DockerREPL.proxy_thread: DockerREPL#proxy_thread.
  DockerREPL.proxy_port: DockerREPL#proxy_port.
  DockerREPL._context_count: DockerREPL#_context_count.
  DockerREPL._history_count: DockerREPL#_history_count.
  _build_custom_tools_code: _build_custom_tools_code().
  _build_exec_script: _build_exec_script().
  DockerREPL.load_context: DockerREPL#load_context().
  DockerREPL._compaction_history: DockerREPL#_compaction_history.
  DockerREPL.custom_tools: DockerREPL#custom_tools.
  DockerREPL.get_context_count: DockerREPL#get_context_count().
  DockerREPL.get_history_count: DockerREPL#get_history_count().
  DockerREPL.__exit__: DockerREPL#__exit__().
  DockerREPL.__del__: DockerREPL#__del__().
  LLMProxyHandler.depth: LLMProxyHandler#depth.
  DockerREPL.subcall_fn: DockerREPL#subcall_fn.
  LLMProxyHandler: LLMProxyHandler#
  LLMProxyHandler.lm_handler_address: LLMProxyHandler#lm_handler_address.
  LLMProxyHandler.max_concurrent_subcalls: LLMProxyHandler#max_concurrent_subcalls.
  DockerREPL.image: DockerREPL#image.
  DockerREPL._cleaned_up: DockerREPL#_cleaned_up.
  LLMProxyHandler.log_message: LLMProxyHandler#log_message().
  DockerREPL.__enter__: DockerREPL#__enter__().
---
# Module: [`rlm/environments/docker_repl.py`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py)

## Classes
### `DockerREPL`  ·  implements/extends NonIsolatedEnv
- def: [`rlm/environments/docker_repl.py:408`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L408) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Docker REPL - runs Python in a Docker container with LLM and recursive RLM support.
- signature: `class DockerREPL(NonIsolatedEnv):`
- members:
  - `_inject_history(self, history: list[Any])` — [`L660`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L660) — Refresh the container's ``history`` variable from a host-side list.
  - `add_context(self, context_payload: dict | list | str, context_index: int | None = None)` — [`L588`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L588) — Add a context as ``context_N`` (auto-incrementing unless given).
  - `add_history(self, message_history: list[dict[str, Any]], history_index: int | None = None)` — [`L625`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L625) — Store a conversation's message history as ``history_N`` in the REPL.
  - `append_compaction_entry(self, entry: list[dict[str, Any]] | dict[str, Any])` — [`L669`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L669) — Append a trajectory segment or summary to the compaction history.
  - `cleanup(self)` — [`L730`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L730) — Tear down the container, proxy server, and workspace. Idempotent.
  - `execute_code(self, code: str)` — [`L680`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L680) — documented in [rlm-environments-docker_repl](../../../concepts/rlm-environments-docker_repl.md)
  - `get_context_count(self)` — [`L621`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L621) — Return the number of contexts loaded.
  - `get_history_count(self)` — [`L653`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L653) — Return the number of conversation histories stored.
  - `load_context(self, context_payload: dict | list | str)` — [`L566`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L566) — Load context as ``context_0`` (with ``context`` aliased to it).
  - `setup(self)` — [`L492`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L492) — Start the proxy server and Docker container. — documented in [rlm-environments-docker_repl](../../../concepts/rlm-environments-docker_repl.md)
  - `update_handler_address(self, address: tuple[str, int])` — [`L573`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L573) — Point the proxy at a new LM handler (each completion() spawns one).
  - `compaction` — [`L450`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L450)
  - `container_id` — [`L451`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L451)
  - `custom_sub_tools` — [`L467`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L467)
  - `custom_tools` — [`L465`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L465)
  - `image` — [`L447`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L447)
  - `lm_handler_address` — [`L448`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L448)
  - `pending_calls` — [`L477`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L477)
  - `proxy_port` — [`L454`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L454)
  - `proxy_server` — [`L452`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L452)
  - `proxy_thread` — [`L453`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L453)
  - `subcall_fn` — [`L449`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L449)
  - `temp_dir` — [`L476`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L476)
- protocol/private: `__del__`[`L772`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L772), `__enter__`[`L765`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L765), `__exit__`[`L768`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L768), `__init__`[`L425`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L425), `_calls_lock`[`L478`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L478), `_cleaned_up`[`L455`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L455), `_compaction_history`[`L462`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L462), `_context_count`[`L458`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L458), `_history_count`[`L459`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L459)
- uses (calls/refs, reference-scoped): [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`validate_custom_tools`](base_env.md#validate_custom_tools), [`depth`](base_env.md#BaseEnv.depth), [`max_concurrent_subcalls`](base_env.md#BaseEnv.max_concurrent_subcalls), [`__init__`](base_env.md#NonIsolatedEnv.__init__), [`_build_exec_script`](docker_repl.md#_build_exec_script), [`LLMProxyHandler`](docker_repl.md#LLMProxyHandler)
- used by: [`get_environment`](__init__.md#get_environment), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`execute_code`](base_env.md#NonIsolatedEnv.execute_code), [`load_context`](base_env.md#NonIsolatedEnv.load_context), [`setup`](base_env.md#NonIsolatedEnv.setup)  (48 test-only)

### `LLMProxyHandler`  ·  implements/extends BaseHTTPRequestHandler
- def: [`rlm/environments/docker_repl.py:44`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L44)
- doc: HTTP handler for LLM/RLM requests from the container.
- signature: `class LLMProxyHandler(BaseHTTPRequestHandler):`
- members:
  - `_resolve_address(self)` — [`L64`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L64) — Read the LM handler address dynamically.
  - `do_POST(self)` — [`L74`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L74)
  - `log_message(self, *args)` — [`L61`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L61)
  - `depth` — [`L55`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L55)
  - `lm_handler_address` — [`L52`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L52)
  - `lock` — [`L54`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L54)
  - `max_concurrent_subcalls` — [`L59`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L59)
  - `pending_calls` — [`L53`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L53)
  - `subcall_fn` — [`L58`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L58)
- protocol/private: `_handle_batched`[`L133`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L133), `_handle_rlm_batched`[`L175`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L175), `_handle_rlm_single`[`L157`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L157), `_handle_single`[`L117`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L117), `_respond`[`L102`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L102), `_run`[`L190`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L190)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`depth`](../core/comms_utils.md#LMRequest.depth)
- used by: [`setup`](docker_repl.md#DockerREPL.setup)

## Functions
- `_build_custom_tools_code(custom_tools: dict[str, Any] | None)` — [`L217`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L217) — Build the in-container injection code for custom tools. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `_build_exec_script(code: str, proxy_port: int, depth: int = 1, custom_tools: dict[str, Any] | None = None, compaction: bool = False)` — [`L258`](../../../../../../raw/code/rlm/rlm/environments/docker_repl.py#L258) — Build the per-cell execution script that runs inside the container.

