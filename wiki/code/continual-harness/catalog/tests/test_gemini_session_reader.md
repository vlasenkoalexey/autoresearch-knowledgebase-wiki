---
title: 'Module: tests/test_gemini_session_reader.py'
type: catalog
provenance: extracted
module: tests/test_gemini_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_gemini_session_reader`/
symbols:
  TestGeminiCostCalculationSubsetStyle.test_gemini_subset_cost_uses_uncached_plus_cached_rates: TestGeminiCostCalculationSubsetStyle#test_gemini_subset_cost_uses_uncached_plus_cached_rates().
  TestExtractTokensFromMessage.test_full_entry_returns_all_buckets: TestExtractTokensFromMessage#test_full_entry_returns_all_buckets().
  TestExtractTokensFromMessage.test_minimal_entry: TestExtractTokensFromMessage#test_minimal_entry().
  TestExtractTokensFromMessage.test_computes_total_when_zero: TestExtractTokensFromMessage#test_computes_total_when_zero().
  TestExtractToolCallsFromMessage.test_extracts_tool_calls: TestExtractToolCallsFromMessage#test_extracts_tool_calls().
  TestExtractToolCallsFromMessage.test_empty_tool_calls: TestExtractToolCallsFromMessage#test_empty_tool_calls().
  TestLoadNewUsageEntries._write_session: TestLoadNewUsageEntries#_write_session().
  TestLoadNewUsageEntries.test_loads_gemini_messages: TestLoadNewUsageEntries#test_loads_gemini_messages().
  TestLoadNewUsageEntries.test_deduplication_across_polls: TestLoadNewUsageEntries#test_deduplication_across_polls().
  TestLoadNewUsageEntries.test_skips_non_gemini_messages: TestLoadNewUsageEntries#test_skips_non_gemini_messages().
  TestLoadNewUsageEntries.test_skips_zero_total_entries: TestLoadNewUsageEntries#test_skips_zero_total_entries().
  TestLoadNewUsageEntries.test_skips_messages_without_id: TestLoadNewUsageEntries#test_skips_messages_without_id().
  TestExtractTokensFromMessage.test_cache_write_none_when_absent: TestExtractTokensFromMessage#test_cache_write_none_when_absent().
  TestExtractTokensFromMessage.test_cache_write_from_session_when_present: TestExtractTokensFromMessage#test_cache_write_from_session_when_present().
  TestExtractTokensFromMessage.test_no_tokens_dict_returns_none: TestExtractTokensFromMessage#test_no_tokens_dict_returns_none().
  TestExtractTokensFromMessage.test_tokens_not_dict_returns_none: TestExtractTokensFromMessage#test_tokens_not_dict_returns_none().
  TestExtractToolCallsFromMessage.test_no_tool_calls_key: TestExtractToolCallsFromMessage#test_no_tool_calls_key().
  TestExtractToolCallsFromMessage.test_tool_calls_not_list: TestExtractToolCallsFromMessage#test_tool_calls_not_list().
  TestExtractToolCallsFromMessage.test_skips_invalid_tool_call_entries: TestExtractToolCallsFromMessage#test_skips_invalid_tool_call_entries().
  TestFindSessionFiles.test_finds_session_files_sorted_by_mtime: TestFindSessionFiles#test_finds_session_files_sorted_by_mtime().
  TestFindSessionFiles.test_empty_dir_returns_empty: TestFindSessionFiles#test_empty_dir_returns_empty().
  TestFindSessionFiles.test_nonexistent_chats_dir_returns_empty: TestFindSessionFiles#test_nonexistent_chats_dir_returns_empty().
  TestFindSessionFiles.test_ignores_non_session_files: TestFindSessionFiles#test_ignores_non_session_files().
  TestLoadNewUsageEntries.test_handles_malformed_json: TestLoadNewUsageEntries#test_handles_malformed_json().
  TestLoadNewUsageEntries.test_empty_dir_returns_empty: TestLoadNewUsageEntries#test_empty_dir_returns_empty().
  TestLoadNewUsageEntries.test_nonexistent_dir_returns_empty: TestLoadNewUsageEntries#test_nonexistent_dir_returns_empty().
  GEMINI_MSG_FULL: GEMINI_MSG_FULL.
  GEMINI_MSG_MINIMAL: GEMINI_MSG_MINIMAL.
  GEMINI_MSG_COMPUTED_TOTAL: GEMINI_MSG_COMPUTED_TOTAL.
  TestExtractTokensFromMessage: TestExtractTokensFromMessage#
  TestExtractToolCallsFromMessage: TestExtractToolCallsFromMessage#
  TestFindSessionFiles: TestFindSessionFiles#
  TestLoadNewUsageEntries: TestLoadNewUsageEntries#
  TestGeminiCostCalculationSubsetStyle: TestGeminiCostCalculationSubsetStyle#
---
# Module: [`tests/test_gemini_session_reader.py`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py)

## Classes
### `TestExtractTokensFromMessage`
- def: [`tests/test_gemini_session_reader.py:70`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L70)
- signature: `class TestExtractTokensFromMessage:`
- members:
  - `test_cache_write_from_session_when_present(self)` — [`L88`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L88) — If session adds cache_write/cacheWrite in future, we read it.
  - `test_cache_write_none_when_absent(self)` — [`L81`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L81) — Gemini session format does not expose cache_write; expect None.
  - `test_computes_total_when_zero(self)` — [`L106`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L106)
  - `test_full_entry_returns_all_buckets(self)` — [`L71`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L71)
  - `test_minimal_entry(self)` — [`L99`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L99)
  - `test_no_tokens_dict_returns_none(self)` — [`L111`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L111)
  - `test_tokens_not_dict_returns_none(self)` — [`L115`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L115)
- uses (calls/refs, reference-scoped): [`extract_tokens_from_message`](../utils/metric_tracking/gemini_session_reader.md#extract_tokens_from_message)  (3 test-only)

### `TestExtractToolCallsFromMessage`
- def: [`tests/test_gemini_session_reader.py:124`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L124)
- signature: `class TestExtractToolCallsFromMessage:`
- members:
  - `test_empty_tool_calls(self)` — [`L131`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L131)
  - `test_extracts_tool_calls(self)` — [`L125`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L125)
  - `test_no_tool_calls_key(self)` — [`L134`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L134)
  - `test_skips_invalid_tool_call_entries(self)` — [`L142`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L142)
  - `test_tool_calls_not_list(self)` — [`L138`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L138)
- uses (calls/refs, reference-scoped): [`extract_tool_calls_from_message`](../utils/metric_tracking/gemini_session_reader.md#extract_tool_calls_from_message)  (2 test-only)

### `TestFindSessionFiles`
- def: [`tests/test_gemini_session_reader.py:157`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L157)
- signature: `class TestFindSessionFiles:`
- members:
  - `test_empty_dir_returns_empty(self, tmp_path)` — [`L172`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L172)
  - `test_finds_session_files_sorted_by_mtime(self, tmp_path)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L158)
  - `test_ignores_non_session_files(self, tmp_path)` — [`L178`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L178)
  - `test_nonexistent_chats_dir_returns_empty(self, tmp_path)` — [`L175`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L175)
