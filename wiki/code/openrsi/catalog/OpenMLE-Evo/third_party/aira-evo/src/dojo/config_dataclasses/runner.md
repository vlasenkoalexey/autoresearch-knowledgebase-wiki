---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.runner`/RunnerConfig#
symbols:
  RunnerConfig: ''
  RunnerConfig.id: id().
  RunnerConfig.launcher: launcher.
  RunnerConfig.validate: validate().
  RunnerConfig.save: save().
  RunnerConfig.logger: logger.
  RunnerConfig.metadata: metadata.
  RunnerConfig.solver: solver.
  RunnerConfig.interpreter: interpreter.
  RunnerConfig.benchmark: benchmark.
  RunnerConfig.vars: vars.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py)

## Classes
### `RunnerConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py:23`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L23)
- signature: `class RunnerConfig(BaseConfig):`
- members:
  - `id(self)` — [`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L60) — Generate a unique ID for the runner based on an unresolved config.
  - `save(self)` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L48) — For distributed training, be careful to only call this function on the main process.
  - `validate(self)` — [`L38`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L38)
  - `benchmark` — [`L28`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L28)
  - `interpreter` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L27)
  - `launcher` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L29)
  - `logger` — [`L24`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L24)
  - `metadata` — [`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L25)
  - `solver` — [`L26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L26)
  - `vars` — [`L30`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/runner.py#L30)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`SolverConfig`](solver/base.md#SolverConfig), [`InterpreterConfig`](interpreter/base.md#InterpreterConfig), [`LoggerConfig`](logger.md#LoggerConfig), [`output_dir`](logger.md#LoggerConfig.output_dir), [`LauncherConfig`](launcher/base.md#LauncherConfig), [`hash`](../../aira_core/config/base.md#BaseConfig.hash), [`fields_to_exclude_from_hash`](../../aira_core/config/base.md#BaseConfig.fields_to_exclude_from_hash), [`MetadataConfig`](metadata.md#MetadataConfig), [`BenchmarkConfig`](benchmark.md#BenchmarkConfig)
- used by: [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`_main`](../main_runner_job_array.md#_main), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`main`](../main_runner_job_array.md#main)

