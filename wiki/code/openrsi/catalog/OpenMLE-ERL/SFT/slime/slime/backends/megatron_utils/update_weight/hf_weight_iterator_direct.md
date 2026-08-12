---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.hf_weight_iterator_direct`/
symbols:
  _get_megatron_local_param_infos: _get_megatron_local_param_infos().
  _get_megatron_full_params: _get_megatron_full_params().
  HfWeightIteratorDirect._convert_to_hf_named_tensors: HfWeightIteratorDirect#_convert_to_hf_named_tensors().
  _get_megatron_local_param_info_buckets: _get_megatron_local_param_info_buckets().
  HfWeightIteratorDirect.megatron_local_param_info_buckets: HfWeightIteratorDirect#megatron_local_param_info_buckets.
  HfWeightIteratorDirect.get_hf_weight_chunks: HfWeightIteratorDirect#get_hf_weight_chunks().
  HfWeightIteratorDirect: HfWeightIteratorDirect#
  HfWeightIteratorDirect.__init__: HfWeightIteratorDirect#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py)

## Classes
### `HfWeightIteratorDirect`  ·  implements/extends HfWeightIteratorBase
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py:19`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L19)
- signature: `class HfWeightIteratorDirect(HfWeightIteratorBase):`
- members:
  - `get_hf_weight_chunks(self, megatron_local_weights)` — [`L24`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L24)
  - `megatron_local_param_info_buckets` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L22)
- protocol/private: `__init__`[`L20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L20), `_convert_to_hf_named_tensors`[`L35`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L35)
- uses (calls/refs, reference-scoped): [`_get_megatron_full_params`](hf_weight_iterator_direct.md#_get_megatron_full_params), [`convert_to_hf`](../megatron_to_hf/__init__.md#convert_to_hf), [`HfWeightIteratorBase`](hf_weight_iterator_base.md#HfWeightIteratorBase), [`_get_megatron_local_param_info_buckets`](hf_weight_iterator_direct.md#_get_megatron_local_param_info_buckets), [`ParamInfo`](../../../utils/types.md#ParamInfo), [`name`](../../../utils/types.md#ParamInfo.name), [`args`](hf_weight_iterator_base.md#HfWeightIteratorBase.args), [`model`](hf_weight_iterator_base.md#HfWeightIteratorBase.model), [`__init__`](hf_weight_iterator_base.md#HfWeightIteratorBase.__init__), [`quantization_config`](hf_weight_iterator_base.md#HfWeightIteratorBase.quantization_config), [`model_name`](hf_weight_iterator_base.md#HfWeightIteratorBase.model_name)
- used by: [`HfWeightIteratorBase`](hf_weight_iterator_base.md#HfWeightIteratorBase), [`create`](hf_weight_iterator_base.md#HfWeightIteratorBase.create), [`get_hf_weight_chunks`](hf_weight_iterator_base.md#HfWeightIteratorBase.get_hf_weight_chunks)

## Functions
- `_get_megatron_full_params(megatron_local_param_infos: Sequence[ParamInfo], megatron_local_weights)` — [`L44`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L44)
- `_get_megatron_local_param_info_buckets(args: Namespace, model: Sequence[torch.nn.Module])` — [`L108`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L108) — Partition params into buckets ≤ update_weight_buffer_size (with TP replication).
- `_get_megatron_local_param_infos(args: Namespace, model: Sequence[torch.nn.Module])` — [`L138`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_direct.py#L138) — Build global param metadata: collect → exchange PP/EP → resolve duplicates (MTP virtual PP)

