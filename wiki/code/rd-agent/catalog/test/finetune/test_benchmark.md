---
title: 'Module: test/finetune/test_benchmark.py'
type: catalog
provenance: extracted
module: test/finetune/test_benchmark.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.finetune.test_benchmark`/
symbols:
  run_benchmark_simple: run_benchmark_simple().
  test_base: test_base.
  result: result.
  _project_root: _project_root.
  benchmark_results: benchmark_results.
  benchmark_name: benchmark_name.
  info: info.
  error_samples: error_samples.
  workspace: workspace.
  model_path_in_docker: model_path_in_docker.
  MODEL: MODEL.
  LIMIT: LIMIT.
  results_summary: results_summary.
  GPU_COUNT: GPU_COUNT.
  timestamp: timestamp.
  BENCHMARKS_TO_TEST: BENCHMARKS_TO_TEST.
  name: name.
---
# Module: [`test/finetune/test_benchmark.py`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py)

## Functions
- `run_benchmark_simple(workspace_path: str, model_path_in_docker: str, benchmark_name: str, gpu_count: int = 4, limit: int = 3, offset: int = 0, max_error_samples: int = 5, result_subdir: str = "")` — [`L28`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L28) — Simplified benchmark runner using rdagent Docker env. — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)

## Module values
- `BENCHMARKS_TO_TEST` — [`L184`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L184)
- `GPU_COUNT` — [`L166`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L166)
- `LIMIT` — [`L165`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L165)
- `MODEL` — [`L164`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L164)
- `_project_root` — [`L17`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L17)
- `benchmark_name` — [`L219`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L219)
- `benchmark_results` — [`L235`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L235)
- `error_samples` — [`L234`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L234)
- `info` — [`L250`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L250)
- `model_path_in_docker` — [`L169`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L169)
- `name` — [`L250`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L250)
- `result` — [`L225`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L225)
- `results_summary` — [`L181`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L181)
- `test_base` — [`L173`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L173)
- `timestamp` — [`L172`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L172)
- `workspace` — [`L224`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark.py#L224)

