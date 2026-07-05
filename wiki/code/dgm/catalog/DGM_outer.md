---
title: 'Module: DGM_outer.py'
type: catalog
provenance: extracted
module: DGM_outer.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 DGM_outer/
symbols:
  main: main().
  choose_selfimproves: choose_selfimproves().
  filter_compiled: filter_compiled().
  update_archive: update_archive().
  get_full_eval_threshold: get_full_eval_threshold().
  get_original_score: get_original_score().
  initialize_run: initialize_run().
  any_exceeding_context_length: any_exceeding_context_length().
---
# Module: [`DGM_outer.py`](../../../../raw/code/dgm/DGM_outer.py)

## Functions
- `any_exceeding_context_length(output_dir, commit_id, instance_ids)` — [`L37`](../../../../raw/code/dgm/DGM_outer.py#L37) — Check if any of the issues have exceeded the context length. — documented in [DGM_outer](../concepts/DGM_outer.md)
- `choose_selfimproves(output_dir, archive, selfimprove_size, method='random', run_baseline=None, polyglot=False)` — [`L50`](../../../../raw/code/dgm/DGM_outer.py#L50) — Choose self-improve attempts for the current generation. — documented in [DGM_outer](../concepts/DGM_outer.md)
- `filter_compiled(run_ids, output_dir, num_swe_issues=[], logger=None)` — [`L152`](../../../../raw/code/dgm/DGM_outer.py#L152) — Filter out runs that did not compile or have all empty patches.
- `get_full_eval_threshold(output_dir, archive)` — [`L192`](../../../../raw/code/dgm/DGM_outer.py#L192) — Get the threshold for full evaluation. — documented in [DGM_outer](../concepts/DGM_outer.md)
- `get_original_score(output_dir)` — [`L167`](../../../../raw/code/dgm/DGM_outer.py#L167) — Get the original score from the initial version. — documented in [DGM_outer](../concepts/DGM_outer.md)
- `initialize_run(output_dir, prevrun_dir=None, polyglot=False)` — [`L15`](../../../../raw/code/dgm/DGM_outer.py#L15) — documented in [DGM_outer](../concepts/DGM_outer.md)
- `main()` — [`L221`](../../../../raw/code/dgm/DGM_outer.py#L221) — documented in [DGM_outer](../concepts/DGM_outer.md)
- `update_archive(output_dir, archive, new_ids, method='keep_all', noise_leeway=0.1)` — [`L174`](../../../../raw/code/dgm/DGM_outer.py#L174) — Update the archive with the new self-improve runs. — documented in [DGM_outer](../concepts/DGM_outer.md)

