---
title: 'Module: swe_bench/report.py'
type: catalog
provenance: extracted
module: swe_bench/report.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `swe_bench.report`/
symbols:
  make_report: make_report().
  make_report.process_single_dname: make_report().process_single_dname().
  preds_to_jsonl: preds_to_jsonl().
  main: main().
  load_predictions: load_predictions().
  remove_patches_to_tests: remove_patches_to_tests().
  run_evals: run_evals().
---
# Module: [`swe_bench/report.py`](../../../../../raw/code/dgm/swe_bench/report.py)

## Functions
- `load_predictions(paths)` — [`L9`](../../../../../raw/code/dgm/swe_bench/report.py#L9)
- `main()` — [`L132`](../../../../../raw/code/dgm/swe_bench/report.py#L132)
- `make_report(dnames, run_ids=None, dataset_name="princeton-nlp/SWE-bench_Verified", output_dir='./swe_bench', dnames_workers=None, num_eval_procs=5)` — [`L96`](../../../../../raw/code/dgm/swe_bench/report.py#L96) — Generate reports for multiple directories in parallel.
- `preds_to_jsonl(dname, predictions)` — [`L67`](../../../../../raw/code/dgm/swe_bench/report.py#L67)
- `process_single_dname(dname, run_id)` — [`L115`](../../../../../raw/code/dgm/swe_bench/report.py#L115)
- `remove_patches_to_tests(model_patch)` — [`L37`](../../../../../raw/code/dgm/swe_bench/report.py#L37) — Remove any changes to the tests directory from the provided patch.
- `run_evals(predictions_jsonl, run_id, dataset_name, root_dir, output_dir, num_eval_procs=5)` — [`L83`](../../../../../raw/code/dgm/swe_bench/report.py#L83)

