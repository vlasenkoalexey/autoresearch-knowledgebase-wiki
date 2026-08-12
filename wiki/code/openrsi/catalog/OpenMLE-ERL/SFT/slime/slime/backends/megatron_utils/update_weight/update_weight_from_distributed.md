---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.update_weight_from_distributed`/
symbols:
  UpdateWeightFromDistributed.update_weights: UpdateWeightFromDistributed#update_weights().
  UpdateWeightFromDistributed._group_name: UpdateWeightFromDistributed#_group_name.
  UpdateWeightFromDistributed._update_weight_from_distributed: UpdateWeightFromDistributed#_update_weight_from_distributed().
  UpdateWeightFromDistributed._update_bucket_weights_from_distributed: UpdateWeightFromDistributed#_update_bucket_weights_from_distributed().
  UpdateWeightFromDistributed._update_expert_bucket_weights_from_distributed: UpdateWeightFromDistributed#_update_expert_bucket_weights_from_distributed().
  UpdateWeightFromDistributed._update_expert_weight_from_distributed: UpdateWeightFromDistributed#_update_expert_weight_from_distributed().
  UpdateWeightFromDistributed.args: UpdateWeightFromDistributed#args.
  UpdateWeightFromDistributed._is_pp_src_rank: UpdateWeightFromDistributed#_is_pp_src_rank.
  UpdateWeightFromDistributed.rollout_engines: UpdateWeightFromDistributed#rollout_engines.
  UpdateWeightFromDistributed.quantization_config: UpdateWeightFromDistributed#quantization_config.
  connect_rollout_engines_from_distributed: connect_rollout_engines_from_distributed().
  post_process_weights: post_process_weights().
  UpdateWeightFromDistributed._model_update_groups: UpdateWeightFromDistributed#_model_update_groups.
  disconnect_rollout_engines_from_distributed: disconnect_rollout_engines_from_distributed().
  update_weights_from_distributed: update_weights_from_distributed().
  UpdateWeightFromDistributed: UpdateWeightFromDistributed#
  UpdateWeightFromDistributed.model: UpdateWeightFromDistributed#model.
  UpdateWeightFromDistributed.model_name: UpdateWeightFromDistributed#model_name.
  UpdateWeightFromDistributed.weight_version: UpdateWeightFromDistributed#weight_version.
  UpdateWeightFromDistributed.rollout_engine_lock: UpdateWeightFromDistributed#rollout_engine_lock.
  UpdateWeightFromDistributed.__init__: UpdateWeightFromDistributed#__init__().
  UpdateWeightFromDistributed.connect_rollout_engines: UpdateWeightFromDistributed#connect_rollout_engines().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py)

## Classes
### `UpdateWeightFromDistributed`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py:20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L20)
- doc: Update distributed engines via NCCL. Each PP rank: group "slime-pp_{pp_rank}",
- signature: `class UpdateWeightFromDistributed:`
- members:
  - `__init__(self, args: Namespace, model: Sequence[torch.nn.Module], weights_getter: Callable[[], Mapping[str, torch.Tensor]], *, model_name: str, quantization_config: dict[str, int | str | list[str]] | None)` — [`L26`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L26) — Initialize. Groups created in connect_rollout_engines.
  - `_update_bucket_weights_from_distributed(self, converted_named_tensors: list[tuple[str, torch.Tensor]], pbar: tqdm | None = None)` — [`L220`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L220) — Lock → broadcast → clear → unlock → pbar++. Lock prevents NCCL deadlock.
  - `_update_expert_bucket_weights_from_distributed(self, named_tensors: list[tuple[str, torch.Tensor]], pbar: tqdm | None = None)` — [`L182`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L182) — Gather EP → HF → broadcast. Clears buffer.
  - `_update_expert_weight_from_distributed(self, name: str, param: torch.nn.Parameter, named_tensors: list[tuple[str, torch.Tensor]], buffer_size: int, pbar: tqdm | None = None)` — [`L158`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L158) — Expert: gather TP → rm pad → buffer. EP gather + HF deferred. Threshold × EP size.
  - `_update_weight_from_distributed(self, name: str, param: torch.nn.Parameter, converted_named_tensors: list[tuple[str, torch.Tensor]], buffer_size: int, pbar: tqdm | None = None)` — [`L134`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L134) — Non-expert: gather TP → rm pad → HF → buffer (flush if full). All gather, PP source buffers.
  - `connect_rollout_engines(self, rollout_engines: Sequence[ActorHandle], rollout_engine_lock: ActorHandle)` — [`L45`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L45) — Create NCCL "slime-pp_{pp_rank}" if PP source (DP=TP=0). Lock prevents concurrent broadcasts.
  - `update_weights(self)` — [`L74`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L74) — Pause → flush → non-expert (TP) → expert (EP) → continue. Progress on PP source.
  - `args` — [`L38`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L38)
  - `model` — [`L39`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L39)
  - `model_name` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L40)
  - `quantization_config` — [`L41`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L41)
  - `rollout_engine_lock` — [`L52`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L52)
  - `rollout_engines` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L51)
  - `weight_version` — [`L42`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L42)
- protocol/private: `_group_name`[`L62`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L62), `_is_pp_src_rank`[`L57`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L57), `_model_update_groups`[`L43`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L43)
- uses (calls/refs, reference-scoped): [`get_gloo_group`](../../../utils/distributed_utils.md#get_gloo_group), [`convert_to_hf`](../megatron_to_hf/__init__.md#convert_to_hf), [`named_params_and_buffers`](common.md#named_params_and_buffers), [`connect_rollout_engines_from_distributed`](update_weight_from_distributed.md#connect_rollout_engines_from_distributed), [`post_process_weights`](update_weight_from_distributed.md#post_process_weights), [`all_gather_param`](common.md#all_gather_param), [`disconnect_rollout_engines_from_distributed`](update_weight_from_distributed.md#disconnect_rollout_engines_from_distributed), [`update_weights_from_distributed`](update_weight_from_distributed.md#update_weights_from_distributed)
- used by: [`_active_model_tag`](../actor.md#MegatronTrainRayActor._active_model_tag)

## Functions
- `connect_rollout_engines_from_distributed(args: Namespace, group_name: str, rollout_engines: Sequence[ActorHandle])` — [`L244`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L244) — Create NCCL group: training rank 0 + all engine GPUs. Blocks until joined.
- `disconnect_rollout_engines_from_distributed(args, group_name, model_update_groups, rollout_engines)` — [`L278`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L278) — Destroy NCCL on training and engines.
- `post_process_weights(restore_weights_before_load: bool, post_process_quantization: bool, rollout_engines: Sequence[ActorHandle])` — [`L317`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L317) — Trigger post-process for int4/fp4 quantization on all rollout engines.
- `update_weights_from_distributed(group_name: str, group: dist.ProcessGroup, weight_version: int, rollout_engines: Sequence[ActorHandle], converted_named_tensors: Sequence[tuple[str, torch.Tensor]])` — [`L287`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/update_weight_from_distributed.py#L287) — Send metadata (Ray), broadcast tensors (NCCL rank 0 → engines).

