---
title: 'Module: tests/test_claude_session_reader.py'
type: catalog
provenance: extracted
module: tests/test_claude_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_claude_session_reader`/
symbols:
  TestAppendCliStepIntegration.test_steps_appended_to_cumulative_metrics: TestAppendCliStepIntegration#test_steps_appended_to_cumulative_metrics().
  TestLoadNewUsageEntries.test_returns_only_assistant_entries_with_usage: TestLoadNewUsageEntries#test_returns_only_assistant_entries_with_usage().
  ASSISTANT_ENTRY_FULL: ASSISTANT_ENTRY_FULL.
  TestLoadNewUsageEntries.test_new_entries_picked_up_after_first_poll: TestLoadNewUsageEntries#test_new_entries_picked_up_after_first_poll().
  TestLoadNewUsageEntries.test_multi_file_rglob: TestLoadNewUsageEntries#test_multi_file_rglob().
  TestCumulativeMetricsSchema.test_append_cli_step_produces_valid_step_shape: TestCumulativeMetricsSchema#test_append_cli_step_produces_valid_step_shape().
  TestCumulativeMetricsSchema.test_persisted_file_has_correct_schema: TestCumulativeMetricsSchema#test_persisted_file_has_correct_schema().
  TestLoadNewUsageEntries._write_jsonl: TestLoadNewUsageEntries#_write_jsonl().
  TestLoadNewUsageEntries.test_deduplication_on_second_poll: TestLoadNewUsageEntries#test_deduplication_on_second_poll().
  TestLoadNewUsageEntries.test_tokens_and_tool_calls_injected: TestLoadNewUsageEntries#test_tokens_and_tool_calls_injected().
  TestCumulativeMetricsSchema.test_fresh_logger_has_required_keys: TestCumulativeMetricsSchema#test_fresh_logger_has_required_keys().
  ASSISTANT_ENTRY_NO_CACHE: ASSISTANT_ENTRY_NO_CACHE.
  TestExtractTokensFromEntry.test_full_entry_returns_all_buckets: TestExtractTokensFromEntry#test_full_entry_returns_all_buckets().
  TestExtractTokensFromEntry.test_no_cache_entry: TestExtractTokensFromEntry#test_no_cache_entry().
  TestExtractTokensFromEntry.test_user_entry_returns_none: TestExtractTokensFromEntry#test_user_entry_returns_none().
  TestExtractTokensFromEntry.test_malformed_usage_returns_none: TestExtractTokensFromEntry#test_malformed_usage_returns_none().
  TestExtractToolCalls.test_extracts_tool_use_blocks: TestExtractToolCalls#test_extracts_tool_use_blocks().
  TestExtractToolCalls.test_no_tools_returns_empty_list: TestExtractToolCalls#test_no_tools_returns_empty_list().
  TestExtractToolCalls.test_user_entry_returns_empty_list: TestExtractToolCalls#test_user_entry_returns_empty_list().
  TestCreateUniqueHash.test_uses_message_id_and_request_id: TestCreateUniqueHash#test_uses_message_id_and_request_id().
  TestLoadNewUsageEntries.test_malformed_lines_skipped: TestLoadNewUsageEntries#test_malformed_lines_skipped().
  TestLoadNewUsageEntries.test_openrouter_dedup_groups_by_message_id: TestLoadNewUsageEntries#test_openrouter_dedup_groups_by_message_id().
  TestLoadNewUsageEntries.test_openrouter_dedup_separate_api_calls: TestLoadNewUsageEntries#test_openrouter_dedup_separate_api_calls().
  USER_ENTRY: USER_ENTRY.
  TestExtractTokensFromEntry.test_top_level_usage_fallback: TestExtractTokensFromEntry#test_top_level_usage_fallback().
  TestExtractTokensFromEntry.test_missing_message_key_falls_back_to_top_level: TestExtractTokensFromEntry#test_missing_message_key_falls_back_to_top_level().
  TestCreateUniqueHash.test_message_id_only_when_no_request_id: TestCreateUniqueHash#test_message_id_only_when_no_request_id().
  TestCreateUniqueHash.test_falls_back_to_uuid: TestCreateUniqueHash#test_falls_back_to_uuid().
  TestCreateUniqueHash.test_returns_none_when_no_ids: TestCreateUniqueHash#test_returns_none_when_no_ids().
  TestParseTimestamp.test_iso_z_string: TestParseTimestamp#test_iso_z_string().
  TestParseTimestamp.test_unix_float: TestParseTimestamp#test_unix_float().
  TestParseTimestamp.test_none_input: TestParseTimestamp#test_none_input().
  TestParseTimestamp.test_malformed_string: TestParseTimestamp#test_malformed_string().
  TestLoadNewUsageEntries.test_nonexistent_path_returns_empty: TestLoadNewUsageEntries#test_nonexistent_path_returns_empty().
  REQUIRED_TOP_LEVEL_KEYS: REQUIRED_TOP_LEVEL_KEYS.
  REQUIRED_STEP_KEYS: REQUIRED_STEP_KEYS.
  MALFORMED_USAGE_ENTRY: MALFORMED_USAGE_ENTRY.
  TestExtractTokensFromEntry: TestExtractTokensFromEntry#
  TestExtractToolCalls: TestExtractToolCalls#
  TestCreateUniqueHash: TestCreateUniqueHash#
  TestParseTimestamp: TestParseTimestamp#
  TestLoadNewUsageEntries: TestLoadNewUsageEntries#
  TestAppendCliStepIntegration: TestAppendCliStepIntegration#
  TestCumulativeMetricsSchema: TestCumulativeMetricsSchema#
---
# Module: [`tests/test_claude_session_reader.py`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py)

## Classes
### `TestAppendCliStepIntegration`
- def: [`tests/test_claude_session_reader.py:385`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L385)
- doc: Test that the poller correctly updates cumulative_metrics via LLMLogger.
- signature: `class TestAppendCliStepIntegration:`
- members:
  - `test_steps_appended_to_cumulative_metrics(self, tmp_path)` — [`L388`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L388)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`load_new_usage_entries`](../utils/metric_tracking/claude_session_reader.md#load_new_usage_entries), [`append_cli_step`](../utils/data_persistence/llm_logger.md#LLMLogger.append_cli_step)  (2 test-only)

### `TestCreateUniqueHash`
- def: [`tests/test_claude_session_reader.py:160`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L160)
- signature: `class TestCreateUniqueHash:`
- members:
  - `test_falls_back_to_uuid(self)` — [`L175`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L175)
  - `test_message_id_only_when_no_request_id(self)` — [`L165`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L165) — OpenRouter entries have message.id but no requestId.
  - `test_returns_none_when_no_ids(self)` — [`L180`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L180)
  - `test_uses_message_id_and_request_id(self)` — [`L161`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L161)
- uses (calls/refs, reference-scoped): [`_create_unique_hash`](../utils/metric_tracking/claude_session_reader.md#_create_unique_hash)  (1 test-only)

### `TestCumulativeMetricsSchema`
- def: [`tests/test_claude_session_reader.py:467`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L467)
- doc: Ensure LLMLogger always produces a cumulative_metrics.json with the required schema.
- signature: `class TestCumulativeMetricsSchema:`
- members:
  - `test_append_cli_step_produces_valid_step_shape(self, tmp_path)` — [`L480`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L480)
  - `test_fresh_logger_has_required_keys(self, tmp_path)` — [`L470`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L470)
  - `test_persisted_file_has_correct_schema(self, tmp_path)` — [`L500`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L500)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`append_cli_step`](../utils/data_persistence/llm_logger.md#LLMLogger.append_cli_step)  (2 test-only)

### `TestExtractTokensFromEntry`
- def: [`tests/test_claude_session_reader.py:96`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L96)
- signature: `class TestExtractTokensFromEntry:`
- members:
  - `test_full_entry_returns_all_buckets(self)` — [`L97`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L97)
  - `test_malformed_usage_returns_none(self)` — [`L118`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L118)
  - `test_missing_message_key_falls_back_to_top_level(self)` — [`L134`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L134)
  - `test_no_cache_entry(self)` — [`L106`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L106)
  - `test_top_level_usage_fallback(self)` — [`L121`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L121)
  - `test_user_entry_returns_none(self)` — [`L115`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L115)
- uses (calls/refs, reference-scoped): [`extract_tokens_from_entry`](../utils/metric_tracking/claude_session_reader.md#extract_tokens_from_entry)  (4 test-only)

### `TestExtractToolCalls`
- def: [`tests/test_claude_session_reader.py:144`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L144)
- signature: `class TestExtractToolCalls:`
- members:
  - `test_extracts_tool_use_blocks(self)` — [`L145`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L145)
  - `test_no_tools_returns_empty_list(self)` — [`L151`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L151)
  - `test_user_entry_returns_empty_list(self)` — [`L155`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L155)
- uses (calls/refs, reference-scoped): [`extract_tool_calls_from_entry`](../utils/metric_tracking/claude_session_reader.md#extract_tool_calls_from_entry)  (3 test-only)

### `TestLoadNewUsageEntries`
- def: [`tests/test_claude_session_reader.py:208`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L208)
- signature: `class TestLoadNewUsageEntries:`
- members:
  - `test_deduplication_on_second_poll(self, tmp_path)` — [`L221`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L221)
  - `test_malformed_lines_skipped(self, tmp_path)` — [`L252`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L252)
  - `test_multi_file_rglob(self, tmp_path)` — [`L265`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L265)
  - `test_new_entries_picked_up_after_first_poll(self, tmp_path)` — [`L229`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L229)
  - `test_nonexistent_path_returns_empty(self, tmp_path)` — [`L260`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L260)
  - `test_openrouter_dedup_groups_by_message_id(self, tmp_path)` — [`L273`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L273) — OpenRouter emits multiple content blocks per API call sharing the
  - `test_openrouter_dedup_separate_api_calls(self, tmp_path)` — [`L342`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L342) — Two separate OpenRouter API calls (different message.id) should
  - `test_returns_only_assistant_entries_with_usage(self, tmp_path)` — [`L214`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L214)
  - `test_tokens_and_tool_calls_injected(self, tmp_path)` — [`L241`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L241)
- protocol/private: `_write_jsonl`[`L209`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L209)
- uses (calls/refs, reference-scoped): [`load_new_usage_entries`](../utils/metric_tracking/claude_session_reader.md#load_new_usage_entries)  (3 test-only)

### `TestParseTimestamp`
- def: [`tests/test_claude_session_reader.py:184`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L184)
- signature: `class TestParseTimestamp:`
- members:
  - `test_iso_z_string(self)` — [`L185`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L185)
  - `test_malformed_string(self)` — [`L200`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L200)
  - `test_none_input(self)` — [`L197`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L197)
  - `test_unix_float(self)` — [`L191`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L191)
- uses (calls/refs, reference-scoped): [`_parse_timestamp`](../utils/metric_tracking/claude_session_reader.md#_parse_timestamp)

## Module values
- `ASSISTANT_ENTRY_FULL` — [`L31`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L31)
- `ASSISTANT_ENTRY_NO_CACHE` — [`L57`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L57)
- `MALFORMED_USAGE_ENTRY` — [`L83`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L83)
- `REQUIRED_STEP_KEYS` — [`L455`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L455)
- `REQUIRED_TOP_LEVEL_KEYS` — [`L437`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L437)
- `USER_ENTRY` — [`L76`](../../../../../raw/code/continual-harness/tests/test_claude_session_reader.py#L76)

