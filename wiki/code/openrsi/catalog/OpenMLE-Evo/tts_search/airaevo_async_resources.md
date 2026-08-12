---
title: 'Module: OpenMLE-Evo/tts_search/airaevo_async_resources.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/airaevo_async_resources.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.airaevo_async_resources`/
symbols:
  build_worker_specs: build_worker_specs().
  WorkerSpec: WorkerSpec#
  resolve_async_worker_count: resolve_async_worker_count().
  resolve_execution_mode: resolve_execution_mode().
  WorkerSpec.worker_id: WorkerSpec#worker_id.
  WorkerSpec.sandbox_url: WorkerSpec#sandbox_url.
  WorkerSpec.gpu_index: WorkerSpec#gpu_index.
  RoundRobinSandboxPool.next_url: RoundRobinSandboxPool#next_url().
  fetch_router_idle_worker_count: fetch_router_idle_worker_count().
  detect_gpu_indices: detect_gpu_indices().
  resolve_async_sandbox_urls: resolve_async_sandbox_urls().
  RoundRobinSandboxPool: RoundRobinSandboxPool#
  EXECUTION_MODES: EXECUTION_MODES.
  SANDBOX_ASSIGNMENTS: SANDBOX_ASSIGNMENTS.
  RoundRobinSandboxPool.urls: RoundRobinSandboxPool#urls.
  RoundRobinSandboxPool._index: RoundRobinSandboxPool#_index.
  RoundRobinSandboxPool.__init__: RoundRobinSandboxPool#__init__().
---
# Module: [`OpenMLE-Evo/tts_search/airaevo_async_resources.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py)

## Classes
### `RoundRobinSandboxPool`
- def: [`OpenMLE-Evo/tts_search/airaevo_async_resources.py:74`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L74) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- signature: `class RoundRobinSandboxPool:`
- members:
  - `next_url(self)` — [`L79`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L79) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
  - `urls` — [`L76`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L76) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- protocol/private: `__init__`[`L75`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L75), `_index`[`L77`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L77)
- used by: [`build_worker_specs`](airaevo_async_resources.md#build_worker_specs)  (2 test-only)

### `WorkerSpec`
- def: [`OpenMLE-Evo/tts_search/airaevo_async_resources.py:68`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L68) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- signature: `class WorkerSpec:`
- members:
  - `gpu_index` — [`L70`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L70) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
  - `sandbox_url` — [`L71`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L71) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
  - `worker_id` — [`L69`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L69) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- used by: [`_debug_cycle_async`](../third_party/aira-evo/src/dojo/solvers/evo/evo.md#Evolutionary._debug_cycle_async), [`_async_worker_loop`](../third_party/aira-evo/src/dojo/solvers/evo/evo.md#Evolutionary._async_worker_loop), [`_next_async_work_item`](../third_party/aira-evo/src/dojo/solvers/evo/evo.md#Evolutionary._next_async_work_item), [`_create_node_from_work_item`](../third_party/aira-evo/src/dojo/solvers/evo/evo.md#Evolutionary._create_node_from_work_item), [`build_worker_specs`](airaevo_async_resources.md#build_worker_specs), [`worker`](../third_party/aira-evo/src/dojo/solvers/evo/evo.md#AsyncWorkItem.worker)  (6 test-only)

## Functions
- `build_worker_specs(*, worker_count: int, sandbox_urls: list[str], assignment: str = "round_robin")` — [`L85`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L85) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `detect_gpu_indices()` — [`L22`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L22) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `fetch_router_idle_worker_count(router_url: str, *, api_key: str | None = None, timeout_seconds: float = 5)` — [`L113`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L113)
- `resolve_async_sandbox_urls(value: Any, *, fallback_url: str | None = None)` — [`L54`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L54)
- `resolve_async_worker_count(value: int | str | None, *, gpu_indices: list[int] | None = None)` — [`L41`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L41) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `resolve_execution_mode(value: str | None)` — [`L12`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L12) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)

## Module values
- `EXECUTION_MODES` — [`L8`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L8) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `SANDBOX_ASSIGNMENTS` — [`L9`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_async_resources.py#L9) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)

