---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.flops_utils`/calculate_
symbols:
  calculate_layer_flops: layer_flops().
  calculate_fwd_flops: fwd_flops().
  calculate_lm_head_flops: lm_head_flops().
  calculate_qkv_projection_flops: qkv_projection_flops().
  calculate_attention_flops: attention_flops().
  calculate_output_flops: output_flops().
  calculate_mlp_flops: mlp_flops().
  calculate_embedding_flops: embedding_flops().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py)

## Functions
- `calculate_attention_flops(args, seqlen, num_attention_heads)` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L35)
- `calculate_embedding_flops(seqlen, hidden_size)` — [`L1`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L1)
- `calculate_fwd_flops(seqlens, args)` — [`L66`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L66)
- `calculate_layer_flops(args, seqlen, hidden_size, num_attention_heads, num_query_groups, ffn_hidden_size)` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L57)
- `calculate_lm_head_flops(seqlen, hidden_size, vocab_size)` — [`L5`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L5)
- `calculate_mlp_flops(seqlen, hidden_size, ffn_hidden_size)` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L53)
- `calculate_output_flops(seqlen, hidden_size)` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L49)
- `calculate_qkv_projection_flops(args, seqlen, hidden_size, num_attention_heads, num_query_groups)` — [`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/flops_utils.py#L9)

