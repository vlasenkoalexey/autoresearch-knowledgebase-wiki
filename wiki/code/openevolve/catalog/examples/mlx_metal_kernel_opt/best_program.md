---
title: 'Module: examples/mlx_metal_kernel_opt/best_program.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.best_program`/
symbols:
  CustomGQAAttention.__call__: CustomGQAAttention#__call__().
  CustomGQAAttention.rope: CustomGQAAttention#rope.
  test_metal_gqa_correctness: test_metal_gqa_correctness().
  create_metal_qwen3_optimization_hook: create_metal_qwen3_optimization_hook().
  benchmark_metal_gqa_optimization.MockArgs.max_position_embeddings: benchmark_metal_gqa_optimization().MockArgs#max_position_embeddings.
  test_metal_gqa_correctness.MockArgs.max_position_embeddings: test_metal_gqa_correctness().MockArgs#max_position_embeddings.
  create_metal_qwen3_optimization_hook.apply_optimization_hook: create_metal_qwen3_optimization_hook().apply_optimization_hook().
  CustomGQAAttention: CustomGQAAttention#
  qwen3_custom_gqa_attention: qwen3_custom_gqa_attention().
  CustomGQAAttention.n_kv_heads: CustomGQAAttention#n_kv_heads.
  CustomGQAAttention.n_heads: CustomGQAAttention#n_heads.
  CustomGQAAttention.scale: CustomGQAAttention#scale.
  CustomGQAAttention.q_proj: CustomGQAAttention#q_proj.
  CustomGQAAttention.k_proj: CustomGQAAttention#k_proj.
  CustomGQAAttention.v_proj: CustomGQAAttention#v_proj.
  CustomGQAAttention.o_proj: CustomGQAAttention#o_proj.
  CustomGQAAttention.q_norm: CustomGQAAttention#q_norm.
  CustomGQAAttention.k_norm: CustomGQAAttention#k_norm.
  create_metal_qwen3_optimization_hook.remove_optimization_hook: create_metal_qwen3_optimization_hook().remove_optimization_hook().
  benchmark_metal_gqa_optimization: benchmark_metal_gqa_optimization().
  benchmark_metal_gqa_optimization.MockArgs: benchmark_metal_gqa_optimization().MockArgs#
  test_metal_gqa_correctness.MockArgs: test_metal_gqa_correctness().MockArgs#
  CustomGQAAttention.__init__: CustomGQAAttention#__init__().
  benchmark_metal_gqa_optimization.MockArgs.hidden_size: benchmark_metal_gqa_optimization().MockArgs#hidden_size.
  benchmark_metal_gqa_optimization.MockArgs.num_attention_heads: benchmark_metal_gqa_optimization().MockArgs#num_attention_heads.
  benchmark_metal_gqa_optimization.MockArgs.num_key_value_heads: benchmark_metal_gqa_optimization().MockArgs#num_key_value_heads.
  benchmark_metal_gqa_optimization.MockArgs.head_dim: benchmark_metal_gqa_optimization().MockArgs#head_dim.
  benchmark_metal_gqa_optimization.MockArgs.rms_norm_eps: benchmark_metal_gqa_optimization().MockArgs#rms_norm_eps.
  benchmark_metal_gqa_optimization.MockArgs.rope_theta: benchmark_metal_gqa_optimization().MockArgs#rope_theta.
  benchmark_metal_gqa_optimization.MockArgs.rope_scaling: benchmark_metal_gqa_optimization().MockArgs#rope_scaling.
  test_metal_gqa_correctness.MockArgs.hidden_size: test_metal_gqa_correctness().MockArgs#hidden_size.
  test_metal_gqa_correctness.MockArgs.num_attention_heads: test_metal_gqa_correctness().MockArgs#num_attention_heads.
  test_metal_gqa_correctness.MockArgs.num_key_value_heads: test_metal_gqa_correctness().MockArgs#num_key_value_heads.
  test_metal_gqa_correctness.MockArgs.head_dim: test_metal_gqa_correctness().MockArgs#head_dim.
  test_metal_gqa_correctness.MockArgs.rms_norm_eps: test_metal_gqa_correctness().MockArgs#rms_norm_eps.
  test_metal_gqa_correctness.MockArgs.rope_theta: test_metal_gqa_correctness().MockArgs#rope_theta.
  test_metal_gqa_correctness.MockArgs.rope_scaling: test_metal_gqa_correctness().MockArgs#rope_scaling.
---
# Module: [`examples/mlx_metal_kernel_opt/best_program.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py)

## Classes
### `CustomGQAAttention`
- def: [`examples/mlx_metal_kernel_opt/best_program.py:244`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L244)
- doc: Qwen3 attention module with custom Metal kernel optimization.
- signature: `class CustomGQAAttention(nn.Module):`
- members:
  - `k_norm` — [`L271`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L271)
  - `k_proj` — [`L265`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L265)
  - `n_heads` — [`L257`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L257)
  - `n_kv_heads` — [`L259`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L259)
  - `o_proj` — [`L267`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L267)
  - `q_norm` — [`L270`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L270)
  - `q_proj` — [`L264`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L264)
  - `rope` — [`L277`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L277)
  - `scale` — [`L261`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L261)
  - `v_proj` — [`L266`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L266)
- protocol/private: `__call__`[`L293`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L293), `__init__`[`L252`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L252)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

### `MockArgs`
- def: [`examples/mlx_metal_kernel_opt/best_program.py:435`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L435)
- signature: `class MockArgs:`
- members:
  - `head_dim` — [`L373`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L373)
  - `head_dim` — [`L439`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L439)
  - `hidden_size` — [`L370`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L370)
  - `hidden_size` — [`L436`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L436)
  - `max_position_embeddings` — [`L377`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L377)
  - `max_position_embeddings` — [`L443`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L443)
  - `num_attention_heads` — [`L371`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L371)
  - `num_attention_heads` — [`L437`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L437)
  - `num_key_value_heads` — [`L372`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L372)
  - `num_key_value_heads` — [`L438`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L438)
  - `rms_norm_eps` — [`L374`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L374)
  - `rms_norm_eps` — [`L440`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L440)
  - `rope_scaling` — [`L376`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L376)
  - `rope_scaling` — [`L442`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L442)
  - `rope_theta` — [`L375`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L375)
  - `rope_theta` — [`L441`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L441)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

## Functions
- `apply_optimization_hook()` — [`L332`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L332) — Apply the Metal kernel optimized attention
- `benchmark_metal_gqa_optimization()` — [`L363`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L363) — Benchmark Metal kernel optimized GQA attention against MLX baseline.
- `create_metal_qwen3_optimization_hook()` — [`L327`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L327) — Create hooks to replace Qwen3's attention with Metal kernel optimized version.
- `qwen3_custom_gqa_attention(queries, keys, values, scale=1, mask=None)` — [`L24`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L24) — Custom Metal kernel implementation for Qwen3 GQA attention.
- `remove_optimization_hook(original_attention)` — [`L350`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L350) — Remove the optimization hook
- `test_metal_gqa_correctness()` — [`L425`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/best_program.py#L425) — Test that Metal kernel implementation produces correct results.

