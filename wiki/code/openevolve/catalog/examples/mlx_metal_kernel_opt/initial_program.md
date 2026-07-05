---
title: 'Module: examples/mlx_metal_kernel_opt/initial_program.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.initial_program`/
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
# Module: [`examples/mlx_metal_kernel_opt/initial_program.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py)

## Classes
### `CustomGQAAttention`
- def: [`examples/mlx_metal_kernel_opt/initial_program.py:241`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L241)
- doc: Qwen3 attention module with custom Metal kernel optimization.
- signature: `class CustomGQAAttention(nn.Module):`
- members:
  - `k_norm` — [`L268`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L268)
  - `k_proj` — [`L262`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L262)
  - `n_heads` — [`L254`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L254)
  - `n_kv_heads` — [`L256`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L256)
  - `o_proj` — [`L264`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L264)
  - `q_norm` — [`L267`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L267)
  - `q_proj` — [`L261`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L261)
  - `rope` — [`L274`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L274)
  - `scale` — [`L258`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L258)
  - `v_proj` — [`L263`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L263)
- protocol/private: `__call__`[`L290`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L290), `__init__`[`L249`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L249)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

### `MockArgs`
- def: [`examples/mlx_metal_kernel_opt/initial_program.py:432`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L432)
- signature: `class MockArgs:`
- members:
  - `head_dim` — [`L370`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L370)
  - `head_dim` — [`L436`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L436)
  - `hidden_size` — [`L367`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L367)
  - `hidden_size` — [`L433`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L433)
  - `max_position_embeddings` — [`L374`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L374)
  - `max_position_embeddings` — [`L440`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L440)
  - `num_attention_heads` — [`L368`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L368)
  - `num_attention_heads` — [`L434`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L434)
  - `num_key_value_heads` — [`L369`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L369)
  - `num_key_value_heads` — [`L435`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L435)
  - `rms_norm_eps` — [`L371`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L371)
  - `rms_norm_eps` — [`L437`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L437)
  - `rope_scaling` — [`L373`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L373)
  - `rope_scaling` — [`L439`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L439)
  - `rope_theta` — [`L372`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L372)
  - `rope_theta` — [`L438`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L438)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

## Functions
- `apply_optimization_hook()` — [`L329`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L329) — Apply the Metal kernel optimized attention
- `benchmark_metal_gqa_optimization()` — [`L360`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L360) — Benchmark Metal kernel optimized GQA attention against MLX baseline.
- `create_metal_qwen3_optimization_hook()` — [`L324`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L324) — Create hooks to replace Qwen3's attention with Metal kernel optimized version.
- `qwen3_custom_gqa_attention(queries, keys, values, scale=1, mask=None)` — [`L24`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L24) — Custom Metal kernel implementation for Qwen3 GQA attention.
- `remove_optimization_hook(original_attention)` — [`L347`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L347) — Remove the optimization hook
- `test_metal_gqa_correctness()` — [`L422`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/initial_program.py#L422) — Test that Metal kernel implementation produces correct results.

