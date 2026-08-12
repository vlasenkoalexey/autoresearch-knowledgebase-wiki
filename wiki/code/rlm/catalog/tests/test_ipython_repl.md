---
title: 'Module: tests/test_ipython_repl.py'
type: catalog
provenance: extracted
module: tests/test_ipython_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_ipython_repl`/
symbols:
  _FakeSubcall.__call__: _FakeSubcall#__call__().
  test_subcall_fn_reentry_into_same_repl_raises.reentering_subcall: test_subcall_fn_reentry_into_same_repl_raises().reentering_subcall().
  test_stale_subcall_completion_not_misattributed_to_next_cell.slow_subcall: test_stale_subcall_completion_not_misattributed_to_next_cell().slow_subcall().
  test_stale_final_answer_not_misattributed_to_next_cell.slow_subcall: test_stale_final_answer_not_misattributed_to_next_cell().slow_subcall().
  test_in_process_subcall_concurrency_is_globally_bounded.slow_subcall: test_in_process_subcall_concurrency_is_globally_bounded().slow_subcall().
  test_subcall_concurrency_is_globally_bounded.slow_subcall: test_subcall_concurrency_is_globally_bounded().slow_subcall().
  BOTH_MODES: BOTH_MODES.
  test_rlm_query_dispatches_to_subcall_fn: test_rlm_query_dispatches_to_subcall_fn().
  test_rlm_query_batched_dispatches: test_rlm_query_batched_dispatches().
  test_stale_subcall_completion_not_misattributed_to_next_cell: test_stale_subcall_completion_not_misattributed_to_next_cell().
  test_stale_final_answer_not_misattributed_to_next_cell: test_stale_final_answer_not_misattributed_to_next_cell().
  test_add_context_versioning: test_add_context_versioning().
  test_add_history_versioning_and_alias: test_add_history_versioning_and_alias().
  test_get_environment_routes_ipython_subprocess: test_get_environment_routes_ipython_subprocess().
  test_rlm_calls_do_not_leak_across_cells: test_rlm_calls_do_not_leak_across_cells().
  test_in_process_scaffold_self_reentry_preserves_outer_state: test_in_process_scaffold_self_reentry_preserves_outer_state().
  test_simple_execution: test_simple_execution().
  test_custom_tool_callable: test_custom_tool_callable().
  test_subprocess_timeout_interrupts_cleanly: test_subprocess_timeout_interrupts_cleanly().
  test_in_process_timeout_no_fire_for_fast_cell: test_in_process_timeout_no_fire_for_fast_cell().
  test_history_is_deep_copied: test_history_is_deep_copied().
  test_context_alias_restored_after_user_overwrites_it: test_context_alias_restored_after_user_overwrites_it().
  test_get_environment_routes_ipython: test_get_environment_routes_ipython().
  test_cell_timeout_zero_treated_as_disabled: test_cell_timeout_zero_treated_as_disabled().
  test_subcall_fn_reentry_into_same_repl_raises: test_subcall_fn_reentry_into_same_repl_raises().
  test_concurrent_execute_does_not_lose_rlm_calls: test_concurrent_execute_does_not_lose_rlm_calls().
  test_in_process_two_instances_have_distinct_user_modules: test_in_process_two_instances_have_distinct_user_modules().
  test_subcall_concurrency_is_globally_bounded: test_subcall_concurrency_is_globally_bounded().
  _has_subprocess: _has_subprocess.
  test_error_captured_in_stderr: test_error_captured_in_stderr().
  test_variable_persistence_across_cells: test_variable_persistence_across_cells().
  test_answer_ready_surfaces_final_answer: test_answer_ready_surfaces_final_answer().
  test_answer_not_ready_returns_none: test_answer_not_ready_returns_none().
  test_answer_content_is_stringified: test_answer_content_is_stringified().
  test_load_context_string: test_load_context_string().
  test_load_context_dict: test_load_context_dict().
  test_custom_tool_data: test_custom_tool_data().
  test_rlm_query_falls_back_when_no_subcall_fn: test_rlm_query_falls_back_when_no_subcall_fn().
  test_subprocess_no_timeout_by_default: test_subprocess_no_timeout_by_default().
  test_in_process_timeout_interrupts_python_loop: test_in_process_timeout_interrupts_python_loop().
  test_in_process_shell_alive_after_timeout: test_in_process_shell_alive_after_timeout().
  test_init_failure_preserves_original_exception_over_cleanup_error: test_init_failure_preserves_original_exception_over_cleanup_error().
  test_cleanup_is_idempotent: test_cleanup_is_idempotent().
  test_update_handler_address: test_update_handler_address().
  test_in_process_persistent_multi_turn_variables: test_in_process_persistent_multi_turn_variables().
  test_cleanup_unregisters_atexit_handler: test_cleanup_unregisters_atexit_handler().
  test_in_process_cell_cannot_reenter_via_scaffold_self: test_in_process_cell_cannot_reenter_via_scaffold_self().
  test_concurrent_add_context_indices_are_unique: test_concurrent_add_context_indices_are_unique().
  test_in_process_subcall_concurrency_is_globally_bounded: test_in_process_subcall_concurrency_is_globally_bounded().
  test_concurrent_execute_does_not_lose_rlm_calls.worker: test_concurrent_execute_does_not_lose_rlm_calls().worker().
  test_in_process_exposes_locals_dict: test_in_process_exposes_locals_dict().
  test_in_process_timeout_interrupts_c_level_sleep: test_in_process_timeout_interrupts_c_level_sleep().
  test_persistent_env_exposes_protocol: test_persistent_env_exposes_protocol().
  test_in_process_error_includes_traceback_and_user_frame: test_in_process_error_includes_traceback_and_user_frame().
  test_in_process_input_is_disabled: test_in_process_input_is_disabled().
  test_in_process_input_restored_if_user_overwrites: test_in_process_input_restored_if_user_overwrites().
  test_in_process_user_module_dropped_from_sys_modules_on_cleanup: test_in_process_user_module_dropped_from_sys_modules_on_cleanup().
  test_setup_failure_runs_cleanup: test_setup_failure_runs_cleanup().
  _FakeSubcall.responses: _FakeSubcall#responses.
  _can_alarm: _can_alarm.
  _FakeSubcall: _FakeSubcall#
  _FakeSubcall.calls: _FakeSubcall#calls.
  test_subcall_timeout_none_is_allowed: test_subcall_timeout_none_is_allowed().
  test_init_failure_preserves_original_exception_over_cleanup_error._broken_setup: test_init_failure_preserves_original_exception_over_cleanup_error()._broken_setup().
  test_subcall_fn_reentry_into_same_repl_raises.runner: test_subcall_fn_reentry_into_same_repl_raises().runner().
  test_concurrent_add_context_indices_are_unique.worker: test_concurrent_add_context_indices_are_unique().worker().
  test_cleanup_unregisters_atexit_handler.sentinel: test_cleanup_unregisters_atexit_handler().sentinel().
  _FakeSubcall.__post_init__: _FakeSubcall#__post_init__().
  test_invalid_kernel_mode_rejected: test_invalid_kernel_mode_rejected().
  test_invalid_startup_timeout_rejected: test_invalid_startup_timeout_rejected().
  test_invalid_subcall_timeout_rejected: test_invalid_subcall_timeout_rejected().
  test_ipython_repl_importable_from_package: test_ipython_repl_importable_from_package().
  _FakeSubcall._i: _FakeSubcall#_i.
  test_init_failure_preserves_original_exception_over_cleanup_error._Boom: test_init_failure_preserves_original_exception_over_cleanup_error()._Boom#
  test_custom_tool_callable.greet: test_custom_tool_callable().greet().
  test_init_failure_preserves_original_exception_over_cleanup_error._broken_cleanup: test_init_failure_preserves_original_exception_over_cleanup_error()._broken_cleanup().
  test_setup_failure_runs_cleanup._Unserializable: test_setup_failure_runs_cleanup()._Unserializable#
---
# Module: [`tests/test_ipython_repl.py`](../../../../../raw/code/rlm/tests/test_ipython_repl.py)

## Classes
### `_Boom`  ·  implements/extends Exception
- def: [`tests/test_ipython_repl.py:342`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L342)
- signature: `class _Boom(Exception):`
- used by: (2 test-only callers)

### `_FakeSubcall`
- def: [`tests/test_ipython_repl.py:52`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L52)
- doc: A stand-in for RLM._subcall that records calls and returns canned responses.
- signature: `class _FakeSubcall:`
- members:
  - `calls` — [`L56`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L56)
  - `responses` — [`L55`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L55)
- protocol/private: `__call__`[`L62`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L62), `__post_init__`[`L58`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L58), `_i`[`L60`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L60)
- uses (calls/refs, reference-scoped): [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../rlm/core/types.md#RLMChatCompletion), [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`usage_summary`](../rlm/core/types.md#RLMChatCompletion.usage_summary), [`execution_time`](../rlm/core/types.md#RLMChatCompletion.execution_time), [`prompt`](../rlm/core/types.md#RLMChatCompletion.prompt), [`root_model`](../rlm/core/types.md#RLMChatCompletion.root_model)
- used by: (5 test-only callers)

### `_Unserializable`
- def: [`tests/test_ipython_repl.py:1028`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L1028)
- signature: `class _Unserializable:`
- used by: (1 test-only callers)

## Functions
- `_broken_cleanup(self)` — [`L353`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L353)
- `_broken_setup(self)` — [`L347`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L347)
- `greet(name: str)` — [`L175`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L175)
- `reentering_subcall(prompt: str, model: str | None = None)` — [`L780`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L780)
- `runner()` — [`L812`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L812)
- `sentinel()` — [`L584`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L584)
- `slow_subcall(prompt: str, model: str | None = None)` — [`L618`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L618)
- `slow_subcall(prompt: str, model: str | None = None)` — [`L670`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L670)
- `slow_subcall(prompt: str, model: str | None = None)` — [`L922`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L922)
- `slow_subcall(prompt: str, model: str | None = None)` — [`L973`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L973)
- `test_add_context_versioning(kernel_mode: str)` — [`L384`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L384)
- `test_add_history_versioning_and_alias(kernel_mode: str)` — [`L398`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L398)
- `test_answer_content_is_stringified(kernel_mode: str)` — [`L141`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L141)
- `test_answer_not_ready_returns_none(kernel_mode: str)` — [`L134`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L134)
- `test_answer_ready_surfaces_final_answer(kernel_mode: str)` — [`L127`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L127)
- `test_cell_timeout_zero_treated_as_disabled(kernel_mode: str)` — [`L521`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L521) — ``cell_timeout=0`` is meaningless; treated as ``None``.
- `test_cleanup_is_idempotent(kernel_mode: str)` — [`L363`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L363)
- `test_cleanup_unregisters_atexit_handler()` — [`L569`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L569) — Cleanup must remove ``InteractiveShell.atexit_operations`` from the
- `test_concurrent_add_context_indices_are_unique(kernel_mode: str)` — [`L888`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L888) — Two threads calling ``add_context`` concurrently must not collide.
- `test_concurrent_execute_does_not_lose_rlm_calls(kernel_mode: str)` — [`L829`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L829) — Two threads each running an ``rlm_query`` cell must each report
- `test_context_alias_restored_after_user_overwrites_it(kernel_mode: str)` — [`L436`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L436) — If user code reassigns ``context``, the next cell sees it restored.
- `test_custom_tool_callable(kernel_mode: str)` — [`L174`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L174)
- `test_custom_tool_data(kernel_mode: str)` — [`L187`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L187)
- `test_error_captured_in_stderr(kernel_mode: str)` — [`L98`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L98)
- `test_get_environment_routes_ipython()` — [`L463`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L463)
- `test_get_environment_routes_ipython_subprocess()` — [`L476`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L476)
- `test_history_is_deep_copied(kernel_mode: str)` — [`L414`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L414)
- `test_in_process_cell_cannot_reenter_via_scaffold_self()` — [`L720`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L720) — An in-process cell that traverses any scaffold bound method's
- `test_in_process_error_includes_traceback_and_user_frame()` — [`L535`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L535) — In-process stderr should include a real traceback, not just a one-liner.
- `test_in_process_exposes_locals_dict()` — [`L113`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L113) — In-process mode mirrors LocalREPL's .locals dict for parity.
- `test_in_process_input_is_disabled()` — [`L554`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L554) — ``input()`` must not block in cells; it should raise.
- `test_in_process_input_restored_if_user_overwrites()` — [`L561`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L561) — If a cell rebinds ``input``, the next cell must still see the disabled stub.
- `test_in_process_persistent_multi_turn_variables()` — [`L448`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L448) — Variables defined in one cell are visible in later add_context calls.
- `test_in_process_scaffold_self_reentry_preserves_outer_state()` — [`L741`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L741) — If the LM tries to reenter and we raise, the *outer* cell's
- `test_in_process_shell_alive_after_timeout()` — [`L295`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L295)
- `test_in_process_subcall_concurrency_is_globally_bounded()` — [`L910`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L910) — In-process mode also caps ``subcall_fn`` globally, matching subprocess.
- `test_in_process_timeout_interrupts_c_level_sleep()` — [`L275`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L275)
- `test_in_process_timeout_interrupts_python_loop()` — [`L285`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L285)
- `test_in_process_timeout_no_fire_for_fast_cell()` — [`L303`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L303)
- `test_in_process_two_instances_have_distinct_user_modules()` — [`L855`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L855) — Two coexisting in-process instances must not share ``sys.modules['__main__']``.
- `test_in_process_user_module_dropped_from_sys_modules_on_cleanup()` — [`L876`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L876) — No ``sys.modules`` leak after cleanup.
- `test_init_failure_preserves_original_exception_over_cleanup_error(monkeypatch)` — [`L338`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L338) — If ``setup`` fails *and* cleanup would also fail, ``__init__``
- `test_invalid_kernel_mode_rejected()` — [`L315`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L315)
- `test_invalid_startup_timeout_rejected(bad)` — [`L321`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L321)
- `test_invalid_subcall_timeout_rejected(bad)` — [`L327`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L327)
- `test_ipython_repl_importable_from_package()` — [`L488`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L488) — ``IPythonREPL`` is in ``__all__`` and must be importable lazily.
- `test_load_context_dict(kernel_mode: str)` — [`L160`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L160)
- `test_load_context_string(kernel_mode: str)` — [`L153`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L153)
- `test_persistent_env_exposes_protocol(kernel_mode: str)` — [`L376`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L376)
- `test_rlm_calls_do_not_leak_across_cells(kernel_mode: str)` — [`L501`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L501) — Each REPLResult.rlm_calls must reflect only the current cell's calls.
- `test_rlm_query_batched_dispatches(kernel_mode: str)` — [`L215`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L215)
- `test_rlm_query_dispatches_to_subcall_fn(kernel_mode: str)` — [`L202`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L202)
- `test_rlm_query_falls_back_when_no_subcall_fn(kernel_mode: str)` — [`L227`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L227) — Without subcall_fn, rlm_query falls through to llm_query (which errors
- `test_setup_failure_runs_cleanup()` — [`L1019`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L1019) — If construction fails after the broker/kernel start, cleanup runs.
- `test_simple_execution(kernel_mode: str)` — [`L90`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L90)
- `test_stale_final_answer_not_misattributed_to_next_cell()` — [`L664`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L664) — A final answer set by a prior cell's delayed code path must not
- `test_stale_subcall_completion_not_misattributed_to_next_cell()` — [`L607`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L607) — A subcall_fn that finishes *during* a subsequent cell — because the
- `test_subcall_concurrency_is_globally_bounded()` — [`L963`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L963) — ``max_concurrent_subcalls`` caps simultaneous ``subcall_fn`` calls
- `test_subcall_fn_reentry_into_same_repl_raises(kernel_mode: str)` — [`L772`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L772) — If subcall_fn calls execute_code on its parent REPL, the call must
- `test_subcall_timeout_none_is_allowed()` — [`L332`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L332) — ``None`` is the documented "no timeout" sentinel, distinct from 0.
- `test_subprocess_no_timeout_by_default()` — [`L259`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L259) — Without cell_timeout, short code runs without issue.
- `test_subprocess_timeout_interrupts_cleanly()` — [`L243`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L243)
- `test_update_handler_address(kernel_mode: str)` — [`L425`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L425)
- `test_variable_persistence_across_cells(kernel_mode: str)` — [`L105`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L105)
- `worker(repl: IPythonREPL)` — [`L837`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L837)
- `worker(i: int)` — [`L894`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L894)

## Module values
- `BOTH_MODES` — [`L36`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L36)
- `_can_alarm` — [`L271`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L271)
- `_has_subprocess` — [`L28`](../../../../../raw/code/rlm/tests/test_ipython_repl.py#L28)

