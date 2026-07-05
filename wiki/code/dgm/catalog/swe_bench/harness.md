---
title: 'Module: swe_bench/harness.py'
type: catalog
provenance: extracted
module: swe_bench/harness.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `swe_bench.harness`/
symbols:
  process_entry: process_entry().
  harness: harness().
  main: main().
  harness.process_evaluation: harness().process_evaluation().
---
# Module: [`swe_bench/harness.py`](../../../../../raw/code/dgm/swe_bench/harness.py)

## Functions
- `harness(test_task_list=None, num_samples=-1, max_workers=4, model_name_or_path=None, model_patch_paths=None, num_evals=1, num_evals_parallel=1, pred_dname='./swe_bench/predictions')` — [`L184`](../../../../../raw/code/dgm/swe_bench/harness.py#L184) — Parallel processing harness using ThreadPoolExecutor.
- `main()` — [`L260`](../../../../../raw/code/dgm/swe_bench/harness.py#L260)
- `process_entry(entry, out_dname, model_name_or_path, model_patch_paths)` — [`L24`](../../../../../raw/code/dgm/swe_bench/harness.py#L24) — Process a single dataset entry. This function encapsulates the main processing logic
- `process_evaluation(eval_idx)` — [`L229`](../../../../../raw/code/dgm/swe_bench/harness.py#L229)

