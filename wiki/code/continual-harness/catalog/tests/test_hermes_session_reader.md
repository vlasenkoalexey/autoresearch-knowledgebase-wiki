---
title: 'Module: tests/test_hermes_session_reader.py'
type: catalog
provenance: extracted
module: tests/test_hermes_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_hermes_session_reader`/
symbols:
  TestHermesSessionReader.test_load_new_usage_entries_reads_session_json_and_usage_events: TestHermesSessionReader#test_load_new_usage_entries_reads_session_json_and_usage_events().
  TestHermesSessionReader.test_second_poll_with_same_state_returns_no_entries: TestHermesSessionReader#test_second_poll_with_same_state_returns_no_entries().
  TestHermesSessionReader.test_get_latest_session_id_reads_session_logs: TestHermesSessionReader#test_get_latest_session_id_reads_session_logs().
  _write_session_log: _write_session_log().
  TestHermesSessionReader.test_normalize_tool_calls_reads_nested_function_shape: TestHermesSessionReader#test_normalize_tool_calls_reads_nested_function_shape().
  _write_usage_events: _write_usage_events().
  TestHermesSessionReader: TestHermesSessionReader#
---
# Module: [`tests/test_hermes_session_reader.py`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py)

## Classes
### `TestHermesSessionReader`
- def: [`tests/test_hermes_session_reader.py:32`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L32)
- signature: `class TestHermesSessionReader:`
- members:
  - `test_get_latest_session_id_reads_session_logs(self, tmp_path)` — [`L33`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L33)
  - `test_load_new_usage_entries_reads_session_json_and_usage_events(self, tmp_path)` — [`L43`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L43)
  - `test_normalize_tool_calls_reads_nested_function_shape(self)` — [`L138`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L138)
  - `test_second_poll_with_same_state_returns_no_entries(self, tmp_path)` — [`L108`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L108)
- uses (calls/refs, reference-scoped): [`load_new_usage_entries`](../utils/metric_tracking/hermes_session_reader.md#load_new_usage_entries), [`get_latest_session_id`](../utils/metric_tracking/hermes_session_reader.md#get_latest_session_id), [`_normalize_tool_calls`](../utils/metric_tracking/hermes_session_reader.md#_normalize_tool_calls)  (2 test-only)

## Functions
- `_write_session_log(tmp_path: Path, payload: dict)` — [`L17`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L17)
- `_write_usage_events(tmp_path: Path, *events: dict)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_hermes_session_reader.py#L27)

