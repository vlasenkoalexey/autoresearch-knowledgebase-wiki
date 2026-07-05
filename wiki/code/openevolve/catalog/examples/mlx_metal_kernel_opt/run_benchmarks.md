---
title: 'Module: examples/mlx_metal_kernel_opt/run_benchmarks.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/run_benchmarks.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.run_benchmarks`/
symbols:
  run_compare_benchmarks: run_compare_benchmarks().
  main: main().
  run_optimized_benchmark: run_optimized_benchmark().
  analyze_comparison_results: analyze_comparison_results().
  save_comparison_results: save_comparison_results().
  print_comparison_summary: print_comparison_summary().
---
# Module: [`examples/mlx_metal_kernel_opt/run_benchmarks.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py)

## Functions
- `analyze_comparison_results(standard_results, optimized_results, model_name)` — [`L172`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L172) — Analyze and compare the benchmark results.
- `main()` — [`L561`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L561)
- `print_comparison_summary(comparison_results)` — [`L415`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L415) — Print a comprehensive comparison summary.
- `run_compare_benchmarks(args)` — [`L24`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L24) — Run comprehensive comparison between standard and optimized attention.
- `run_optimized_benchmark(args, original_dir)` — [`L102`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L102) — Run benchmark with the optimized attention from best_program.py.
- `save_comparison_results(comparison_results, output_dir)` — [`L332`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/run_benchmarks.py#L332) — Save detailed comparison results to files.

