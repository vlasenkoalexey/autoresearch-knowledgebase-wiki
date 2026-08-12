---
title: 'Module: OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime_plugins.models.qwen3_5`/
symbols:
  Qwen3_5GatedDeltaNet.forward: Qwen3_5GatedDeltaNet#forward().
  Attention.hf_config: Attention#hf_config.
  Qwen3_5GatedDeltaNet.conv1d: Qwen3_5GatedDeltaNet#conv1d.
  Qwen3_5GatedDeltaNet.value_dim: Qwen3_5GatedDeltaNet#value_dim.
  Qwen3_5GatedDeltaNet.key_dim: Qwen3_5GatedDeltaNet#key_dim.
  Qwen3_5GatedDeltaNet.norm: Qwen3_5GatedDeltaNet#norm.
  Attention.linear_attn: Attention#linear_attn.
  Qwen3_5GatedDeltaNet.num_v_heads: Qwen3_5GatedDeltaNet#num_v_heads.
  get_qwen3_5_spec: get_qwen3_5_spec().
  Attention.input_layernorm: Attention#input_layernorm.
  Qwen3_5GatedDeltaNet.conv_dim: Qwen3_5GatedDeltaNet#conv_dim.
  Qwen3_5GatedDeltaNet.in_proj_b: Qwen3_5GatedDeltaNet#in_proj_b.
  Qwen3_5GatedDeltaNet.in_proj_a: Qwen3_5GatedDeltaNet#in_proj_a.
  Qwen3_5GatedDeltaNet.out_proj: Qwen3_5GatedDeltaNet#out_proj.
  Qwen3_5GatedDeltaNet.hidden_size: Qwen3_5GatedDeltaNet#hidden_size.
  Attention.hf_forward: Attention#hf_forward().
  Qwen3_5GatedDeltaNet.num_k_heads: Qwen3_5GatedDeltaNet#num_k_heads.
  Qwen3_5GatedDeltaNet.head_v_dim: Qwen3_5GatedDeltaNet#head_v_dim.
  Qwen3_5GatedDeltaNet.in_proj_qkv: Qwen3_5GatedDeltaNet#in_proj_qkv.
  Qwen3_5GatedDeltaNet.in_proj_z: Qwen3_5GatedDeltaNet#in_proj_z.
  Qwen3_5GatedDeltaNet.dt_bias: Qwen3_5GatedDeltaNet#dt_bias.
  Attention: Attention#
  Qwen3_5GatedDeltaNet.head_k_dim: Qwen3_5GatedDeltaNet#head_k_dim.
  Attention.__init__: Attention#__init__().
  _get_text_config: _get_text_config().
  _load_hf_config: _load_hf_config().
  Qwen3_5GatedDeltaNet: Qwen3_5GatedDeltaNet#
  Qwen3_5GatedDeltaNet.conv_kernel_size: Qwen3_5GatedDeltaNet#conv_kernel_size.
  Qwen3_5GatedDeltaNet.activation: Qwen3_5GatedDeltaNet#activation.
  Qwen3_5GatedDeltaNet.layer_norm_epsilon: Qwen3_5GatedDeltaNet#layer_norm_epsilon.
  Qwen3_5GatedDeltaNet.A_log: Qwen3_5GatedDeltaNet#A_log.
  Qwen3_5GatedDeltaNet.__init__: Qwen3_5GatedDeltaNet#__init__().
  Qwen3_5GatedDeltaNet.layer_idx: Qwen3_5GatedDeltaNet#layer_idx.
  Qwen3_5GatedDeltaNet.act: Qwen3_5GatedDeltaNet#act.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py)

## Classes
### `Attention`  ·  implements/extends HuggingfaceAttention
- def: [`OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py:166`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L166)
- signature: `class Attention(HuggingfaceAttention):`
- members:
  - `hf_forward(self, hidden_states, packed_seq_params)` — [`L198`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L198)
  - `hf_config` — [`L183`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L183)
  - `input_layernorm` — [`L192`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L192)
  - `linear_attn` — [`L186`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L186)
- protocol/private: `__init__`[`L167`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L167)
- uses (calls/refs, reference-scoped): [`HuggingfaceAttention`](hf_attention.md#HuggingfaceAttention), [`_get_text_config`](qwen3_5.md#_get_text_config), [`Qwen3_5GatedDeltaNet`](qwen3_5.md#Qwen3_5GatedDeltaNet), [`__init__`](hf_attention.md#HuggingfaceAttention.__init__), [`hf_layer_idx`](hf_attention.md#HuggingfaceAttention.hf_layer_idx)
- used by: [`get_qwen3_5_spec`](qwen3_5.md#get_qwen3_5_spec), [`HuggingfaceAttention`](hf_attention.md#HuggingfaceAttention), [`hf_forward`](hf_attention.md#HuggingfaceAttention.hf_forward)

### `Qwen3_5GatedDeltaNet`
- def: [`OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py:50`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L50)
- doc: Qwen3.5 GatedDeltaNet with varlen support.
- signature: `class Qwen3_5GatedDeltaNet(nn.Module):`
- members:
  - `forward(self, hidden_states: torch.Tensor, cu_seqlens: torch.Tensor = None)` — [`L105`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L105)
  - `A_log` — [`L93`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L93)
  - `act` — [`L70`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L70)
  - `activation` — [`L69`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L69)
  - `conv1d` — [`L75`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L75)
  - `conv_dim` — [`L74`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L74)
  - `conv_kernel_size` — [`L67`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L67)
  - `dt_bias` — [`L90`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L90)
  - `head_k_dim` — [`L62`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L62)
  - `head_v_dim` — [`L63`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L63)
  - `hidden_size` — [`L59`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L59)
  - `in_proj_a` — [`L87`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L87)
  - `in_proj_b` — [`L86`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L86)
  - `in_proj_qkv` — [`L84`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L84)
  - `in_proj_z` — [`L85`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L85)
  - `key_dim` — [`L64`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L64)
  - `layer_idx` — [`L68`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L68)
  - `layer_norm_epsilon` — [`L71`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L71)
  - `norm` — [`L95`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L95)
  - `num_k_heads` — [`L61`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L61)
  - `num_v_heads` — [`L60`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L60)
  - `out_proj` — [`L103`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L103)
  - `value_dim` — [`L65`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L65)
- protocol/private: `__init__`[`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L57)
- used by: [`linear_attn`](qwen3_5.md#Attention.linear_attn)

## Functions
- `_get_text_config(hf_config)` — [`L42`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L42) — Extract text config from a VLM config if needed.
- `_load_hf_config(checkpoint_path)` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L15) — Load HF config, handling cases where transformers doesn't know the model type.
- `get_qwen3_5_spec(args, config, vp_stage)` — [`L207`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime_plugins/models/qwen3_5.py#L207)

