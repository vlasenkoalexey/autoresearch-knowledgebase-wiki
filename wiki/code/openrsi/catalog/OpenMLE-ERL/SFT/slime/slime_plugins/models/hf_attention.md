---
title: 'Module: OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime_plugins.models.hf_attention`/HuggingfaceAttention#
symbols:
  HuggingfaceAttention.forward: forward().
  HuggingfaceAttention: ''
  HuggingfaceAttention.hf_config: hf_config.
  HuggingfaceAttention.hf_forward: hf_forward().
  HuggingfaceAttention.args: args.
  HuggingfaceAttention.__init__: __init__().
  HuggingfaceAttention.hf_layer_idx: hf_layer_idx.
  HuggingfaceAttention.config: config.
  HuggingfaceAttention.layer_number: layer_number.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py)

## Classes
### `HuggingfaceAttention`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py:12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L12)
- doc: Attention layer abstract class.
- signature: `class HuggingfaceAttention(MegatronModule, ABC):`
- members:
  - `forward(self, hidden_states: torch.Tensor, attention_mask: torch.Tensor, key_value_states: torch.Tensor | None = None, inference_context: BaseInferenceContext | None = None, rotary_pos_emb: torch.Tensor | tuple[torch.Tensor, torch.Tensor] | None = None, rotary_pos_cos: torch.Tensor | None = None, rotary_pos_sin: torch.Tensor | None = None, rotary_pos_cos_sin: torch.Tensor | None = None, attention_bias: torch.Tensor | None = None, packed_seq_params: PackedSeqParams | None = None, sequence_len_offset: int | None = None, *, inference_params: BaseInferenceContext | None = None)` — [`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L37)
  - `hf_forward(self, hidden_states, packed_seq_params)` — [`L114`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L114) — Huggingface forward function
  - `args` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L28)
  - `config` — [`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L29)
  - `hf_config` — [`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L33)
  - `hf_layer_idx` — [`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L32)
  - `layer_number` — [`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L31)
- protocol/private: `__init__`[`L19`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/hf_attention.py#L19)
- uses (calls/refs, reference-scoped): [`hf_forward`](qwen3_5.md#Attention.hf_forward), [`Attention`](qwen3_5.md#Attention)
- used by: [`linear_attn`](qwen3_5.md#Attention.linear_attn), [`Attention`](qwen3_5.md#Attention), [`__init__`](qwen3_5.md#Attention.__init__)

