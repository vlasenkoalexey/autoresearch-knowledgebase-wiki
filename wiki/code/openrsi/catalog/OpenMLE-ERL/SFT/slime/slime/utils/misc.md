---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/misc.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/misc.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.misc`/
symbols:
  load_function: load_function().
  Box: Box#
  SingletonMeta: SingletonMeta#
  should_run_periodic_action: should_run_periodic_action().
  get_free_port: get_free_port().
  chunk_named_params_by_size: chunk_named_params_by_size().
  SingletonMeta._instances: SingletonMeta#_instances.
  group_by: group_by().
  SingletonMeta.__call__: SingletonMeta#__call__().
  SingletonMeta.clear_instances: SingletonMeta#clear_instances().
  Box.inner: Box#inner().
  get_current_node_ip: get_current_node_ip().
  Box._inner: Box#_inner.
  _chunk_by_size: _chunk_by_size().
  exec_command: exec_command().
  Box.__init__: Box#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/misc.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py)

## Classes
### `Box`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/misc.py:97`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L97)
- signature: `class Box:`
- members:
  - `inner(self)` — [`L102`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L102)
- protocol/private: `__init__`[`L98`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L98), `_inner`[`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L99)
- used by: [`train`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.train), [`train`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train), [`_get_rollout_data`](../backends/megatron_utils/actor.md#MegatronTrainRayActor._get_rollout_data), [`_split_train_data_by_dp`](../ray/rollout.md#RolloutManager._split_train_data_by_dp)

### `SingletonMeta`  ·  implements/extends type
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/misc.py:20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L20)
- doc: A metaclass for creating singleton classes.
- signature: `class SingletonMeta(type):`
- members:
  - `clear_instances(cls)` — [`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L33)
- protocol/private: `__call__`[`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L27), `_instances`[`L25`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L25)
- used by: [`Timer`](timer.md#Timer), [`GenerateState`](../rollout/sglang_rollout.md#GenerateState), [`_TensorboardAdapter`](tensorboard_utils.md#_TensorboardAdapter)

## Functions
- `_chunk_by_size(objects: Iterable[Any], compute_size: Callable[[Any], int], chunk_size: int)` — [`L131`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L131)
- `chunk_named_params_by_size(named_params: Iterable[tuple[str, torch.Tensor]], chunk_size: int)` — [`L123`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L123)
- `exec_command(cmd: str, capture_output: bool = False)` — [`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L37)
- `get_current_node_ip()` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L58)
- `get_free_port(start_port=10000, consecutive=1)` — [`L65`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L65)
- `group_by(iterable, key=None)` — [`L114`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L114) — Similar to itertools.groupby, but do not require iterable to be sorted
- `load_function(path)` — [`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L9) — Load a function from a module.
- `should_run_periodic_action(rollout_id: int, interval: int | None, num_rollout_per_epoch: int | None = None, num_rollout: int | None = None)` — [`L73`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/misc.py#L73) — Return True when a periodic action (eval/save/checkpoint) should run.

