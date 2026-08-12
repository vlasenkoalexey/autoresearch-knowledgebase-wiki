---
title: 'Module: tests/test_codex_session_reader.py'
type: catalog
provenance: extracted
module: tests/test_codex_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_codex_session_reader`/Test
symbols:
  TestFindSessionFiles.test_empty_dir_returns_empty: FindSessionFiles#test_empty_dir_returns_empty().
  TestFindSessionFiles.test_sessions_subdir_found: FindSessionFiles#test_sessions_subdir_found().
  TestFindSessionFiles.test_fallback_to_data_path_jsonl: FindSessionFiles#test_fallback_to_data_path_jsonl().
  TestLoadNewUsageEntries.test_empty_dir_returns_empty: LoadNewUsageEntries#test_empty_dir_returns_empty().
  TestLoadNewUsageEntries.test_event_msg_token_count_extracted: LoadNewUsageEntries#test_event_msg_token_count_extracted().
  TestLoadNewUsageEntries.test_usage_object_extracted: LoadNewUsageEntries#test_usage_object_extracted().
  TestLoadNewUsageEntries.test_dedup_by_processed_hashes: LoadNewUsageEntries#test_dedup_by_processed_hashes().
  TestLoadNewUsageEntries.test_malformed_line_skipped: LoadNewUsageEntries#test_malformed_line_skipped().
  TestLoadNewUsageEntries.test_duplicate_token_snapshots_collapsed_and_tool_call_attached: LoadNewUsageEntries#test_duplicate_token_snapshots_collapsed_and_tool_call_attached().
  TestLoadNewUsageEntries.test_multiple_rollouts_do_not_dedup_each_other: LoadNewUsageEntries#test_multiple_rollouts_do_not_dedup_each_other().
  TestFindSessionFiles: FindSessionFiles#
  TestLoadNewUsageEntries: LoadNewUsageEntries#
---
# Module: [`tests/test_codex_session_reader.py`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py)

## Classes
### `TestFindSessionFiles`
- def: [`tests/test_codex_session_reader.py:18`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L18)
- signature: `class TestFindSessionFiles:`
- members:
  - `test_empty_dir_returns_empty(self, tmp_path)` — [`L19`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L19)
  - `test_fallback_to_data_path_jsonl(self, tmp_path)` — [`L30`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L30)
  - `test_sessions_subdir_found(self, tmp_path)` — [`L22`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L22)
- uses (calls/refs, reference-scoped): [`find_session_files`](../utils/metric_tracking/codex_session_reader.md#find_session_files)

### `TestLoadNewUsageEntries`
- def: [`tests/test_codex_session_reader.py:36`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L36)
- signature: `class TestLoadNewUsageEntries:`
- members:
  - `test_dedup_by_processed_hashes(self, tmp_path)` — [`L82`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L82)
  - `test_duplicate_token_snapshots_collapsed_and_tool_call_attached(self, tmp_path)` — [`L119`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L119)
  - `test_empty_dir_returns_empty(self, tmp_path)` — [`L37`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L37)
  - `test_event_msg_token_count_extracted(self, tmp_path)` — [`L42`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L42)
  - `test_malformed_line_skipped(self, tmp_path)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L105)
  - `test_multiple_rollouts_do_not_dedup_each_other(self, tmp_path)` — [`L181`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L181)
  - `test_usage_object_extracted(self, tmp_path)` — [`L66`](../../../../../raw/code/continual-harness/tests/test_codex_session_reader.py#L66)
- uses (calls/refs, reference-scoped): [`load_new_usage_entries`](../utils/metric_tracking/codex_session_reader.md#load_new_usage_entries)

