---
title: 'Module: tests/test_llm_logger_metrics.py'
type: catalog
provenance: extracted
module: tests/test_llm_logger_metrics.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_llm_logger_metrics`/
symbols:
  _make_logger: _make_logger().
  TestLoadRestoresActionTracking.test_restore_milestone_actions_after_load: TestLoadRestoresActionTracking#test_restore_milestone_actions_after_load().
  TestLoadRestoresActionTracking.test_restore_objective_actions_after_load: TestLoadRestoresActionTracking#test_restore_objective_actions_after_load().
  TestAddStepToolCalls.test_attaches_to_existing_step: TestAddStepToolCalls#test_attaches_to_existing_step().
  TestIncrementActionCount.test_increment_by_default: TestIncrementActionCount#test_increment_by_default().
  TestIncrementActionCount.test_increment_by_n: TestIncrementActionCount#test_increment_by_n().
  TestAddStepToolCalls.test_creates_entry_if_missing: TestAddStepToolCalls#test_creates_entry_if_missing().
  TestLogMilestoneWithActions.test_first_milestone_cumulative_and_split: TestLogMilestoneWithActions#test_first_milestone_cumulative_and_split().
  TestLogMilestoneWithActions.test_second_milestone_split_is_delta: TestLogMilestoneWithActions#test_second_milestone_split_is_delta().
  TestLogMilestoneWithActions.test_three_milestones_split_chain: TestLogMilestoneWithActions#test_three_milestones_split_chain().
  TestLogMilestoneWithActions.test_milestone_preserves_token_fields: TestLogMilestoneWithActions#test_milestone_preserves_token_fields().
  TestLogObjectiveWithActions.test_first_objective_cumulative_and_split: TestLogObjectiveWithActions#test_first_objective_cumulative_and_split().
  TestLogObjectiveWithActions.test_second_objective_split_is_delta: TestLogObjectiveWithActions#test_second_objective_split_is_delta().
  TestLogObjectiveWithActions.test_objective_preserves_category_and_index: TestLogObjectiveWithActions#test_objective_preserves_category_and_index().
  TestMilestoneSplitDeltas.test_split_steps_are_deltas: TestMilestoneSplitDeltas#test_split_steps_are_deltas().
  TestMilestoneSplitDeltas.test_split_time_is_delta: TestMilestoneSplitDeltas#test_split_time_is_delta().
  TestMilestoneSplitDeltas.test_split_tokens_are_deltas: TestMilestoneSplitDeltas#test_split_tokens_are_deltas().
  sys_path: sys_path.
  _add_step_entry: _add_step_entry().
  TestIncrementActionCount: TestIncrementActionCount#
  TestAddStepToolCalls: TestAddStepToolCalls#
  TestLogMilestoneWithActions: TestLogMilestoneWithActions#
  TestLogObjectiveWithActions: TestLogObjectiveWithActions#
  TestMilestoneSplitDeltas: TestMilestoneSplitDeltas#
  TestLoadRestoresActionTracking: TestLoadRestoresActionTracking#
---
# Module: [`tests/test_llm_logger_metrics.py`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py)

## Classes
### `TestAddStepToolCalls`
- def: [`tests/test_llm_logger_metrics.py:57`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L57)
- signature: `class TestAddStepToolCalls:`
- members:
  - `test_attaches_to_existing_step(self)` — [`L59`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L59)
  - `test_creates_entry_if_missing(self)` — [`L73`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L73)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`add_step_tool_calls`](../utils/data_persistence/llm_logger.md#LLMLogger.add_step_tool_calls)  (2 test-only)

### `TestIncrementActionCount`
- def: [`tests/test_llm_logger_metrics.py:40`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L40)
- signature: `class TestIncrementActionCount:`
- members:
  - `test_increment_by_default(self)` — [`L42`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L42)
  - `test_increment_by_n(self)` — [`L49`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L49)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`increment_action_count`](../utils/data_persistence/llm_logger.md#LLMLogger.increment_action_count)  (1 test-only)

### `TestLoadRestoresActionTracking`
- def: [`tests/test_llm_logger_metrics.py:228`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L228)
- doc: Verify that load_cumulative_metrics restores _last_*_actions from saved entries.
- signature: `class TestLoadRestoresActionTracking:`
- members:
  - `test_restore_milestone_actions_after_load(self)` — [`L231`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L231)
  - `test_restore_objective_actions_after_load(self)` — [`L250`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L250)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`log_milestone_completion`](../utils/data_persistence/llm_logger.md#LLMLogger.log_milestone_completion), [`save_cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.save_cumulative_metrics), [`load_cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.load_cumulative_metrics), [`log_objective_completion`](../utils/data_persistence/llm_logger.md#LLMLogger.log_objective_completion)  (1 test-only)

### `TestLogMilestoneWithActions`
- def: [`tests/test_llm_logger_metrics.py:82`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L82)
- signature: `class TestLogMilestoneWithActions:`
- members:
  - `test_first_milestone_cumulative_and_split(self)` — [`L84`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L84)
  - `test_milestone_preserves_token_fields(self)` — [`L124`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L124) — Action tracking shouldn't break existing token fields.
  - `test_second_milestone_split_is_delta(self)` — [`L96`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L96)
  - `test_three_milestones_split_chain(self)` — [`L110`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L110)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`log_milestone_completion`](../utils/data_persistence/llm_logger.md#LLMLogger.log_milestone_completion)  (1 test-only)

### `TestLogObjectiveWithActions`
- def: [`tests/test_llm_logger_metrics.py:141`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L141)
- signature: `class TestLogObjectiveWithActions:`
- members:
  - `test_first_objective_cumulative_and_split(self)` — [`L143`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L143)
  - `test_objective_preserves_category_and_index(self)` — [`L175`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L175)
  - `test_second_objective_split_is_delta(self)` — [`L157`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L157)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`log_objective_completion`](../utils/data_persistence/llm_logger.md#LLMLogger.log_objective_completion)  (1 test-only)

### `TestMilestoneSplitDeltas`
- def: [`tests/test_llm_logger_metrics.py:187`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L187)
- doc: Verify that split metrics for milestones are correct deltas between consecutive milestones.
- signature: `class TestMilestoneSplitDeltas:`
- members:
  - `test_split_steps_are_deltas(self)` — [`L190`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L190)
  - `test_split_time_is_delta(self)` — [`L202`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L202)
  - `test_split_tokens_are_deltas(self)` — [`L211`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L211)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`log_milestone_completion`](../utils/data_persistence/llm_logger.md#LLMLogger.log_milestone_completion)  (1 test-only)

## Functions
- `_add_step_entry(logger: LLMLogger, step: int)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L27) — Simulate a log_interaction that creates a step entry (minimal token usage).
- `_make_logger(tmpdir: str)` — [`L18`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L18) — Create an LLMLogger wired to a temp directory.

## Module values
- `sys_path` — [`L11`](../../../../../raw/code/continual-harness/tests/test_llm_logger_metrics.py#L11)