- uses (calls/refs, reference-scoped): [`find_session_files`](../utils/metric_tracking/gemini_session_reader.md#find_session_files)

### `TestGeminiCostCalculationSubsetStyle`
- def: [`tests/test_gemini_session_reader.py:289`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L289)
- doc: Verify append_cli_step correctly computes cost when cached is a subset of prompt.
- signature: `class TestGeminiCostCalculationSubsetStyle:`
- members:
  - `test_gemini_subset_cost_uses_uncached_plus_cached_rates(self, tmp_path)` — [`L292`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L292) — Gemini: prompt=total input, cached=subset. Cost = uncached*prompt_rate + cached*cached_rate.
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`append_cli_step`](../utils/data_persistence/llm_logger.md#LLMLogger.append_cli_step)

### `TestLoadNewUsageEntries`
- def: [`tests/test_gemini_session_reader.py:192`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L192)
- signature: `class TestLoadNewUsageEntries:`
- members:
  - `test_deduplication_across_polls(self, tmp_path)` — [`L216`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L216)
  - `test_empty_dir_returns_empty(self, tmp_path)` — [`L274`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L274)
  - `test_handles_malformed_json(self, tmp_path)` — [`L267`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L267)
  - `test_loads_gemini_messages(self, tmp_path)` — [`L197`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L197)
  - `test_nonexistent_dir_returns_empty(self, tmp_path)` — [`L279`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L279)
  - `test_skips_messages_without_id(self, tmp_path)` — [`L255`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L255)
  - `test_skips_non_gemini_messages(self, tmp_path)` — [`L230`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L230)
  - `test_skips_zero_total_entries(self, tmp_path)` — [`L243`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L243)
- protocol/private: `_write_session`[`L193`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L193)
- uses (calls/refs, reference-scoped): [`load_new_usage_entries`](../utils/metric_tracking/gemini_session_reader.md#load_new_usage_entries)

## Module values
- `GEMINI_MSG_COMPUTED_TOTAL` — [`L51`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L51)
- `GEMINI_MSG_FULL` — [`L24`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L24)
- `GEMINI_MSG_MINIMAL` — [`L43`](../../../../../raw/code/continual-harness/tests/test_gemini_session_reader.py#L43)

