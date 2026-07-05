---
title: 'Module: test/finetune/test_benchmark_api.py'
type: catalog
provenance: extracted
module: test/finetune/test_benchmark_api.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.finetune.test_benchmark_api`/
symbols:
  benchmark_name: benchmark_name.
  result: result.
  run_benchmark_api: run_benchmark_api().
  f: f.
  _project_root: _project_root.
  LIMIT: LIMIT.
  test_range: test_range.
  split_range: split_range.
  workspace: workspace.
  info: info.
  result_file: result_file.
  error_samples: error_samples.
  test_base: test_base.
  benchmark_results: benchmark_results.
  results_summary: results_summary.
  API_BASE: API_BASE.
  BENCHMARK: BENCHMARK.
  split_name: split_name.
  generate_api_config: generate_api_config().
  TEST_BENCHMARK_RANGES: TEST_BENCHMARK_RANGES.
  MODEL: MODEL.
  name: name.
  API_KEY: API_KEY.
  HF_TOKEN: HF_TOKEN.
  MAX_OUT_LEN: MAX_OUT_LEN.
  MAX_SEQ_LEN: MAX_SEQ_LEN.
  BATCH_SIZE: BATCH_SIZE.
  QUERY_PER_SECOND: QUERY_PER_SECOND.
  MAX_NUM_WORKERS: MAX_NUM_WORKERS.
  val_range: val_range.
  API_CONFIG_TEMPLATE: API_CONFIG_TEMPLATE.
  timestamp: timestamp.
  BENCHMARKS_TO_TEST: BENCHMARKS_TO_TEST.
---
# Module: [`test/finetune/test_benchmark_api.py`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py)

## Functions
- `generate_api_config(model_abbr: str, model_path: str, api_key: str, api_base: str, dataset_imports: list[str], limit: int | None = None, offset: int = 0, test_range: str | None = None, work_dir: str = "/workspace", max_out_len: int = 8192, max_seq_len: int = 32768, batch_size: int = 8, query_per_second: int = 1, max_num_workers: int = 16, retry: int = 5)` — [`L94`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L94) — Generate OpenCompass config for API-based model evaluation.
- `run_benchmark_api(workspace_path: str, model_name: str, api_key: str, api_base: str, benchmark_name: str, limit: int | None = 3, offset: int = 0, test_range: str | None = None, max_error_samples: int = 5, max_out_len: int = 8192, max_seq_len: int = 32768, batch_size: int = 8, query_per_second: int = 1, max_num_workers: int = 16, retry: int = 5, hf_token: str | None = None, result_subdir: str = "")` — [`L180`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L180) — API-based benchmark runner using rdagent Docker env. — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)

## Module values
- `API_BASE` — [`L336`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L336)
- `API_CONFIG_TEMPLATE` — [`L29`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L29)
- `API_KEY` — [`L335`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L335)
- `BATCH_SIZE` — [`L343`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L343)
- `BENCHMARK` — [`L368`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L368)
- `BENCHMARKS_TO_TEST` — [`L431`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L431)
- `HF_TOKEN` — [`L338`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L338)
- `LIMIT` — [`L421`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L421)
- `MAX_NUM_WORKERS` — [`L345`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L345)
- `MAX_OUT_LEN` — [`L341`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L341)
- `MAX_SEQ_LEN` — [`L342`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L342)
- `MODEL` — [`L337`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L337)
- `QUERY_PER_SECOND` — [`L344`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L344)
- `TEST_BENCHMARK_RANGES` — [`L353`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L353)
- `_project_root` — [`L18`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L18)
- `benchmark_name` — [`L466`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L466)
- `benchmark_results` — [`L397`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L397)
- `error_samples` — [`L396`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L396)
- `f` — [`L401`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L401)
- `info` — [`L416`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L416)
- `name` — [`L416`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L416)
- `result` — [`L378`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L378)
- `result_file` — [`L400`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L400)
- `results_summary` — [`L369`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L369)
- `split_name` — [`L371`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L371)
- `split_range` — [`L371`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L371)
- `test_base` — [`L349`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L349)
- `test_range` — [`L357`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L357)
- `timestamp` — [`L348`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L348)
- `val_range` — [`L357`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L357)
- `workspace` — [`L377`](../../../../../../raw/code/rd-agent/test/finetune/test_benchmark_api.py#L377)

