---
title: 'Module: utils/evo_utils.py'
type: catalog
provenance: extracted
module: utils/evo_utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `utils.evo_utils`/
symbols:
  load_dgm_metadata: load_dgm_metadata().
  get_all_performance: get_all_performance().
  get_model_patch_paths: get_model_patch_paths().
  is_compiled_self_improve: is_compiled_self_improve().
---
# Module: [`utils/evo_utils.py`](../../../../../raw/code/dgm/utils/evo_utils.py)

## Functions
- `get_all_performance(run_keyword, results_dir='./swe_bench')` — [`L43`](../../../../../raw/code/dgm/utils/evo_utils.py#L43) — Retrieve performance results for all runs based on the provided keyword. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `get_model_patch_paths(root_dir, dgm_dir, parent_commit)` — [`L28`](../../../../../raw/code/dgm/utils/evo_utils.py#L28) — documented in [analysis-visualize_archive](../../concepts/analysis-visualize_archive.md)
- `is_compiled_self_improve(metadata, num_swe_issues=[], logger=None)` — [`L96`](../../../../../raw/code/dgm/utils/evo_utils.py#L96) — Checks if the run was properly compiled and 'self-improved' by verifying: — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `load_dgm_metadata(dgm_metadata_path, last_only=False)` — [`L7`](../../../../../raw/code/dgm/utils/evo_utils.py#L7) — documented in [DGM_outer](../../concepts/DGM_outer.md)

