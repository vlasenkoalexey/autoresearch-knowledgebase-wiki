---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.megatron_to_hf.qwen3_5_moe`/
symbols:
  convert_qwen3_5_moe_to_hf: convert_qwen3_5_moe_to_hf().
  _convert_full_attention_qkv: _convert_full_attention_qkv().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py)

## Functions
- `_convert_full_attention_qkv(args, layer_idx: str, param: torch.Tensor)` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py#L16) — Split fused QKV weights using the gated Qwen3.5 Q-projection layout.
- `convert_qwen3_5_moe_to_hf(args, name: str, param: torch.Tensor)` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/megatron_to_hf/qwen3_5_moe.py#L40) — Map one Megatron parameter to one or more Qwen3.5 HF parameters.

