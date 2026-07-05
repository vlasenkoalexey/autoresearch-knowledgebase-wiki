---
title: 'Module: examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.qwen3_benchmark_suite`/
symbols:
  Qwen3BenchmarkSuite.run_single_benchmark: Qwen3BenchmarkSuite#run_single_benchmark().
  BenchmarkConfig.name: BenchmarkConfig#name.
  Qwen3BenchmarkSuite._parse_benchmark_output: Qwen3BenchmarkSuite#_parse_benchmark_output().
  Qwen3BenchmarkSuite.save_results: Qwen3BenchmarkSuite#save_results().
  BenchmarkConfig.prompt: BenchmarkConfig#prompt.
  BenchmarkConfig: BenchmarkConfig#
  Qwen3BenchmarkSuite.create_benchmark_configs: Qwen3BenchmarkSuite#create_benchmark_configs().
  Qwen3BenchmarkSuite._result_to_dict: Qwen3BenchmarkSuite#_result_to_dict().
  BenchmarkConfig.max_tokens: BenchmarkConfig#max_tokens.
  BenchmarkConfig.description: BenchmarkConfig#description.
  Qwen3BenchmarkSuite.run_full_benchmark_suite: Qwen3BenchmarkSuite#run_full_benchmark_suite().
  Qwen3BenchmarkSuite.print_summary_table: Qwen3BenchmarkSuite#print_summary_table().
  BenchmarkResult.decode_tokens_per_sec: BenchmarkResult#decode_tokens_per_sec.
  BenchmarkResult: BenchmarkResult#
  BenchmarkResult.prefill_tokens_per_sec: BenchmarkResult#prefill_tokens_per_sec.
  BenchmarkResult.peak_memory_gb: BenchmarkResult#peak_memory_gb.
  Qwen3BenchmarkSuite.generate_summary: Qwen3BenchmarkSuite#generate_summary().
  BenchmarkResult.name: BenchmarkResult#name.
  Qwen3BenchmarkSuite: Qwen3BenchmarkSuite#
  BenchmarkResult.total_time_sec: BenchmarkResult#total_time_sec.
  main: main().
  BenchmarkResult.total_tokens_per_sec: BenchmarkResult#total_tokens_per_sec.
  BenchmarkResult.generated_tokens: BenchmarkResult#generated_tokens.
  Qwen3BenchmarkSuite.results: Qwen3BenchmarkSuite#results.
  BenchmarkResult.prompt_tokens: BenchmarkResult#prompt_tokens.
  Qwen3BenchmarkSuite._create_very_long_context_prompt: Qwen3BenchmarkSuite#_create_very_long_context_prompt().
  Qwen3BenchmarkSuite.hook_program_path: Qwen3BenchmarkSuite#hook_program_path.
  Qwen3BenchmarkSuite.model_path: Qwen3BenchmarkSuite#model_path.
  Qwen3BenchmarkSuite._create_maximum_context_prompt: Qwen3BenchmarkSuite#_create_maximum_context_prompt().
  BenchmarkResult.prompt: BenchmarkResult#prompt.
  BenchmarkResult.generated_text: BenchmarkResult#generated_text.
  Qwen3BenchmarkSuite._create_long_context_prompt: Qwen3BenchmarkSuite#_create_long_context_prompt().
  Qwen3BenchmarkSuite._create_medium_context_prompt: Qwen3BenchmarkSuite#_create_medium_context_prompt().
  Qwen3BenchmarkSuite._create_progressive_context_prompt: Qwen3BenchmarkSuite#_create_progressive_context_prompt().
  Qwen3BenchmarkSuite.__init__: Qwen3BenchmarkSuite#__init__().
---
# Module: [`examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py)

## Classes
### `BenchmarkConfig`
- def: [`examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py:45`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L45)
- doc: Benchmark configuration
- signature: `class BenchmarkConfig:`
- members:
  - `description` — [`L51`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L51)
  - `max_tokens` — [`L50`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L50)
  - `name` — [`L48`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L48)
  - `prompt` — [`L49`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L49)
- used by: (9 test-only callers)

### `BenchmarkResult`
- def: [`examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py:29`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L29)
- doc: Single benchmark result
- signature: `class BenchmarkResult:`
- members:
  - `decode_tokens_per_sec` — [`L36`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L36)
  - `generated_text` — [`L41`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L41)
  - `generated_tokens` — [`L34`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L34)
  - `name` — [`L32`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L32)
  - `peak_memory_gb` — [`L38`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L38)
  - `prefill_tokens_per_sec` — [`L35`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L35)
  - `prompt` — [`L40`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L40)
  - `prompt_tokens` — [`L33`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L33)
  - `total_time_sec` — [`L39`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L39)
  - `total_tokens_per_sec` — [`L37`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L37)
- used by: (11 test-only callers)

### `Qwen3BenchmarkSuite`
- def: [`examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py:54`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L54)
- doc: Comprehensive benchmark suite for Qwen3-0.6B Metal kernel optimization
- signature: `class Qwen3BenchmarkSuite:`
- members:
  - `_create_long_context_prompt(self)` — [`L267`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L267) — Create long context prompt
  - `_create_maximum_context_prompt(self)` — [`L409`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L409) — Create maximum length context prompt for stress testing
  - `_create_medium_context_prompt(self)` — [`L254`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L254) — Create medium-length context prompt
  - `_create_progressive_context_prompt(self)` — [`L370`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L370) — Create prompt that builds context progressively
  - `_create_very_long_context_prompt(self)` — [`L304`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L304) — Create very long context prompt to test KV cache scaling
  - `_parse_benchmark_output(self, stdout: str, config: BenchmarkConfig, total_time: float)` — [`L745`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L745) — Parse mlx-lm output to extract performance metrics
  - `_result_to_dict(self, result: BenchmarkResult)` — [`L952`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L952) — Convert BenchmarkResult to dictionary
  - `create_benchmark_configs(self)` — [`L68`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L68) — Create comprehensive benchmark configurations
  - `generate_summary(self, results: List[BenchmarkResult])` — [`L838`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L838) — Generate benchmark summary statistics
  - `print_summary_table(self)` — [`L967`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L967) — Print a summary table of all results
  - `run_full_benchmark_suite(self)` — [`L810`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L810) — Run the complete benchmark suite
  - `run_single_benchmark(self, config: BenchmarkConfig)` — [`L558`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L558) — Run a single benchmark configuration with proper warmup
  - `save_results(self, results: List[BenchmarkResult], summary: Dict)` — [`L890`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L890) — Save benchmark results to files
  - `hook_program_path` — [`L65`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L65)
  - `model_path` — [`L62`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L62)
  - `results` — [`L66`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L66)
- protocol/private: `__init__`[`L57`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L57)
- uses (calls/refs, reference-scoped): (16 test-only callers)
- used by: (9 test-only callers)

## Functions
- `main()` — [`L1004`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/qwen3_benchmark_suite.py#L1004) — Run the complete benchmark suite

