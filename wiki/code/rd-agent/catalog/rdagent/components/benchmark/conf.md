---
title: 'Module: rdagent/components/benchmark/conf.py'
type: catalog
provenance: extracted
module: rdagent/components/benchmark/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.benchmark.conf`/
symbols:
  BenchmarkSettings: BenchmarkSettings#
  BenchmarkSettings.bench_data_path: BenchmarkSettings#bench_data_path.
  DIRNAME: DIRNAME.
  BenchmarkSettings.bench_test_round: BenchmarkSettings#bench_test_round.
  BenchmarkSettings.bench_method_cls: BenchmarkSettings#bench_method_cls.
  BenchmarkSettings.bench_method_extra_kwargs: BenchmarkSettings#bench_method_extra_kwargs.
  BenchmarkSettings.Config: BenchmarkSettings#Config#
  BenchmarkSettings.Config.env_prefix: BenchmarkSettings#Config#env_prefix.
  BenchmarkSettings.bench_test_case_n: BenchmarkSettings#bench_test_case_n.
  BenchmarkSettings.bench_result_path: BenchmarkSettings#bench_result_path.
---
# Module: [`rdagent/components/benchmark/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py)

## Classes
### `BenchmarkSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/components/benchmark/conf.py:10`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L10)
- signature: `class BenchmarkSettings(ExtendedBaseSettings):`
- members:
  - `bench_data_path` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L15) — ---
  - `bench_method_cls` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L24) — ---
  - `bench_method_extra_kwargs` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L27) — ---
  - `bench_result_path` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L32) — ---
  - `bench_test_case_n` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L21) — ---
  - `bench_test_round` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L18) — ---
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings)  (1 test-only)
- used by: [`ExtendedBaseSettings`](../../core/conf.md#ExtendedBaseSettings)  (5 test-only)

### `Config`
- def: [`rdagent/components/benchmark/conf.py:11`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L11)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L12`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L12)

## Module values
- `DIRNAME` — [`L7`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/conf.py#L7)

