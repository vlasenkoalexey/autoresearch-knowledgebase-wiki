---
title: 'Module: OpenMLE-Evo/tts_search/airaevo_concurrency.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/airaevo_concurrency.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.airaevo_concurrency`/
symbols:
  _connect_client_manager: _connect_client_manager().
  SharedConcurrencyServer.env: SharedConcurrencyServer#env.
  acquire_sandbox_slot_async: acquire_sandbox_slot_async().
  _get_llm_semaphore_proxy: _get_llm_semaphore_proxy().
  _get_sandbox_semaphore_proxy: _get_sandbox_semaphore_proxy().
  SharedConcurrencyServer._manager: SharedConcurrencyServer#_manager.
  SharedConcurrencyServer.__init__: SharedConcurrencyServer#__init__().
  resolve_task_concurrency_per_epoch: resolve_task_concurrency_per_epoch().
  _client_manager._client_manager: _client_manager._client_manager.
  _ClientSemaphoreManager: _ClientSemaphoreManager#
  acquire_llm_slot_async: acquire_llm_slot_async().
  _acquire_semaphore_async: _acquire_semaphore_async().
  acquire_llm_slot: acquire_llm_slot().
  acquire_sandbox_slot: acquire_sandbox_slot().
  _llm_semaphore_proxy._llm_semaphore_proxy: _llm_semaphore_proxy._llm_semaphore_proxy.
  _sandbox_semaphore_proxy._sandbox_semaphore_proxy: _sandbox_semaphore_proxy._sandbox_semaphore_proxy.
  SharedConcurrencyServer._get_llm_semaphore: SharedConcurrencyServer#_get_llm_semaphore().
  SharedConcurrencyServer._get_sandbox_semaphore: SharedConcurrencyServer#_get_sandbox_semaphore().
  SharedConcurrencyServer.shutdown: SharedConcurrencyServer#shutdown().
  SharedConcurrencyServer.__init__._ServerSemaphoreManager: SharedConcurrencyServer#__init__()._ServerSemaphoreManager#
  _client_lock: _client_lock.
  ENV_ENABLED: ENV_ENABLED.
  ENV_HOST: ENV_HOST.
  ENV_PORT: ENV_PORT.
  ENV_AUTHKEY: ENV_AUTHKEY.
  SharedConcurrencyServer: SharedConcurrencyServer#
  ASYNC_SEMAPHORE_POLL_INTERVAL_SECONDS: ASYNC_SEMAPHORE_POLL_INTERVAL_SECONDS.
  SharedConcurrencyServer._llm_semaphore: SharedConcurrencyServer#_llm_semaphore.
  SharedConcurrencyServer._sandbox_semaphore: SharedConcurrencyServer#_sandbox_semaphore.
---
# Module: [`OpenMLE-Evo/tts_search/airaevo_concurrency.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py)

## Classes
### `SharedConcurrencyServer`
- def: [`OpenMLE-Evo/tts_search/airaevo_concurrency.py:31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L31)
- signature: `class SharedConcurrencyServer:`
- members:
  - `shutdown(self)` — [`L68`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L68)
  - `env` — [`L55`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L55)
- protocol/private: `__init__`[`L32`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L32), `_get_llm_semaphore`[`L62`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L62), `_get_sandbox_semaphore`[`L65`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L65), `_llm_semaphore`[`L33`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L33), `_manager`[`L49`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L49), `_sandbox_semaphore`[`L34`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L34)
- uses (calls/refs, reference-scoped): [`_ServerSemaphoreManager`](airaevo_concurrency.md#SharedConcurrencyServer.__init__._ServerSemaphoreManager), [`ENV_AUTHKEY`](airaevo_concurrency.md#ENV_AUTHKEY), [`ENV_ENABLED`](airaevo_concurrency.md#ENV_ENABLED), [`ENV_HOST`](airaevo_concurrency.md#ENV_HOST), [`ENV_PORT`](airaevo_concurrency.md#ENV_PORT)
- used by: (2 test-only callers)

### `_ClientSemaphoreManager`  ·  implements/extends SyncManager
- def: [`OpenMLE-Evo/tts_search/airaevo_concurrency.py:23`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L23)
- signature: `class _ClientSemaphoreManager(SyncManager):`
- used by: [`_connect_client_manager`](airaevo_concurrency.md#_connect_client_manager), [`_client_manager`](airaevo_concurrency.md#_client_manager._client_manager)

### `_ServerSemaphoreManager`  ·  implements/extends SyncManager
- def: [`OpenMLE-Evo/tts_search/airaevo_concurrency.py:37`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L37)
- signature: `class _ServerSemaphoreManager(SyncManager):`
- used by: [`_manager`](airaevo_concurrency.md#SharedConcurrencyServer._manager), [`__init__`](airaevo_concurrency.md#SharedConcurrencyServer.__init__)

## Functions
- `_acquire_semaphore_async(semaphore: Any)` — [`L135`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L135)
- `_connect_client_manager()` — [`L96`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L96)
- `_get_llm_semaphore_proxy()` — [`L113`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L113)
- `_get_sandbox_semaphore_proxy()` — [`L124`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L124)
- `acquire_llm_slot()` — [`L143`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L143)
- `acquire_llm_slot_async()` — [`L175`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L175)
- `acquire_sandbox_slot()` — [`L159`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L159)
- `acquire_sandbox_slot_async()` — [`L189`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L189)
- `resolve_task_concurrency_per_epoch(*, configured_task_concurrency: int | None, llm_concurrency: int, sandbox_concurrency: int, num_epochs: int, async_workers: int | str | None = 1)` — [`L78`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L78) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)

## Module values
- `ASYNC_SEMAPHORE_POLL_INTERVAL_SECONDS` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L20)
- `ENV_AUTHKEY` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L19)
- `ENV_ENABLED` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L16)
- `ENV_HOST` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L17)
- `ENV_PORT` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L18)
- `_client_lock` — [`L75`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L75)
- `_client_manager` — [`L72`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L72)
- `_llm_semaphore_proxy` — [`L73`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L73)
- `_sandbox_semaphore_proxy` — [`L74`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/airaevo_concurrency.py#L74)

