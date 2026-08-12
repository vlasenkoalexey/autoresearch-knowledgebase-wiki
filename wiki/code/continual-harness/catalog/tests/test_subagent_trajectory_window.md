---
title: 'Module: tests/test_subagent_trajectory_window.py'
type: catalog
provenance: extracted
module: tests/test_subagent_trajectory_window.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_subagent_trajectory_window`/
symbols:
  test_sync_trajectories_to_run_data: test_sync_trajectories_to_run_data().
  test_load_recent_trajectories_caps_window_at_max: test_load_recent_trajectories_caps_window_at_max().
  test_load_recent_trajectories_from_cache: test_load_recent_trajectories_from_cache().
  test_trajectory_file_resolves_run_data_copy_when_cache_missing: test_trajectory_file_resolves_run_data_copy_when_cache_missing().
  test_load_recent_trajectories_handles_missing_or_empty_files: test_load_recent_trajectories_handles_missing_or_empty_files().
  _CACHE_MOCK_TARGET: _CACHE_MOCK_TARGET.
  test_format_trajectory_window_without_post_state: test_format_trajectory_window_without_post_state().
  test_format_trajectory_window_with_legacy_post_state: test_format_trajectory_window_with_legacy_post_state().
  test_format_trajectory_window_with_objective_context: test_format_trajectory_window_with_objective_context().
  test_read_last_jsonl_lines_matches_full_scan_suffix: test_read_last_jsonl_lines_matches_full_scan_suffix().
  _RunManagerStub: _RunManagerStub#
  _write_trajectories_cache: _write_trajectories_cache().
  _RunManagerStub.__init__: _RunManagerStub#__init__().
  _RunManagerStub.run_dir: _RunManagerStub#run_dir.
---
# Module: [`tests/test_subagent_trajectory_window.py`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py)

## Classes
### `_RunManagerStub`
- def: [`tests/test_subagent_trajectory_window.py:22`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L22)
- signature: `class _RunManagerStub:`
- members:
  - `run_dir` — [`L24`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L24)
- protocol/private: `__init__`[`L23`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L23)
- used by: (2 test-only callers)

## Functions
- `_write_trajectories_cache(cache_dir: Path, count: int)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L27) — Write trajectory entries to cache-style path.
- `test_format_trajectory_window_with_legacy_post_state()` — [`L116`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L116) — post_state is ignored even if present in legacy data.
- `test_format_trajectory_window_with_objective_context()` — [`L133`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L133)
- `test_format_trajectory_window_without_post_state()` — [`L98`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L98)
- `test_load_recent_trajectories_caps_window_at_max(tmp_path)` — [`L64`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L64)
- `test_load_recent_trajectories_from_cache(tmp_path)` — [`L55`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L55)
- `test_load_recent_trajectories_handles_missing_or_empty_files(tmp_path)` — [`L89`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L89)
- `test_read_last_jsonl_lines_matches_full_scan_suffix(tmp_path)` — [`L179`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L179)
- `test_sync_trajectories_to_run_data(tmp_path)` — [`L152`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L152) — sync_trajectories_to_run_data copies JSONL from cache to run_data.
- `test_trajectory_file_resolves_run_data_copy_when_cache_missing(tmp_path)` — [`L76`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L76)

## Module values
- `_CACHE_MOCK_TARGET` — [`L52`](../../../../../raw/code/continual-harness/tests/test_subagent_trajectory_window.py#L52)

