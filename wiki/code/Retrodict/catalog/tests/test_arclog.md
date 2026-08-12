---
title: 'Module: tests/test_arclog.py'
type: catalog
provenance: extracted
module: tests/test_arclog.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_arclog`/
symbols:
  load_arclog_module: load_arclog_module().
  copy_workspace: copy_workspace().
  FIXTURE_LOG: FIXTURE_LOG.
  test_load_parses_shared_golden_log_with_diffs: test_load_parses_shared_golden_log_with_diffs().
  test_boards_are_numpy_arrays_for_spatial_ops: test_boards_are_numpy_arrays_for_spatial_ops().
  test_objects_accepts_a_step_object: test_objects_accepts_a_step_object().
  ARClOG_PATH: ARClOG_PATH.
  REPO_ROOT: REPO_ROOT.
  test_load_parses_summarized_diff_line: test_load_parses_summarized_diff_line().
  test_diff_uses_column_row_ordering: test_diff_uses_column_row_ordering().
  test_objects_find_components_and_translation_invariant_hashes: test_objects_find_components_and_translation_invariant_hashes().
  test_objects_support_eight_way_connectivity_and_reject_invalid_connectivity: test_objects_support_eight_way_connectivity_and_reject_invalid_connectivity().
  test_object_hash_is_stable_across_analysis_subprocesses: test_object_hash_is_stable_across_analysis_subprocesses().
  test_arclog_imports_in_workspace_but_game_engine_stays_blocked: test_arclog_imports_in_workspace_but_game_engine_stays_blocked().
  test_scratch_modules_can_be_written_then_imported_without_engine_access: test_scratch_modules_can_be_written_then_imported_without_engine_access().
---
# Module: [`tests/test_arclog.py`](../../../../../raw/code/Retrodict/tests/test_arclog.py)

## Functions
- `copy_workspace(tmp_path: Path)` — [`L33`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L33)
- `load_arclog_module()` — [`L19`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L19)
- `test_arclog_imports_in_workspace_but_game_engine_stays_blocked(tmp_path: Path, analysis_python: Path)` — [`L199`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L199)
- `test_boards_are_numpy_arrays_for_spatial_ops()` — [`L73`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L73)
- `test_diff_uses_column_row_ordering()` — [`L124`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L124)
- `test_load_parses_shared_golden_log_with_diffs()` — [`L40`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L40)
- `test_load_parses_summarized_diff_line(tmp_path: Path)` — [`L92`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L92)
- `test_object_hash_is_stable_across_analysis_subprocesses(tmp_path: Path, analysis_python: Path)` — [`L189`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L189)
- `test_objects_accepts_a_step_object()` — [`L166`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L166)
- `test_objects_find_components_and_translation_invariant_hashes()` — [`L135`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L135)
- `test_objects_support_eight_way_connectivity_and_reject_invalid_connectivity()` — [`L174`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L174)
- `test_scratch_modules_can_be_written_then_imported_without_engine_access(tmp_path: Path, analysis_python: Path)` — [`L212`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L212)

## Module values
- `ARClOG_PATH` — [`L15`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L15)
- `FIXTURE_LOG` — [`L16`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L16)
- `REPO_ROOT` — [`L14`](../../../../../raw/code/Retrodict/tests/test_arclog.py#L14)

