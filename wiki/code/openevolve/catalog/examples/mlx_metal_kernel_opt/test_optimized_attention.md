---
title: 'Module: examples/mlx_metal_kernel_opt/test_optimized_attention.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/test_optimized_attention.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.test_optimized_attention`/
symbols:
  run_comparison_test: run_comparison_test().
  main: main().
  run_mlx_lm_generation: run_mlx_lm_generation().
  find_best_program: find_best_program().
  load_custom_attention_class: load_custom_attention_class().
  apply_monkey_patch: apply_monkey_patch().
  remove_monkey_patch: remove_monkey_patch().
---
# Module: [`examples/mlx_metal_kernel_opt/test_optimized_attention.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py)

## Functions
- `apply_monkey_patch(custom_attention_class)` — [`L99`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L99) — Apply monkey patch to replace Qwen3 attention with custom implementation
- `find_best_program()` — [`L26`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L26) — Find the best_program.py file in the expected location
- `load_custom_attention_class(program_path: str)` — [`L50`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L50) — Load the CustomGQAAttention class from the evolved program
- `main()` — [`L439`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L439)
- `remove_monkey_patch(original_attention)` — [`L124`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L124) — Remove the monkey patch and restore original attention
- `run_comparison_test(prompt: str, custom_attention_class, max_tokens: int = 1000, debug: bool = False)` — [`L297`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L297) — Run comparison test between standard and optimized attention
- `run_mlx_lm_generation(prompt: str, max_tokens: int = 1000, model: str = "mlx-community/Qwen3-0.6B-bf16", debug: bool = False)` — [`L138`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/test_optimized_attention.py#L138) — Run mlx-lm generation and parse the output

