---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.task.mlebench`/
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
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py)

## Classes
### `MLEBenchTaskConfig`  ·  implements/extends TaskConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py:74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L74)
- signature: `class MLEBenchTaskConfig(TaskConfig):`
- members:
  - `validate(self)` — [`L125`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L125)
  - `benchmark` — [`L75`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L75)
  - `cache_dir` — [`L89`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L89)
  - `data_dir` — [`L82`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L82)
  - `private_dir` — [`L103`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L103)
  - `public_dir` — [`L96`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L96)
  - `results_output_dir` — [`L117`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L117)
  - `submission_fname` — [`L110`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L110)
- uses (calls/refs, reference-scoped): [`TaskConfig`](base.md#TaskConfig), [`get_mlebench_data_dir`](../../utils/environment.md#get_mlebench_data_dir), [`validate`](base.md#TaskConfig.validate)
- used by: [`to_cfg_list`](../benchmark.md#BenchmarkConfig.to_cfg_list), [`TaskConfig`](base.md#TaskConfig), [`validate`](base.md#TaskConfig.validate), [`__init__`](../../tasks/mlebench/task.md#MLEBenchTask.__init__)

## Module values
- `mlebench_operator_prompts` — [`L14`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/task/mlebench.py#L14)

