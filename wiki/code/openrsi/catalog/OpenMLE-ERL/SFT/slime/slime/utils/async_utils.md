---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.async_utils`/
symbols:
  run: run().
  AsyncLoopThread._thread: AsyncLoopThread#_thread.
  get_async_loop: get_async_loop().
  async_loop: async_loop.
  AsyncLoopThread._start_loop: AsyncLoopThread#_start_loop().
  AsyncLoopThread.run: AsyncLoopThread#run().
  AsyncLoopThread.loop: AsyncLoopThread#loop.
  AsyncLoopThread: AsyncLoopThread#
  __all__: __all__.
  AsyncLoopThread.__init__: AsyncLoopThread#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py)

## Classes
### `AsyncLoopThread`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py:8`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L8)
- signature: `class AsyncLoopThread:`
- members:
  - `run(self, coro)` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L18)
  - `loop` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L10)
- protocol/private: `__init__`[`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L9), `_start_loop`[`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L14), `_thread`[`L11`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L11)
- used by: [`run`](async_utils.md#run), [`get_async_loop`](async_utils.md#get_async_loop)

## Functions
- `get_async_loop()` — [`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L27)
- `run(coro)` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L34) — Run a coroutine in the background event loop.

## Module values
- `__all__` — [`L4`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L4)
- `async_loop` — [`L24`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/async_utils.py#L24)

