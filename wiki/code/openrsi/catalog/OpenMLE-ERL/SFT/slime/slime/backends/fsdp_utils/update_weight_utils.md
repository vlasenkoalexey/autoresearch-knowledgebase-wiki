---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.update_weight_utils`/
symbols:
  UpdateWeight.update_weights: UpdateWeight#update_weights().
  UpdateWeightFromDistributed._group_name: UpdateWeightFromDistributed#_group_name.
  UpdateWeightFromTensor.update_bucket_weights: UpdateWeightFromTensor#update_bucket_weights().
  UpdateWeightFromDistributed.update_bucket_weights: UpdateWeightFromDistributed#update_bucket_weights().
  UpdateWeight: UpdateWeight#
  UpdateWeight.wait_and_update_bucket_weights: UpdateWeight#wait_and_update_bucket_weights().
  UpdateWeight.update_bucket_weights: UpdateWeight#update_bucket_weights().
  UpdateWeightFromTensor.rollout_engines: UpdateWeightFromTensor#rollout_engines.
  UpdateWeightFromDistributed._model_update_groups: UpdateWeightFromDistributed#_model_update_groups.
  UpdateWeight.args: UpdateWeight#args.
  UpdateWeight.connect_rollout_engines: UpdateWeight#connect_rollout_engines().
  UpdateWeightFromTensor: UpdateWeightFromTensor#
  UpdateWeightFromDistributed: UpdateWeightFromDistributed#
  UpdateWeightFromDistributed._is_src_rank: UpdateWeightFromDistributed#_is_src_rank.
  UpdateWeight.weight_version: UpdateWeight#weight_version.
  UpdateWeightFromTensor._ipc_gather_src: UpdateWeightFromTensor#_ipc_gather_src.
  UpdateWeightFromTensor._ipc_gather_group: UpdateWeightFromTensor#_ipc_gather_group.
  UpdateWeightFromTensor._ipc_engine: UpdateWeightFromTensor#_ipc_engine.
  UpdateWeightFromDistributed.rollout_engines: UpdateWeightFromDistributed#rollout_engines.
  logger: logger.
  UpdateWeight.model: UpdateWeight#model.
  UpdateWeightFromTensor.connect_rollout_engines: UpdateWeightFromTensor#connect_rollout_engines().
  UpdateWeight.__init__: UpdateWeight#__init__().
  UpdateWeightFromTensor.tp_rank: UpdateWeightFromTensor#tp_rank.
  UpdateWeightFromDistributed.connect_rollout_engines: UpdateWeightFromDistributed#connect_rollout_engines().
  UpdateWeightFromDistributed.rollout_engine_lock: UpdateWeightFromDistributed#rollout_engine_lock.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py)

## Classes
### `UpdateWeight`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py:32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L32)
- signature: `class UpdateWeight(abc.ABC):`
- members:
  - `connect_rollout_engines(self, rollout_engines: Sequence[ActorHandle], rollout_engine_lock: ActorHandle | None)` — [`L39`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L39)
  - `update_bucket_weights(self, named_tensors, weight_version=None)` — [`L79`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L79)
  - `update_weights(self)` — [`L46`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L46)
  - `wait_and_update_bucket_weights(self, bucket)` — [`L74`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L74)
  - `args` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L34)
  - `model` — [`L35`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L35)
  - `weight_version` — [`L36`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L36)
- protocol/private: `__init__`[`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L33)
- uses (calls/refs, reference-scoped): [`update_bucket_weights`](update_weight_utils.md#UpdateWeightFromDistributed.update_bucket_weights), [`update_bucket_weights`](update_weight_utils.md#UpdateWeightFromTensor.update_bucket_weights), [`UpdateWeightFromDistributed`](update_weight_utils.md#UpdateWeightFromDistributed), [`UpdateWeightFromTensor`](update_weight_utils.md#UpdateWeightFromTensor), [`connect_rollout_engines`](update_weight_utils.md#UpdateWeightFromTensor.connect_rollout_engines), [`connect_rollout_engines`](update_weight_utils.md#UpdateWeightFromDistributed.connect_rollout_engines)
- used by: [`update_weights`](actor.md#FSDPTrainRayActor.update_weights), [`_group_name`](update_weight_utils.md#UpdateWeightFromDistributed._group_name), [`rollout_engines`](update_weight_utils.md#UpdateWeightFromTensor.rollout_engines), [`UpdateWeightFromDistributed`](update_weight_utils.md#UpdateWeightFromDistributed), [`UpdateWeightFromTensor`](update_weight_utils.md#UpdateWeightFromTensor)

### `UpdateWeightFromDistributed`  ·  implements/extends UpdateWeight
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py:177`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L177)
- doc: Broadcast weights via a temporary NCCL group to rollout engines.
- signature: `class UpdateWeightFromDistributed(UpdateWeight):`
- members:
  - `connect_rollout_engines(self, rollout_engines: Sequence[ActorHandle], rollout_engine_lock: ActorHandle | None)` — [`L180`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L180) — On rank 0, initialize a temporary NCCL group for parameter broadcast.
  - `update_bucket_weights(self, named_tensors, weight_version=None)` — [`L222`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L222) — Send names/dtypes/shapes metadata to engines, then broadcast tensors.
  - `rollout_engine_lock` — [`L187`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L187)
  - `rollout_engines` — [`L186`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L186)
- protocol/private: `_group_name`[`L194`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L194), `_is_src_rank`[`L192`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L192), `_model_update_groups`[`L213`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L213)
- uses (calls/refs, reference-scoped): [`UpdateWeight`](update_weight_utils.md#UpdateWeight), [`init_process_group`](../../utils/distributed_utils.md#init_process_group), [`args`](update_weight_utils.md#UpdateWeight.args)
- used by: [`weight_updater`](actor.md#FSDPTrainRayActor.weight_updater), [`UpdateWeight`](update_weight_utils.md#UpdateWeight), [`update_bucket_weights`](update_weight_utils.md#UpdateWeight.update_bucket_weights), [`connect_rollout_engines`](update_weight_utils.md#UpdateWeight.connect_rollout_engines)

### `UpdateWeightFromTensor`  ·  implements/extends UpdateWeight
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py:83`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L83)
- doc: Push model weights to rollout engines using tensors.
- signature: `class UpdateWeightFromTensor(UpdateWeight):`
- members:
  - `connect_rollout_engines(self, rollout_engines: Sequence[ActorHandle], rollout_engine_lock: ActorHandle | None)` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L91) — Attach rollout engines and create per-engine IPC (Gloo) groups.
  - `update_bucket_weights(self, named_tensors, weight_version=None)` — [`L119`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L119)
  - `rollout_engines` — [`L101`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L101)
  - `tp_rank` — [`L117`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L117)
- protocol/private: `_ipc_engine`[`L115`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L115), `_ipc_gather_group`[`L114`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L114), `_ipc_gather_src`[`L113`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L113)
- uses (calls/refs, reference-scoped): [`UpdateWeight`](update_weight_utils.md#UpdateWeight), [`args`](update_weight_utils.md#UpdateWeight.args), [`logger`](update_weight_utils.md#logger)
- used by: [`update_weights`](actor.md#FSDPTrainRayActor.update_weights), [`weight_updater`](actor.md#FSDPTrainRayActor.weight_updater), [`UpdateWeight`](update_weight_utils.md#UpdateWeight), [`update_bucket_weights`](update_weight_utils.md#UpdateWeight.update_bucket_weights), [`connect_rollout_engines`](update_weight_utils.md#UpdateWeight.connect_rollout_engines)

## Module values
- `logger` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/update_weight_utils.py#L29)

