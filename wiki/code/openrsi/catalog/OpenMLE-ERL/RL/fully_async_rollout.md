---
title: 'Module: OpenMLE-ERL/RL/fully_async_rollout.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/fully_async_rollout.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.fully_async_rollout`/
symbols:
  AsyncRolloutWorker.continuous_worker_loop: AsyncRolloutWorker#continuous_worker_loop().
  _global_worker: _global_worker.
  generate_rollout_async: generate_rollout_async().
  get_global_worker: get_global_worker().
  AsyncRolloutWorker.worker_thread: AsyncRolloutWorker#worker_thread.
  AsyncRolloutWorker.pause_and_wait_idle: AsyncRolloutWorker#pause_and_wait_idle().
  generate_rollout_fully_async: generate_rollout_fully_async().
  get_existing_global_worker: get_existing_global_worker().
  stop_global_worker: stop_global_worker().
  AsyncRolloutWorker.stop: AsyncRolloutWorker#stop().
  AsyncRolloutWorker.get_queue_size: AsyncRolloutWorker#get_queue_size().
  _reset_sample_for_generation_retry: _reset_sample_for_generation_retry().
  AsyncRolloutWorker.idle: AsyncRolloutWorker#idle.
  AsyncRolloutWorker.start: AsyncRolloutWorker#start().
  AsyncRolloutWorker.resume: AsyncRolloutWorker#resume().
  AsyncRolloutWorker.pause_requested: AsyncRolloutWorker#pause_requested.
  AsyncRolloutWorker.make_callback: AsyncRolloutWorker#make_callback().
  AsyncRolloutWorker.task_done_callback: AsyncRolloutWorker#task_done_callback().
  AsyncRolloutWorker.worker_thread_func: AsyncRolloutWorker#worker_thread_func().
  AsyncRolloutWorker.get_completed_groups: AsyncRolloutWorker#get_completed_groups().
  _worker_lock: _worker_lock.
  AsyncRolloutWorker.running: AsyncRolloutWorker#running.
  AsyncRolloutWorker.output_queue: AsyncRolloutWorker#output_queue.
  AsyncRolloutWorker.args: AsyncRolloutWorker#args.
  _GENERATION_ABORT_METADATA_KEYS: _GENERATION_ABORT_METADATA_KEYS.
  _GENERATION_ABORT_CODE_CATEGORIES: _GENERATION_ABORT_CODE_CATEGORIES.
  _sample_has_generation_abort: _sample_has_generation_abort().
  AsyncRolloutWorker.data_buffer: AsyncRolloutWorker#data_buffer.
  AsyncRolloutWorker.state: AsyncRolloutWorker#state.
  AsyncRolloutWorker: AsyncRolloutWorker#
  AsyncRolloutWorker.__init__: AsyncRolloutWorker#__init__().
  AsyncRolloutWorker.concurrency: AsyncRolloutWorker#concurrency.
---
# Module: [`OpenMLE-ERL/RL/fully_async_rollout.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py)

## Classes
### `AsyncRolloutWorker`
- def: [`OpenMLE-ERL/RL/fully_async_rollout.py:86`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L86)
- members:
  - `continuous_worker_loop(self)` — [`L103`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L103) — Continuous work loop - constantly get data from data_buffer and process
  - `get_completed_groups(self)` — [`L224`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L224) — Get completed sample groups
  - `get_queue_size(self)` — [`L235`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L235) — Get current output queue size
  - `make_callback(gid)` — [`L155`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L155)
  - `pause_and_wait_idle(self, timeout: float | None = None)` — [`L208`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L208) — Pause new training rollout submissions and wait for in-flight groups.
  - `resume(self)` — [`L218`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L218) — Resume training rollout submissions after eval.
  - `start(self)` — [`L193`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L193) — Start continuous work mode
  - `stop(self)` — [`L200`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L200) — Stop worker thread
  - `task_done_callback(task)` — [`L156`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L156)
  - `worker_thread_func(self)` — [`L189`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L189) — Worker function running in independent thread
  - `args` — [`L93`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L93)
  - `concurrency` — [`L95`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L95)
  - `data_buffer` — [`L94`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L94)
  - `idle` — [`L101`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L101)
  - `output_queue` — [`L97`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L97)
  - `pause_requested` — [`L100`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L100)
  - `running` — [`L96`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L96)
  - `state` — [`L99`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L99)
  - `worker_thread` — [`L98`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L98)
- protocol/private: `__init__`[`L92`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L92)
- used by: [`generate_rollout_async`](fully_async_rollout.md#generate_rollout_async), [`get_global_worker`](fully_async_rollout.md#get_global_worker), [`generate_rollout_fully_async`](fully_async_rollout.md#generate_rollout_fully_async), [`get_existing_global_worker`](fully_async_rollout.md#get_existing_global_worker), [`stop_global_worker`](fully_async_rollout.md#stop_global_worker)

## Functions
- `_reset_sample_for_generation_retry(sample: Sample)` — [`L32`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L32)
- `_sample_has_generation_abort(sample: Sample)` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L25)
- `generate_rollout_async(args, rollout_id: int, data_buffer)` — [`L240`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L240) — Simplified asynchronous rollout generation - using global continuous worker
- `generate_rollout_fully_async(args, rollout_id, data_buffer, evaluation=False)` — [`L346`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L346)
- `get_existing_global_worker()` — [`L66`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L66) — Return the existing worker without creating a new one.
- `get_global_worker(args, data_buffer)` — [`L53`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L53) — Get or create global worker
- `stop_global_worker()` — [`L77`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L77) — Stop global worker

## Module values
- `_GENERATION_ABORT_CODE_CATEGORIES` — [`L22`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L22)
- `_GENERATION_ABORT_METADATA_KEYS` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L16)
- `_global_worker` — [`L14`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L14)
- `_worker_lock` — [`L15`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/fully_async_rollout.py#L15)

