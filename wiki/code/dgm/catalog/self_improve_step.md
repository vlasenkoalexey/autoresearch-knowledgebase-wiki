---
title: 'Module: self_improve_step.py'
type: catalog
provenance: extracted
module: self_improve_step.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 self_improve_step/
symbols:
  self_improve: self_improve().
  diagnose_problem: diagnose_problem().
  diagnose_improvement: diagnose_improvement().
  run_harness_swe: run_harness_swe().
  run_harness_polyglot: run_harness_polyglot().
  dataset: dataset.
  save_metadata: save_metadata().
  main: main().
  diagnose_model: diagnose_model.
---
# Module: [`self_improve_step.py`](../../../../raw/code/dgm/self_improve_step.py)

## Functions
- `diagnose_improvement(entry, parent_commit, root_dir, model_patch_file, out_dir, run_id, patch_files=[], max_attempts=3)` — [`L69`](../../../../raw/code/dgm/self_improve_step.py#L69) — Diagnose the improvement of the model patch. — documented in [self_improve_step](../concepts/self_improve_step.md)
- `diagnose_problem(entry, commit, root_dir, out_dir, patch_files=[], max_attempts=3, polyglot=False)` — [`L30`](../../../../raw/code/dgm/self_improve_step.py#L30) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `main()` — [`L422`](../../../../raw/code/dgm/self_improve_step.py#L422) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `run_harness_polyglot(entry, model_name_or_path, patch_files, num_evals, output_dir, metadata, run_id, test_more_threshold, test_task_list, test_task_list_more)` — [`L180`](../../../../raw/code/dgm/self_improve_step.py#L180) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `run_harness_swe(entry, model_name_or_path, patch_files, num_evals, output_dir, metadata, run_id, test_more_threshold, test_task_list, test_task_list_more)` — [`L125`](../../../../raw/code/dgm/self_improve_step.py#L125) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `save_metadata(metadata, output_dir)` — [`L120`](../../../../raw/code/dgm/self_improve_step.py#L120) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `self_improve(parent_commit='initial', output_dir='output_selfimprove/', force_rebuild=False, num_evals=1, post_improve_diagnose=True, entry=None, test_task_list=None, test_more_threshold=None, test_task_list_more=None, full_eval_threshold=None, run_baseline=None, polyglot=False)` — [`L223`](../../../../raw/code/dgm/self_improve_step.py#L223) — documented in [self_improve_step](../concepts/self_improve_step.md)

## Module values
- `dataset` — [`L27`](../../../../raw/code/dgm/self_improve_step.py#L27) — documented in [self_improve_step](../concepts/self_improve_step.md)
- `diagnose_model` — [`L28`](../../../../raw/code/dgm/self_improve_step.py#L28)

