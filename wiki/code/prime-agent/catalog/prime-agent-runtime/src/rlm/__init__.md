---
title: 'Module: prime-agent-runtime/src/rlm/__init__.py'
type: catalog
provenance: extracted
module: prime-agent-runtime/src/rlm/__init__.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `prime-agent-runtime.src.rlm`/
symbols:
  _subagent_from_payload: _subagent_from_payload().
  host_request: host_request().
  _HarnessProxy._resolve: _HarnessProxy#_resolve().
  _spawn_handle_from_payload: _spawn_handle_from_payload().
  _model_from_payload: _model_from_payload().
  delete_subagent: delete_subagent().
  run: run().
  _HarnessProxy._degraded: _HarnessProxy#_degraded().
  RLMSubagent: RLMSubagent#
  host_request._on_msg: host_request()._on_msg().
  find_models: find_models().
  list_subagents: list_subagents().
  _HarnessProxy: _HarnessProxy#
  RLMSpawnHandle: RLMSpawnHandle#
  _HarnessProxy._fallback: _HarnessProxy#_fallback.
  _HarnessProxy._unpersisted: _HarnessProxy#_unpersisted.
  _RLMCallable.run: _RLMCallable#run().
  _RLMCallable.find_models: _RLMCallable#find_models().
  _RLMCallable.list_subagents: _RLMCallable#list_subagents().
  _RLMCallable.delete_subagent: _RLMCallable#delete_subagent().
  _RLMCallable.__call__: _RLMCallable#__call__().
  rlm: rlm.
  _CallableModule.__call__: _CallableModule#__call__().
  _harness_state: _harness_state.
  RLMModel: RLMModel#
  _HarnessProxy.__getattr__: _HarnessProxy#__getattr__().
  _HarnessProxy.__repr__: _HarnessProxy#__repr__().
  _RLMCallable.harness: _RLMCallable#harness.
  _RLMCallable.get_harness_state: _RLMCallable#get_harness_state.
  __getattr__: __getattr__().
  RLMSubagent.rlm_child_id: RLMSubagent#rlm_child_id.
  HOST_COMM_TARGET: HOST_COMM_TARGET.
  RLMSpawnHandle.rlm_child_id: RLMSpawnHandle#rlm_child_id.
  RLMSpawnHandle.name: RLMSpawnHandle#name.
  RLMSpawnHandle.session_dir: RLMSpawnHandle#session_dir.
  RLMSpawnHandle.model: RLMSpawnHandle#model.
  RLMModel.provider: RLMModel#provider.
  RLMModel.id: RLMModel#id.
  RLMModel.name: RLMModel#name.
  RLMModel.selector: RLMModel#selector.
  RLMSubagent.active_session_id: RLMSubagent#active_session_id.
  RLMSubagent.session_id: RLMSubagent#session_id.
  RLMSubagent.session_name: RLMSubagent#session_name.
  RLMSubagent.session_dir: RLMSubagent#session_dir.
  RLMSubagent.status: RLMSubagent#status.
  _install_control_comm_handlers: _install_control_comm_handlers().
  host_request._on_msg._resolve_result: host_request()._on_msg()._resolve_result().
  host_request._on_msg._resolve_error: host_request()._on_msg()._resolve_error().
  host_request._on_msg._resolve_unexpected: host_request()._on_msg()._resolve_unexpected().
  _RLMCallable: _RLMCallable#
  _CallableModule: _CallableModule#
  _LAZY_MCP: _LAZY_MCP.
  __all__: __all__.
---
# Module: [`prime-agent-runtime/src/rlm/__init__.py`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py)

## Classes
### `RLMModel`
- def: [`prime-agent-runtime/src/rlm/__init__.py:36`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L36)
- signature: `class RLMModel:`
- members:
  - `id` — [`L38`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L38)
  - `name` — [`L39`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L39)
  - `provider` — [`L37`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L37)
  - `selector` — [`L40`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L40)
