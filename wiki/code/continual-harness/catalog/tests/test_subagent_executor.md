---
title: 'Module: tests/test_subagent_executor.py'
type: catalog
provenance: extracted
module: tests/test_subagent_executor.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_subagent_executor`/
symbols:
  _make_executor: _make_executor().
  sys_path: sys_path.
  TestExecuteCustomSubagent.test_builtin_subagent_rejected: TestExecuteCustomSubagent#test_builtin_subagent_rejected().
  TestRunGenericLoop.test_basic_loop_runs_to_safety_cap: TestRunGenericLoop#test_basic_loop_runs_to_safety_cap().
  TestRunGenericLoop.test_should_continue_fn_can_break: TestRunGenericLoop#test_should_continue_fn_can_break().
  TestRunGenericLoop.test_no_tool_calls_breaks: TestRunGenericLoop#test_no_tool_calls_breaks().
  TestRunGenericLoop.test_on_turn_complete_callback: TestRunGenericLoop#test_on_turn_complete_callback().
  TestExecuteCustomSubagent.test_inline_config_runs: TestExecuteCustomSubagent#test_inline_config_runs().
  TestExecuteCustomSubagent.test_registry_lookup_not_found: TestExecuteCustomSubagent#test_registry_lookup_not_found().
  StubVLM._next: StubVLM#_next().
  _make_runtime: _make_runtime().
  StubVLM: StubVLM#
  TestRunGenericLoop.test_consecutive_vlm_failures_abort: TestRunGenericLoop#test_consecutive_vlm_failures_abort().
  TestExecuteCustomSubagent.test_missing_both_id_and_config: TestExecuteCustomSubagent#test_missing_both_id_and_config().
  TestExecuteCustomSubagent.test_both_id_and_config: TestExecuteCustomSubagent#test_both_id_and_config().
  TestExecuteCustomSubagent.test_forbidden_tools_rejected: TestExecuteCustomSubagent#test_forbidden_tools_rejected().
  TestProcessTrajectoryHistory.test_missing_directive: TestProcessTrajectoryHistory#test_missing_directive().
  TestProcessTrajectoryHistory.test_invalid_window_range: TestProcessTrajectoryHistory#test_invalid_window_range().
  TestProcessTrajectoryHistory.test_successful_analysis: TestProcessTrajectoryHistory#test_successful_analysis().
  TestProcessTrajectoryHistory.test_swapped_range_is_normalized: TestProcessTrajectoryHistory#test_swapped_range_is_normalized().
  TestRunGenericLoop.side_effect: TestRunGenericLoop#side_effect().
  StubVLM.get_query: StubVLM#get_query().
  StubVLM.get_text_query: StubVLM#get_text_query().
  _step_counter: _step_counter.
  StubVLM.responses: StubVLM#responses.
  StubVLM._idx: StubVLM#_idx.
  _make_mock_mcp: _make_mock_mcp().
  _make_run_data_manager: _make_run_data_manager().
  TestRunGenericLoop.no_tools: TestRunGenericLoop#no_tools().
  TestExecuteCustomSubagent.side_effect: TestExecuteCustomSubagent#side_effect().
  StubVLM.__init__: StubVLM#__init__().
  StubVLM.with_tools: StubVLM#with_tools.
  TestRunGenericLoop: TestRunGenericLoop#
  TestExecuteCustomSubagent: TestExecuteCustomSubagent#
  TestProcessTrajectoryHistory: TestProcessTrajectoryHistory#
---
# Module: [`tests/test_subagent_executor.py`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py)

## Classes
### `StubVLM`
- def: [`tests/test_subagent_executor.py:63`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L63)
- doc: VLM stub that returns canned text responses and optionally function calls.
- signature: `class StubVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L71`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L71)
  - `get_text_query(self, prompt, interaction_name)` — [`L74`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L74)
  - `responses` — [`L67`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L67)
  - `with_tools` — [`L69`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L69)
- protocol/private: `__init__`[`L66`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L66), `_idx`[`L68`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L68), `_next`[`L77`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L77)
- used by: (5 test-only callers)

### `TestExecuteCustomSubagent`
- def: [`tests/test_subagent_executor.py:228`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L228)
- signature: `class TestExecuteCustomSubagent:`
- members:
  - `side_effect(response, tool_calls_made, depth, max_depth, **kw)` — [`L259`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L259)
  - `test_both_id_and_config(self, tmp_path)` — [`L235`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L235)
  - `test_builtin_subagent_rejected(self, tmp_path)` — [`L282`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L282) — Attempting to launch a built-in subagent via execute_custom_subagent
  - `test_forbidden_tools_rejected(self, tmp_path)` — [`L245`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L245)
  - `test_inline_config_runs(self, tmp_path)` — [`L258`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L258)
  - `test_missing_both_id_and_config(self, tmp_path)` — [`L229`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L229)
  - `test_registry_lookup_not_found(self, tmp_path)` — [`L301`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L301)
- uses (calls/refs, reference-scoped): [`entries`](../utils/stores/base_store.md#BaseStore.entries), [`SubagentStore`](../utils/stores/subagents.md#SubagentStore), [`execute_custom_subagent`](../agents/subagents/utils/executor.md#SubagentExecutor.execute_custom_subagent), [`is_builtin`](../utils/stores/subagents.md#SubagentEntry.is_builtin)  (1 test-only)

### `TestProcessTrajectoryHistory`
- def: [`tests/test_subagent_executor.py:320`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L320)
- signature: `class TestProcessTrajectoryHistory:`
- members:
  - `test_invalid_window_range(self, tmp_path)` — [`L329`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L329)
  - `test_missing_directive(self, tmp_path)` — [`L321`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L321)
  - `test_successful_analysis(self, tmp_path)` — [`L338`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L338)
  - `test_swapped_range_is_normalized(self, tmp_path)` — [`L358`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L358)
- uses (calls/refs, reference-scoped): [`process_trajectory_history`](../agents/subagents/utils/executor.md#SubagentExecutor.process_trajectory_history)  (1 test-only)

### `TestRunGenericLoop`
- def: [`tests/test_subagent_executor.py:117`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L117)
- signature: `class TestRunGenericLoop:`
- members:
  - `no_tools(response, tool_calls_made, depth, max_depth, **kw)` — [`L164`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L164)
  - `side_effect(response, tool_calls_made, depth, max_depth, **kw)` — [`L122`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L122)
  - `test_basic_loop_runs_to_safety_cap(self, tmp_path)` — [`L118`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L118)
  - `test_consecutive_vlm_failures_abort(self, tmp_path)` — [`L181`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L181) — After MAX_CONSECUTIVE_FAILURES VLM errors, loop aborts.
  - `test_no_tool_calls_breaks(self, tmp_path)` — [`L162`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L162) — If the VLM produces no tool calls, the loop breaks immediately.
  - `test_on_turn_complete_callback(self, tmp_path)` — [`L200`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L200)
  - `test_should_continue_fn_can_break(self, tmp_path)` — [`L141`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L141)
- uses (calls/refs, reference-scoped): [`run_generic_loop`](../agents/subagents/utils/executor.md#SubagentExecutor.run_generic_loop)  (2 test-only)

## Functions
- `_make_executor(tmp_path, *, vlm_stub=None, tool_calls_side_effect=None)` — [`L87`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L87)
- `_make_mock_mcp()` — [`L40`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L40) — MCPToolAdapter mock — returns a minimal game state on every call.
- `_make_run_data_manager(tmp_path)` — [`L55`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L55)
- `_make_runtime()` — [`L28`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L28) — Minimal PokeAgentRuntime with a simple step counter.

## Module values
- `_step_counter` — [`L25`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L25)
- `sys_path` — [`L12`](../../../../../raw/code/continual-harness/tests/test_subagent_executor.py#L12)

