---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.benchmark`/BenchmarkConfig#
symbols:
  BenchmarkConfig.to_cfg_list: to_cfg_list().
  BenchmarkConfig: ''
  BenchmarkConfig.validate: validate().
  BenchmarkConfig.task_overrides: task_overrides.
  BenchmarkConfig.name: name.
  BenchmarkConfig.tasks: tasks.
  BenchmarkConfig.overrides: overrides.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py)

## Classes
### `BenchmarkConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py:20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L20)
- signature: `class BenchmarkConfig(BaseConfig):`
- members:
  - `to_cfg_list(self)` — [`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L52) — Convert the benchmark configuration to an iterator of task configurations.
  - `validate(self)` — [`L49`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L49)
  - `name` — [`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L21)
  - `overrides` — [`L35`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L35)
  - `task_overrides` — [`L42`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L42)
  - `tasks` — [`L28`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/benchmark.py#L28)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`MLEBenchTaskConfig`](task/mlebench.md#MLEBenchTaskConfig), [`name`](task/base.md#TaskConfig.name), [`benchmark`](task/mlebench.md#MLEBenchTaskConfig.benchmark)
- used by: [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`_main`](../main_runner_job_array.md#_main), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`benchmark`](runner.md#RunnerConfig.benchmark)