- used by: [`_model_from_payload`](__init__.md#_model_from_payload), [`find_models`](__init__.md#find_models), [`find_models`](__init__.md#_RLMCallable.find_models)

### `RLMSpawnHandle`
- def: [`prime-agent-runtime/src/rlm/__init__.py:28`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L28)
- signature: `class RLMSpawnHandle:`
- members:
  - `model` — [`L32`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L32)
  - `name` — [`L30`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L30)
  - `rlm_child_id` — [`L29`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L29)
  - `session_dir` — [`L31`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L31)
- used by: [`_spawn_handle_from_payload`](__init__.md#_spawn_handle_from_payload), [`run`](__init__.md#run), [`__call__`](__init__.md#_CallableModule.__call__), [`__call__`](__init__.md#_RLMCallable.__call__), [`run`](__init__.md#_RLMCallable.run)

### `RLMSubagent`
- def: [`prime-agent-runtime/src/rlm/__init__.py:44`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L44)
- signature: `class RLMSubagent:`
- members:
  - `active_session_id` — [`L46`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L46)
  - `rlm_child_id` — [`L45`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L45)
  - `session_dir` — [`L49`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L49)
  - `session_id` — [`L47`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L47)
  - `session_name` — [`L48`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L48)
  - `status` — [`L50`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L50)
- used by: [`_subagent_from_payload`](__init__.md#_subagent_from_payload), [`delete_subagent`](__init__.md#delete_subagent), [`list_subagents`](__init__.md#list_subagents), [`delete_subagent`](__init__.md#_RLMCallable.delete_subagent), [`list_subagents`](__init__.md#_RLMCallable.list_subagents)

### `_CallableModule`  ·  implements/extends ModuleType
- def: [`prime-agent-runtime/src/rlm/__init__.py:308`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L308)
- signature: `class _CallableModule(types.ModuleType):`
- protocol/private: `__call__`[`L309`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L309)
- uses (calls/refs, reference-scoped): [`run`](__init__.md#run), [`RLMSpawnHandle`](__init__.md#RLMSpawnHandle)

### `_HarnessProxy`
- def: [`prime-agent-runtime/src/rlm/__init__.py:233`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L233)
- doc: Resolve the harness state against the current environment on every access.
- signature: `class _HarnessProxy:`
- protocol/private: `__getattr__`[`L274`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L274), `__repr__`[`L277`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L277), `_degraded`[`L269`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L269), `_fallback`[`L247`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L247), `_resolve`[`L250`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L250), `_unpersisted`[`L248`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L248)
- uses (calls/refs, reference-scoped): [`get_harness_state`](harness.md#get_harness_state), [`HarnessState`](harness.md#HarnessState)
- used by: [`_harness_state`](__init__.md#_harness_state)

### `_RLMCallable`
- def: [`prime-agent-runtime/src/rlm/__init__.py:284`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L284)
- signature: `class _RLMCallable:`
- members:
  - `delete_subagent(self, target: str | RLMSubagent)` — [`L297`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L297)
  - `find_models(self, query: str = "", limit: int = 8)` — [`L291`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L291)
  - `list_subagents(self)` — [`L294`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L294)
  - `run(self, prompt: str, **kwargs: Any)` — [`L288`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L288)
  - `get_harness_state` — [`L286`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L286)
  - `harness` — [`L285`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L285)
- protocol/private: `__call__`[`L300`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L300)
- uses (calls/refs, reference-scoped): [`get_harness_state`](harness.md#get_harness_state), [`delete_subagent`](__init__.md#delete_subagent), [`run`](__init__.md#run), [`RLMSubagent`](__init__.md#RLMSubagent), [`find_models`](__init__.md#find_models), [`list_subagents`](__init__.md#list_subagents), [`RLMSpawnHandle`](__init__.md#RLMSpawnHandle), [`_harness_state`](__init__.md#_harness_state), [`RLMModel`](__init__.md#RLMModel)
- used by: [`rlm`](__init__.md#rlm)

## Functions
- `__getattr__(name: str)` — [`L341`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L341)
- `_install_control_comm_handlers()` — [`L53`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L53) — Let comm replies arrive on the control channel during an execute_request.
- `_model_from_payload(payload: Any)` — [`L154`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L154)
- `_on_msg(msg: dict[str, Any])` — [`L104`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L104)
- `_resolve_error()` — [`L121`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L121)
- `_resolve_result()` — [`L112`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L112)
- `_resolve_unexpected()` — [`L130`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L130)
- `_spawn_handle_from_payload(payload: Any)` — [`L67`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L67)
- `_subagent_from_payload(payload: Any, operation: str = "rlm.list_subagents")` — [`L179`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L179)
- `delete_subagent(target: str | RLMSubagent)` — [`L219`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L219) — Delete one running or retained direct child from the current parent session.
- `find_models(query: str = "", limit: int = 8)` — [`L166`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L166) — Search a bounded list of models backed by active user credentials.
- `host_request(request_type: str, payload: dict[str, Any] | None = None)` — [`L84`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L84) — Send a typed request to the Prime Agent host and await its reply.
- `list_subagents()` — [`L210`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L210) — List direct RLM children retained by the current parent session.
- `run(prompt: str, **kwargs: Any)` — [`L143`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L143) — Spawn a recursive Prime Agent child and return once its task is admitted.

## Module values
- `HOST_COMM_TARGET` — [`L24`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L24)
- `_LAZY_MCP` — [`L338`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L338)
- `__all__` — [`L315`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L315)
- `_harness_state` — [`L281`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L281)
- `rlm` — [`L304`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/__init__.py#L304)

