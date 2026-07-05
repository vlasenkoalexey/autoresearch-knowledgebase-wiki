---
title: 'Module: rdagent/scenarios/finetune/benchmark/benchmark.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/benchmark/benchmark.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.benchmark.benchmark`/
symbols:
  run_benchmark: run_benchmark().
  result: result.
  test_workspace: test_workspace.
  GPU_COUNT: GPU_COUNT.
  get_benchmark_ranges: get_benchmark_ranges().
  test_task: test_task.
  LORA_ADAPTER_PATH: LORA_ADAPTER_PATH.
  e: e.
  BENCHMARK: BENCHMARK.
  MODEL_NAME: MODEL_NAME.
  get_model_inference_config: get_model_inference_config().
  detect_model_type: detect_model_type().
---
# Module: [`rdagent/scenarios/finetune/benchmark/benchmark.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py)

## Functions
- `detect_model_type(model_path: str)` — [`L95`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L95) — Detect whether the given model path corresponds to a LoRA adapter.
- `get_benchmark_ranges()` — [`L332`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L332) — Get validation and test range strings for benchmark evaluation.
- `get_model_inference_config(base_model_name: str, gpu_count: int)` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L50) — Load model inference configuration from YAML file.
- `run_benchmark(workspace_path: str, model_path: str, model_name: str, benchmark_name: str, gpu_count: int, test_range: Optional[str] = "[:100]", num_runs: int = 1, pass_k: Optional[List[int]] = None, max_error_samples: int = 10, result_subdir: str = "")` — [`L116`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L116) — Run benchmark evaluation on a fine-tuned model. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)

## Module values
- `BENCHMARK` — [`L354`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L354)
- `GPU_COUNT` — [`L355`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L355)
- `LORA_ADAPTER_PATH` — [`L352`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L352)
- `MODEL_NAME` — [`L353`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L353)
- `e` — [`L394`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L394)
- `result` — [`L381`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L381)
- `test_task` — [`L375`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L375)
- `test_workspace` — [`L376`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/benchmark.py#L376)

