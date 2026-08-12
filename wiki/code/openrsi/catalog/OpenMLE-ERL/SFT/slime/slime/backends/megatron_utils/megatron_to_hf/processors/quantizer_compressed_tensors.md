---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.megatron_to_hf.processors.quantizer_compressed_tensors`/
symbols:
  WQLinear_GEMM.training: WQLinear_GEMM#training.
  WQLinear_GEMM.w_bit: WQLinear_GEMM#w_bit.
  pack_layer: pack_layer().
  WQLinear_GEMM.from_linear: WQLinear_GEMM#from_linear().
  quantize_params_compressed_tensors: quantize_params_compressed_tensors().
  quantize: quantize().
  WQLinear_GEMM.group_size: WQLinear_GEMM#group_size.
  WQLinear_GEMM.in_features: WQLinear_GEMM#in_features.
  WQLinear_GEMM.bias: WQLinear_GEMM#bias.
  pack_to_int32: pack_to_int32().
  round_to_quantized_type_dtype: round_to_quantized_type_dtype().
  logger: logger.
  __all__: __all__.
  WQLinear_GEMM: WQLinear_GEMM#
  WQLinear_GEMM.__init__: WQLinear_GEMM#__init__().
  WQLinear_GEMM.out_features: WQLinear_GEMM#out_features.
  if_quant: if_quant().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py)

## Classes
### `WQLinear_GEMM`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py:19`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L19)
- signature: `class WQLinear_GEMM(nn.Module):`
- members:
  - `from_linear(cls, linear, w_bit, group_size, init_only=False, scales=None, zeros=None)` — [`L73`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L73)
  - `bias` — [`L70`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L70)
  - `group_size` — [`L29`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L29)
  - `in_features` — [`L26`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L26)
  - `out_features` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L27)
  - `training` — [`L30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L30)
  - `w_bit` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L28)
- protocol/private: `__init__`[`L20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L20)

## Functions
- `if_quant(name, patterns)` — [`L226`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L226)
- `pack_layer(weight, group_size, sym=True)` — [`L233`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L233)
- `pack_to_int32(value, num_bits, packed_dim=1, sym=False)` — [`L135`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L135)
- `quantize(x, scale, zero_point, dtype=torch.int8)` — [`L195`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L195)
- `quantize_params_compressed_tensors(converted_named_params, quantization_config)` — [`L266`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L266)
- `round_to_quantized_type_dtype(tensor, dtype, cast_to_original_dtype=False)` — [`L181`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L181)

## Module values
- `__all__` — [`L16`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L16)
- `logger` — [`L13`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/processors/quantizer_compressed_tensors.py#L13)

