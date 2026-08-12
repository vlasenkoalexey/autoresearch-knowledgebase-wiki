---
title: 'Module: OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.airaevo_concurrency`/
symbols:
  _connect_client_manager: _connect_client_manager().
  SharedConcurrencyServer.env: SharedConcurrencyServer#env.
  SharedConcurrencyServer._manager: SharedConcurrencyServer#_manager.
  SharedConcurrencyServer.__init__: SharedConcurrencyServer#__init__().
  _client_manager._client_manager: _client_manager._client_manager.
  _get_llm_semaphore_proxy: _get_llm_semaphore_proxy().
  _get_sandbox_semaphore_proxy: _get_sandbox_semaphore_proxy().
  _ClientSemaphoreManager: _ClientSemaphoreManager#
  acquire_llm_slot: acquire_llm_slot().
  acquire_sandbox_slot: acquire_sandbox_slot().
  _llm_semaphore_proxy._llm_semaphore_proxy: _llm_semaphore_proxy._llm_semaphore_proxy.
  _sandbox_semaphore_proxy._sandbox_semaphore_proxy: _sandbox_semaphore_proxy._sandbox_semaphore_proxy.
  SharedConcurrencyServer._get_llm_semaphore: SharedConcurrencyServer#_get_llm_semaphore().
  SharedConcurrencyServer._get_sandbox_semaphore: SharedConcurrencyServer#_get_sandbox_semaphore().
  SharedConcurrencyServer.shutdown: SharedConcurrencyServer#shutdown().
  SharedConcurrencyServer.__init__._ServerSemaphoreManager: SharedConcurrencyServer#__init__()._ServerSemaphoreManager#
  ENV_ENABLED: ENV_ENABLED.
  ENV_HOST: ENV_HOST.
  ENV_PORT: ENV_PORT.
  ENV_AUTHKEY: ENV_AUTHKEY.
  SharedConcurrencyServer: SharedConcurrencyServer#
  resolve_task_concurrency_per_epoch: resolve_task_concurrency_per_epoch().
  SharedConcurrencyServer._llm_semaphore: SharedConcurrencyServer#_llm_semaphore.
  SharedConcurrencyServer._sandbox_semaphore: SharedConcurrencyServer#_sandbox_semaphore.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py)

## Classes
### `SharedConcurrencyServer`
- def: [`OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py:28`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L28)
- signature: `class SharedConcurrencyServer:`
- members:
  - `shutdown(self)` — [`L65`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L65)
  - `env` — [`L52`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L52)
- protocol/private: `__init__`[`L29`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L29), `_get_llm_semaphore`[`L59`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L59), `_get_sandbox_semaphore`[`L62`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L62), `_llm_semaphore`[`L30`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L30), `_manager`[`L46`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L46), `_sandbox_semaphore`[`L31`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L31)
- uses (calls/refs, reference-scoped): [`_ServerSemaphoreManager`](airaevo_concurrency.md#SharedConcurrencyServer.__init__._ServerSemaphoreManager), [`ENV_AUTHKEY`](airaevo_concurrency.md#ENV_AUTHKEY), [`ENV_ENABLED`](airaevo_concurrency.md#ENV_ENABLED), [`ENV_HOST`](airaevo_concurrency.md#ENV_HOST), [`ENV_PORT`](airaevo_concurrency.md#ENV_PORT)
- used by: (1 test-only callers)

### `_ClientSemaphoreManager`  ·  implements/extends SyncManager
- def: [`OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py:20`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L20)
- signature: `class _ClientSemaphoreManager(SyncManager):`
- used by: [`_connect_client_manager`](airaevo_concurrency.md#_connect_client_manager), [`_client_manager`](airaevo_concurrency.md#_client_manager._client_manager)

### `_ServerSemaphoreManager`  ·  implements/extends SyncManager
- def: [`OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py:34`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L34)
- signature: `class _ServerSemaphoreManager(SyncManager):`
- used by: [`_manager`](airaevo_concurrency.md#SharedConcurrencyServer._manager), [`__init__`](airaevo_concurrency.md#SharedConcurrencyServer.__init__)

## Functions
- `_connect_client_manager()` — [`L88`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L88)
- `_get_llm_semaphore_proxy()` — [`L103`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L103)
- `_get_sandbox_semaphore_proxy()` — [`L113`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L113)
- `acquire_llm_slot()` — [`L124`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L124)
- `acquire_sandbox_slot()` — [`L140`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L140)
- `resolve_task_concurrency_per_epoch(*, configured_task_concurrency: int | None, llm_concurrency: int, sandbox_concurrency: int, num_epochs: int)` — [`L74`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L74)

## Module values
- `ENV_AUTHKEY` — [`L17`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L17)
- `ENV_ENABLED` — [`L14`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L14)
- `ENV_HOST` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L15)
- `ENV_PORT` — [`L16`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L16)
- `_client_manager` — [`L69`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L69)
- `_llm_semaphore_proxy` — [`L70`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L70)
- `_sandbox_semaphore_proxy` — [`L71`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/airaevo_concurrency.py#L71)

