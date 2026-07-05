---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks`/
symbols:
  BENCHMARKS.BENCHMARKS: BENCHMARKS.BENCHMARKS.
  get_evaluator: get_evaluator().
  BenchmarkConfig: BenchmarkConfig#
  get_benchmark: get_benchmark().
  BenchmarkConfig.data_module: BenchmarkConfig#data_module.
  BenchmarkConfig.evaluator_class: BenchmarkConfig#evaluator_class.
  BenchmarkConfig.id: BenchmarkConfig#id.
  BenchmarkConfig.description: BenchmarkConfig#description.
  BenchmarkConfig.eval_config: BenchmarkConfig#eval_config.
  BenchmarkConfig.expose_files: BenchmarkConfig#expose_files.
  BENCHMARKS_DIR: BENCHMARKS_DIR.
  BenchmarkConfig.bench_dir: BenchmarkConfig#bench_dir.
  list_benchmarks: list_benchmarks().
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py)

## Classes
### `BenchmarkConfig`
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py:19`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L19)
- doc: Benchmark 配置
- signature: `class BenchmarkConfig:`
- members:
  - `bench_dir` — [`L34`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L34)
  - `data_module` — [`L28`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L28)
  - `description` — [`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L29)
  - `eval_config` — [`L30`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L30)
  - `evaluator_class` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L27)
  - `expose_files` — [`L31`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L31)
  - `id` — [`L26`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L26)
- used by: [`download_data`](../core/utils.md#download_data)  (4 test-only)

## Functions
- `get_benchmark(benchmark_id: str)` — [`L114`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L114) — 获取 benchmark 配置
- `get_evaluator(benchmark_id: str)` — [`L122`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L122) — 获取 benchmark 的评测器实例
- `list_benchmarks()` — [`L134`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L134) — 列出所有可用的 benchmark

## Module values
- `BENCHMARKS` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L38)
- `BENCHMARKS_DIR` — [`L15`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/__init__.py#L15)

