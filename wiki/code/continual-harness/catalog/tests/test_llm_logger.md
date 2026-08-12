---
title: 'Module: tests/test_llm_logger.py'
type: catalog
provenance: extracted
module: tests/test_llm_logger.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_llm_logger`/
symbols:
  TestCumulativeMetricsPersistence.test_save_and_load_cumulative_metrics_roundtrip: TestCumulativeMetricsPersistence#test_save_and_load_cumulative_metrics_roundtrip().
  TestStepsNoTruncation.test_more_than_1000_steps_preserved: TestStepsNoTruncation#test_more_than_1000_steps_preserved().
  TestCumulativeMetricsPersistence.test_load_cumulative_metrics_missing_file_returns_false: TestCumulativeMetricsPersistence#test_load_cumulative_metrics_missing_file_returns_false().
  TestCheckpointNoCumulativeMetrics.test_save_checkpoint_does_not_include_cumulative_metrics: TestCheckpointNoCumulativeMetrics#test_save_checkpoint_does_not_include_cumulative_metrics().
  TestCheckpointNoCumulativeMetrics.test_load_checkpoint_does_not_overlay_metrics: TestCheckpointNoCumulativeMetrics#test_load_checkpoint_does_not_overlay_metrics().
  TestBackupRestoreWithoutMetricsFile.test_no_metrics_file_starts_fresh: TestBackupRestoreWithoutMetricsFile#test_no_metrics_file_starts_fresh().
  TestAgentStepInJsonl.test_log_interaction_embeds_agent_step_from_env: TestAgentStepInJsonl#test_log_interaction_embeds_agent_step_from_env().
  TestAgentStepInJsonl.test_log_thinking_embeds_agent_step_argument: TestAgentStepInJsonl#test_log_thinking_embeds_agent_step_argument().
  sys_path: sys_path.
  TestStepsNoTruncation._get_cache_path: TestStepsNoTruncation#_get_cache_path().
  TestCumulativeMetricsPersistence: TestCumulativeMetricsPersistence#
  TestCheckpointNoCumulativeMetrics: TestCheckpointNoCumulativeMetrics#
  TestStepsNoTruncation: TestStepsNoTruncation#
  TestBackupRestoreWithoutMetricsFile: TestBackupRestoreWithoutMetricsFile#
  TestAgentStepInJsonl: TestAgentStepInJsonl#
---
# Module: [`tests/test_llm_logger.py`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py)

## Classes
### `TestAgentStepInJsonl`
- def: [`tests/test_llm_logger.py:148`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L148)
- doc: SSE/UI: each log line should carry the global agent step when known.
- signature: `class TestAgentStepInJsonl:`
- members:
  - `test_log_interaction_embeds_agent_step_from_env(self, monkeypatch)` — [`L151`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L151)
  - `test_log_thinking_embeds_agent_step_argument(self)` — [`L175`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L175)
- uses (calls/refs, reference-scoped): [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`log_file`](../utils/data_persistence/llm_logger.md#LLMLogger.log_file), [`log_interaction`](../utils/data_persistence/llm_logger.md#LLMLogger.log_interaction), [`log_thinking`](../utils/data_persistence/llm_logger.md#LLMLogger.log_thinking)

### `TestBackupRestoreWithoutMetricsFile`
- def: [`tests/test_llm_logger.py:130`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L130)
- doc: Test restore from backup with checkpoint but no cumulative_metrics.json.
- signature: `class TestBackupRestoreWithoutMetricsFile:`
- members:
  - `test_no_metrics_file_starts_fresh(self)` — [`L133`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L133)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`load_cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.load_cumulative_metrics)

### `TestCheckpointNoCumulativeMetrics`
- def: [`tests/test_llm_logger.py:54`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L54)
- doc: Test that checkpoint_llm.txt no longer embeds cumulative_metrics.
- signature: `class TestCheckpointNoCumulativeMetrics:`
- members:
  - `test_load_checkpoint_does_not_overlay_metrics(self)` — [`L74`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L74)
  - `test_save_checkpoint_does_not_include_cumulative_metrics(self)` — [`L57`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L57)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`save_checkpoint`](../utils/data_persistence/llm_logger.md#LLMLogger.save_checkpoint), [`load_checkpoint`](../utils/data_persistence/llm_logger.md#LLMLogger.load_checkpoint)

### `TestCumulativeMetricsPersistence`
- def: [`tests/test_llm_logger.py:20`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L20)
- doc: Test save/load of cumulative_metrics.json.
- signature: `class TestCumulativeMetricsPersistence:`
- members:
  - `test_load_cumulative_metrics_missing_file_returns_false(self)` — [`L23`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L23)
  - `test_save_and_load_cumulative_metrics_roundtrip(self)` — [`L33`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L33)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`save_cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.save_cumulative_metrics), [`load_cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.load_cumulative_metrics)

### `TestStepsNoTruncation`
- def: [`tests/test_llm_logger.py:98`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L98)
- doc: Test that steps array is no longer truncated at 1000.
- signature: `class TestStepsNoTruncation:`
- members:
  - `test_more_than_1000_steps_preserved(self)` — [`L101`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L101)
- protocol/private: `_get_cache_path`[`L107`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L107)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`LLMLogger`](../utils/data_persistence/llm_logger.md#LLMLogger), [`log_interaction`](../utils/data_persistence/llm_logger.md#LLMLogger.log_interaction)

## Module values
- `sys_path` — [`L13`](../../../../../raw/code/continual-harness/tests/test_llm_logger.py#L13)

