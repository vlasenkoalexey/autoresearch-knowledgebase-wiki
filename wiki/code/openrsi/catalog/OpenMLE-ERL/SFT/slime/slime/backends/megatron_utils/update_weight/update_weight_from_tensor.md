---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.update_weight_from_tensor`/
symbols:
  UpdateWeightFromTensor._send_hf_params: UpdateWeightFromTensor#_send_hf_params().
  UpdateWeightFromTensor._group_name: UpdateWeightFromTensor#_group_name.
  UpdateWeightFromTensor.update_weights: UpdateWeightFromTensor#update_weights().
  UpdateWeightFromTensor.rollout_engines: UpdateWeightFromTensor#rollout_engines.
  UpdateWeightFromTensor.args: UpdateWeightFromTensor#args.
  UpdateWeightFromTensor._hf_weight_iterator: UpdateWeightFromTensor#_hf_weight_iterator.
  UpdateWeightFromTensor.use_distribute: UpdateWeightFromTensor#use_distribute.
  UpdateWeightFromTensor.weight_version: UpdateWeightFromTensor#weight_version.
  UpdateWeightFromTensor.quantization_config: UpdateWeightFromTensor#quantization_config.
  UpdateWeightFromTensor._model_update_groups: UpdateWeightFromTensor#_model_update_groups.
  UpdateWeightFromTensor.distributed_rollout_engines: UpdateWeightFromTensor#distributed_rollout_engines.
  UpdateWeightFromTensor: UpdateWeightFromTensor#
  UpdateWeightFromTensor._is_distributed_src_rank: UpdateWeightFromTensor#_is_distributed_src_rank.
  UpdateWeightFromTensor.weights_getter: UpdateWeightFromTensor#weights_getter.
  UpdateWeightFromTensor._ipc_gather_group: UpdateWeightFromTensor#_ipc_gather_group.
  UpdateWeightFromTensor._ipc_gather_src: UpdateWeightFromTensor#_ipc_gather_src.
  UpdateWeightFromTensor.connect_rollout_engines: UpdateWeightFromTensor#connect_rollout_engines().
  UpdateWeightFromTensor._ipc_engine: UpdateWeightFromTensor#_ipc_engine.
  _send_to_colocated_engine: _send_to_colocated_engine().
  UpdateWeightFromTensor.__init__: UpdateWeightFromTensor#__init__().
  UpdateWeightFromTensor.model: UpdateWeightFromTensor#model.
  UpdateWeightFromTensor.model_name: UpdateWeightFromTensor#model_name.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py)

## Classes
### `UpdateWeightFromTensor`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py:24`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L24)
- doc: Update rollout engines from tensor dict:
- signature: `class UpdateWeightFromTensor:`
- members:
  - `__init__(self, args: Namespace, model: Sequence[torch.nn.Module], weights_getter: Callable[[], Mapping[str, torch.Tensor]], *, model_name: str, quantization_config: dict[str, int | str | list[str]] | None)` — [`L32`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L32) — Compute param buckets, create IPC Gloo groups (rollout_num_gpus_per_engine ranks/group).
  - `connect_rollout_engines(self, rollout_engines: Sequence[ActorHandle], rollout_engine_lock: ActorHandle)` — [`L66`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L66) — Split colocated/distributed engines. Global source rank (DP=TP=PP=0) creates NCCL
  - `update_weights(self)` — [`L107`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L107) — version++, flush caches, process buckets. Progress on rank 0.
  - `args` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L44)
  - `distributed_rollout_engines` — [`L81`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L81)
  - `model` — [`L45`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L45)
  - `model_name` — [`L47`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L47)
  - `quantization_config` — [`L48`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L48)
  - `rollout_engines` — [`L73`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L73)
  - `use_distribute` — [`L77`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L77)
  - `weight_version` — [`L49`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L49)
  - `weights_getter` — [`L46`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L46)
- protocol/private: `_group_name`[`L87`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L87), `_hf_weight_iterator`[`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L51), `_ipc_engine`[`L104`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L104), `_ipc_gather_group`[`L61`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L61), `_ipc_gather_src`[`L62`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L62), `_is_distributed_src_rank`[`L82`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L82), `_model_update_groups`[`L64`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L64), `_send_hf_params`[`L145`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L145)
- uses (calls/refs, reference-scoped): [`get_gloo_group`](../../../utils/distributed_utils.md#get_gloo_group), [`HfWeightIteratorBase`](hf_weight_iterator_base.md#HfWeightIteratorBase), [`create`](hf_weight_iterator_base.md#HfWeightIteratorBase.create), [`connect_rollout_engines_from_distributed`](update_weight_from_distributed.md#connect_rollout_engines_from_distributed), [`post_process_weights`](update_weight_from_distributed.md#post_process_weights), [`disconnect_rollout_engines_from_distributed`](update_weight_from_distributed.md#disconnect_rollout_engines_from_distributed), [`update_weights_from_distributed`](update_weight_from_distributed.md#update_weights_from_distributed), [`_send_to_colocated_engine`](update_weight_from_tensor.md#_send_to_colocated_engine)
- used by: [`update_weights`](../actor.md#MegatronTrainRayActor.update_weights), [`_active_model_tag`](../actor.md#MegatronTrainRayActor._active_model_tag)

## Functions
- `_send_to_colocated_engine(hf_named_tensors: list[tuple[str, torch.Tensor]], *, ipc_engine, ipc_gather_src, ipc_gather_group, weight_version)` — [`L171`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_tensor.py#L171)

