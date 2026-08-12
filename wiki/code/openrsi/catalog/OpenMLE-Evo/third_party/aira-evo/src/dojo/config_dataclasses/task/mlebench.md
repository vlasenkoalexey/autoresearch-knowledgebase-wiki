---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.task.mlebench`/
symbols:
  MLEBenchTaskConfig: MLEBenchTaskConfig#
  MLEBenchTaskConfig.cache_dir: MLEBenchTaskConfig#cache_dir.
  MLEBenchTaskConfig.validate: MLEBenchTaskConfig#validate().
  MLEBenchTaskConfig.benchmark: MLEBenchTaskConfig#benchmark.
  MLEBenchTaskConfig.data_dir: MLEBenchTaskConfig#data_dir.
  MLEBenchTaskConfig.public_dir: MLEBenchTaskConfig#public_dir.
  MLEBenchTaskConfig.private_dir: MLEBenchTaskConfig#private_dir.
  MLEBenchTaskConfig.submission_fname: MLEBenchTaskConfig#submission_fname.
  MLEBenchTaskConfig.results_output_dir: MLEBenchTaskConfig#results_output_dir.
  mlebench_operator_prompts.mlebench_operator_prompts: mlebench_operator_prompts.mlebench_operator_prompts.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py)

## Classes
### `MLEBenchTaskConfig`  ·  implements/extends TaskConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py:73`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L73)
- signature: `class MLEBenchTaskConfig(TaskConfig):`
- members:
  - `validate(self)` — [`L124`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L124)
  - `benchmark` — [`L74`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L74)
  - `cache_dir` — [`L88`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L88)
  - `data_dir` — [`L81`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L81)
  - `private_dir` — [`L102`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L102)
  - `public_dir` — [`L95`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L95)
  - `results_output_dir` — [`L116`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L116)
  - `submission_fname` — [`L109`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L109)
- uses (calls/refs, reference-scoped): [`get_mlebench_data_dir`](../../utils/environment.md#get_mlebench_data_dir), [`TaskConfig`](base.md#TaskConfig), [`validate`](base.md#TaskConfig.validate)
- used by: [`execute_code`](../../grade_code.md#execute_code), [`to_cfg_list`](../benchmark.md#BenchmarkConfig.to_cfg_list), [`TaskConfig`](base.md#TaskConfig), [`validate`](base.md#TaskConfig.validate), [`__init__`](../../tasks/mlebench/task.md#MLEBenchTask.__init__)

## Module values
- `mlebench_operator_prompts` — [`L14`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L14)

