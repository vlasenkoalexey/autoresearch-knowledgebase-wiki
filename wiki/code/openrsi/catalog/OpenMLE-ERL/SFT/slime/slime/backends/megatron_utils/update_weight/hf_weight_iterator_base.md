---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.hf_weight_iterator_base`/HfWeightIteratorBase#
symbols:
  HfWeightIteratorBase: ''
  HfWeightIteratorBase.create: create().
  HfWeightIteratorBase.args: args.
  HfWeightIteratorBase.get_hf_weight_chunks: get_hf_weight_chunks().
  HfWeightIteratorBase.model: model.
  HfWeightIteratorBase.__init__: __init__().
  HfWeightIteratorBase.quantization_config: quantization_config.
  HfWeightIteratorBase.model_name: model_name.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py)

## Classes
### `HfWeightIteratorBase`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py:4`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L4)
- signature: `class HfWeightIteratorBase(ABC):`
- members:
  - `create(args, model, **kwargs)` — [`L6`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L6)
  - `get_hf_weight_chunks(self, megatron_local_weights)` — [`L24`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L24) — Mental model of the API:
  - `args` — [`L18`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L18)
  - `model` — [`L19`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L19)
  - `model_name` — [`L20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L20)
  - `quantization_config` — [`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L21)
- protocol/private: `__init__`[`L17`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_base.py#L17)
- uses (calls/refs, reference-scoped): [`get_hf_weight_chunks`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge.get_hf_weight_chunks), [`get_hf_weight_chunks`](hf_weight_iterator_direct.md#HfWeightIteratorDirect.get_hf_weight_chunks), [`HfWeightIteratorBridge`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge), [`HfWeightIteratorDirect`](hf_weight_iterator_direct.md#HfWeightIteratorDirect)
- used by: [`get_hf_weight_chunks`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge.get_hf_weight_chunks), [`_convert_to_hf_named_tensors`](hf_weight_iterator_direct.md#HfWeightIteratorDirect._convert_to_hf_named_tensors), [`_hf_weight_iterator`](update_weight_from_tensor.md#UpdateWeightFromTensor._hf_weight_iterator), [`megatron_local_param_info_buckets`](hf_weight_iterator_direct.md#HfWeightIteratorDirect.megatron_local_param_info_buckets), [`HfWeightIteratorBridge`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge), [`HfWeightIteratorDirect`](hf_weight_iterator_direct.md#HfWeightIteratorDirect), [`_bridge`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge._bridge), [`__init__`](hf_weight_iterator_bridge.md#HfWeightIteratorBridge.__init__), [`__init__`](hf_weight_iterator_direct.md#HfWeightIteratorDirect.__init__)

