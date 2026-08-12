---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.hf_weight_iterator_bridge`/
symbols:
  HfWeightIteratorBridge.get_hf_weight_chunks: HfWeightIteratorBridge#get_hf_weight_chunks().
  _process_conversion_tasks: _process_conversion_tasks().
  _MapWithLen.__iter__: _MapWithLen#__iter__().
  HfWeightIteratorBridge: HfWeightIteratorBridge#
  HfWeightIteratorBridge._bridge: HfWeightIteratorBridge#_bridge.
  HfWeightIteratorBridge.__init__: HfWeightIteratorBridge#__init__().
  _MapWithLen.__len__: _MapWithLen#__len__().
  _MapWithLen.xs: _MapWithLen#xs.
  _process_conversion_tasks._handle_one: _process_conversion_tasks()._handle_one().
  _MapWithLen.fn: _MapWithLen#fn.
  _MapWithLen: _MapWithLen#
  _MapWithLen.__init__: _MapWithLen#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py)

## Classes
### `HfWeightIteratorBridge`  ·  implements/extends HfWeightIteratorBase
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py:12`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L12)
- signature: `class HfWeightIteratorBridge(HfWeightIteratorBase):`
- members:
  - `get_hf_weight_chunks(self, megatron_local_weights)` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L22)
- protocol/private: `__init__`[`L13`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L13), `_bridge`[`L20`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L20)
- uses (calls/refs, reference-scoped): [`HfWeightIteratorBase`](hf_weight_iterator_base.md#HfWeightIteratorBase), [`quantize_params`](../megatron_to_hf/processors/__init__.md#quantize_params), [`_process_conversion_tasks`](hf_weight_iterator_bridge.md#_process_conversion_tasks), [`args`](hf_weight_iterator_base.md#HfWeightIteratorBase.args), [`strip_param_name_prefix`](../misc_utils.md#strip_param_name_prefix), [`chunk_named_params_by_size`](../../../utils/misc.md#chunk_named_params_by_size), [`postprocess_hf_param`](../megatron_to_hf/__init__.md#postprocess_hf_param), [`model`](hf_weight_iterator_base.md#HfWeightIteratorBase.model), [`patch_megatron_model`](../../../utils/megatron_bridge_utils.md#patch_megatron_model), [`__init__`](hf_weight_iterator_base.md#HfWeightIteratorBase.__init__), [`quantization_config`](hf_weight_iterator_base.md#HfWeightIteratorBase.quantization_config)
- used by: [`HfWeightIteratorBase`](hf_weight_iterator_base.md#HfWeightIteratorBase), [`create`](hf_weight_iterator_base.md#HfWeightIteratorBase.create), [`get_hf_weight_chunks`](hf_weight_iterator_base.md#HfWeightIteratorBase.get_hf_weight_chunks)

### `_MapWithLen`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py:75`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L75)
- members:
  - `fn` — [`L77`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L77)
  - `xs` — [`L78`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L78)
- protocol/private: `__init__`[`L76`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L76), `__iter__`[`L83`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L83), `__len__`[`L80`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L80)
- used by: [`_process_conversion_tasks`](hf_weight_iterator_bridge.md#_process_conversion_tasks)

## Functions
- `_handle_one(task)` — [`L59`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L59)
- `_process_conversion_tasks(vanilla_conversion_tasks, new_weight_dict)` — [`L58`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/hf_weight_iterator_bridge.py#L58)

