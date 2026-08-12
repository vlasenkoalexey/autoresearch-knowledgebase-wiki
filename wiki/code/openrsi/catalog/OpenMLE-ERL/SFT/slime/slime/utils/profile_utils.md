---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.profile_utils`/
symbols:
  TrainProfiler._memory_profiler_overall: TrainProfiler#_memory_profiler_overall.
  TrainProfiler.step: TrainProfiler#step().
  _TorchMemoryProfiler.oom_observer: _TorchMemoryProfiler#oom_observer().
  _MemrayMemoryProfiler.stop: _MemrayMemoryProfiler#stop().
  _MemrayMemoryProfiler._tracker: _MemrayMemoryProfiler#_tracker.
  TrainProfiler.iterate_train_actor: TrainProfiler#iterate_train_actor().
  TrainProfiler.iterate_train_log_probs: TrainProfiler#iterate_train_log_probs().
  _BaseMemoryProfiler.create: _BaseMemoryProfiler#create().
  _BaseMemoryProfiler._path_dump: _BaseMemoryProfiler#_path_dump.
  logger: logger.
  TrainProfiler._torch_profiler_overall: TrainProfiler#_torch_profiler_overall.
  _BaseMemoryProfiler.start: _BaseMemoryProfiler#start().
  _BaseMemoryProfiler.stop: _BaseMemoryProfiler#stop().
  _TorchMemoryProfiler.start: _TorchMemoryProfiler#start().
  _TorchMemoryProfiler.stop: _TorchMemoryProfiler#stop().
  TrainProfiler.on_init_end: TrainProfiler#on_init_end().
  _profile_simple_loop: _profile_simple_loop().
  TrainProfiler: TrainProfiler#
  _TorchMemoryProfiler: _TorchMemoryProfiler#
  _MemrayMemoryProfiler: _MemrayMemoryProfiler#
  TrainProfiler.args: TrainProfiler#args.
  _BaseMemoryProfiler: _BaseMemoryProfiler#
  _MemrayMemoryProfiler.__init__: _MemrayMemoryProfiler#__init__().
  _MemrayMemoryProfiler.start: _MemrayMemoryProfiler#start().
  _create_torch_profiler: _create_torch_profiler().
  _BaseMemoryProfiler.__init__: _BaseMemoryProfiler#__init__().
  TrainProfiler.__init__: TrainProfiler#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py)

## Classes
### `TrainProfiler`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py:13`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L13)
- signature: `class TrainProfiler:`
- members:
  - `iterate_train_actor(self, iterator)` — [`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L41)
  - `iterate_train_log_probs(self, iterator)` — [`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L44)
  - `on_init_end(self)` — [`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L26)
  - `step(self, rollout_id: int)` — [`L30`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L30)
  - `args` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L15)
- protocol/private: `__init__`[`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L14), `_memory_profiler_overall`[`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L17), `_torch_profiler_overall`[`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L16)
- uses (calls/refs, reference-scoped): [`create`](profile_utils.md#_BaseMemoryProfiler.create), [`_profile_simple_loop`](profile_utils.md#_profile_simple_loop), [`_BaseMemoryProfiler`](profile_utils.md#_BaseMemoryProfiler), [`_create_torch_profiler`](profile_utils.md#_create_torch_profiler)
- used by: [`train_actor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_actor), [`_train_core`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._train_core), [`_compute_log_prob`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._compute_log_prob), [`rollout_data_postprocess`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.rollout_data_postprocess), [`max_tokens_per_gpu`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.max_tokens_per_gpu), [`prof`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.prof), [`prof`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.prof)

### `_BaseMemoryProfiler`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py:81`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L81)
- members:
  - `create(args)` — [`L83`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L83)
  - `start(self)` — [`L96`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L96)
  - `stop(self)` — [`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L99)
- protocol/private: `__init__`[`L90`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L90), `_path_dump`[`L91`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L91)
- uses (calls/refs, reference-scoped): [`stop`](profile_utils.md#_MemrayMemoryProfiler.stop), [`start`](profile_utils.md#_TorchMemoryProfiler.start), [`stop`](profile_utils.md#_TorchMemoryProfiler.stop), [`_MemrayMemoryProfiler`](profile_utils.md#_MemrayMemoryProfiler), [`_TorchMemoryProfiler`](profile_utils.md#_TorchMemoryProfiler), [`start`](profile_utils.md#_MemrayMemoryProfiler.start)
- used by: [`_memory_profiler_overall`](profile_utils.md#TrainProfiler._memory_profiler_overall), [`oom_observer`](profile_utils.md#_TorchMemoryProfiler.oom_observer), [`stop`](profile_utils.md#_MemrayMemoryProfiler.stop), [`_tracker`](profile_utils.md#_MemrayMemoryProfiler._tracker), [`stop`](profile_utils.md#_TorchMemoryProfiler.stop), [`_MemrayMemoryProfiler`](profile_utils.md#_MemrayMemoryProfiler), [`_TorchMemoryProfiler`](profile_utils.md#_TorchMemoryProfiler), [`__init__`](profile_utils.md#_MemrayMemoryProfiler.__init__)

### `_MemrayMemoryProfiler`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py:130`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L130)
- members:
  - `start(self)` — [`L135`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L135)
  - `stop(self)` — [`L145`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L145)
- protocol/private: `__init__`[`L131`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L131), `_tracker`[`L139`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L139)
- uses (calls/refs, reference-scoped): [`_path_dump`](profile_utils.md#_BaseMemoryProfiler._path_dump), [`logger`](profile_utils.md#logger), [`_BaseMemoryProfiler`](profile_utils.md#_BaseMemoryProfiler), [`__init__`](profile_utils.md#_BaseMemoryProfiler.__init__)
- used by: [`create`](profile_utils.md#_BaseMemoryProfiler.create), [`start`](profile_utils.md#_BaseMemoryProfiler.start), [`stop`](profile_utils.md#_BaseMemoryProfiler.stop)

### `_TorchMemoryProfiler`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py:103`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L103)
- members:
  - `oom_observer(device, alloc, device_alloc, device_free)` — [`L114`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L114)
  - `start(self)` — [`L104`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L104)
  - `stop(self)` — [`L124`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L124)
- uses (calls/refs, reference-scoped): [`print_memory`](memory_utils.md#print_memory), [`_path_dump`](profile_utils.md#_BaseMemoryProfiler._path_dump), [`logger`](profile_utils.md#logger), [`_BaseMemoryProfiler`](profile_utils.md#_BaseMemoryProfiler)
- used by: [`create`](profile_utils.md#_BaseMemoryProfiler.create), [`start`](profile_utils.md#_BaseMemoryProfiler.start), [`stop`](profile_utils.md#_BaseMemoryProfiler.stop)

## Functions
- `_create_torch_profiler(args, name)` — [`L60`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L60)
- `_profile_simple_loop(iterator, args, name)` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L48)

## Module values
- `logger` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/profile_utils.py#L10)

