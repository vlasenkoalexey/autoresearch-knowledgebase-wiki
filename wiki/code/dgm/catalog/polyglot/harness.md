---
title: 'Module: polyglot/harness.py'
type: catalog
provenance: extracted
module: polyglot/harness.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.harness`/
symbols:
  process_entry: process_entry().
  harness: harness().
  main: main().
  harness.process_evaluation: harness().process_evaluation().
  get_eval_script: get_eval_script().
---
# Module: [`polyglot/harness.py`](../../../../../raw/code/dgm/polyglot/harness.py)

## Functions
- `get_eval_script(commands)` — [`L28`](../../../../../raw/code/dgm/polyglot/harness.py#L28)
- `harness(dataset_path="polyglot/polyglot_benchmark_metadata.json", test_task_list=None, num_samples=-1, max_workers=4, model_name_or_path=None, model_patch_paths=None, num_evals=1, num_evals_parallel=1, pred_dname='./polyglot/predictions', output_dir='./polyglot/predictions')` — [`L236`](../../../../../raw/code/dgm/polyglot/harness.py#L236) — Parallel processing harness using ThreadPoolExecutor. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `main()` — [`L385`](../../../../../raw/code/dgm/polyglot/harness.py#L385)
- `process_entry(entry, out_dname, model_name_or_path, model_patch_paths)` — [`L31`](../../../../../raw/code/dgm/polyglot/harness.py#L31) — Process a single dataset entry. This function encapsulates the main processing logic — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `process_evaluation(eval_idx)` — [`L298`](../../../../../raw/code/dgm/polyglot/harness.py#L298)

