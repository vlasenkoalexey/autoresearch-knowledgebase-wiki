---
title: 'Module: tests/test_local_repl.py'
type: catalog
provenance: extracted
module: tests/test_local_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_local_repl`/TestLocalREPL
symbols:
  TestLocalREPLPersistence.test_variable_persistence: Persistence#test_variable_persistence().
  TestLocalREPLBasic.test_simple_execution: Basic#test_simple_execution().
  TestLocalREPLPersistence.test_list_comprehension: Persistence#test_list_comprehension().
  TestLocalREPLBuiltins.test_imports_work: Builtins#test_imports_work().
  TestLocalREPLScaffoldRestoration.test_context_restored_after_overwrite: ScaffoldRestoration#test_context_restored_after_overwrite().
  TestLocalREPLSimulatingRLMNoPersistence.test_simulated_rlm_completions_reset_environment: SimulatingRLMNoPersistence#test_simulated_rlm_completions_reset_environment().
  TestLocalREPLSimulatingRLMNoPersistence.test_simulated_rlm_completions_functions_not_preserved: SimulatingRLMNoPersistence#test_simulated_rlm_completions_functions_not_preserved().
  TestLocalREPLBasic.test_print_output: Basic#test_print_output().
  TestLocalREPLBasic.test_error_handling: Basic#test_error_handling().
  TestLocalREPLBasic.test_syntax_error: Basic#test_syntax_error().
  TestLocalREPLPersistence.test_function_persistence: Persistence#test_function_persistence().
  TestLocalREPLBuiltins.test_safe_builtins_available: Builtins#test_safe_builtins_available().
  TestLocalREPLHelpers.test_answer_ready_surfaces_final_answer: Helpers#test_answer_ready_surfaces_final_answer().
  TestLocalREPLHelpers.test_answer_ready_false_does_not_surface: Helpers#test_answer_ready_false_does_not_surface().
  TestLocalREPLHelpers.test_answer_rebind_to_plain_dict: Helpers#test_answer_rebind_to_plain_dict().
  TestLocalREPLHelpers.test_llm_query_no_handler: Helpers#test_llm_query_no_handler().
  TestLocalREPLScaffoldRestoration.test_llm_query_restored_after_overwrite: ScaffoldRestoration#test_llm_query_restored_after_overwrite().
  TestLocalREPLScaffoldRestoration.test_answer_rewrap_after_rebind: ScaffoldRestoration#test_answer_rewrap_after_rebind().
  TestLocalREPLCleanup.test_cleanup_clears_state: Cleanup#test_cleanup_clears_state().
  TestLocalREPLContextManager.test_context_manager: ContextManager#test_context_manager().
  TestLocalREPLHelpers.test_answer_dict_defaults: Helpers#test_answer_dict_defaults().
  TestLocalREPLContext.test_string_context: Context#test_string_context().
  TestLocalREPLContext.test_dict_context: Context#test_dict_context().
  TestLocalREPLContext.test_list_context: Context#test_list_context().
  TestLocalREPLCleanup.test_temp_dir_created_and_cleaned: Cleanup#test_temp_dir_created_and_cleaned().
  TestLocalREPLBasic: Basic#
  TestLocalREPLPersistence: Persistence#
  TestLocalREPLBuiltins: Builtins#
  TestLocalREPLContextManager: ContextManager#
  TestLocalREPLHelpers: Helpers#
  TestLocalREPLContext: Context#
  TestLocalREPLScaffoldRestoration: ScaffoldRestoration#
  TestLocalREPLCleanup: Cleanup#
  TestLocalREPLSimulatingRLMNoPersistence: SimulatingRLMNoPersistence#
---
# Module: [`tests/test_local_repl.py`](../../../../../raw/code/rlm/tests/test_local_repl.py)

## Classes
### `TestLocalREPLBasic`
- def: [`tests/test_local_repl.py:8`](../../../../../raw/code/rlm/tests/test_local_repl.py#L8)
- doc: Basic functionality tests for LocalREPL.
- signature: `class TestLocalREPLBasic:`
- members:
  - `test_error_handling(self)` — [`L26`](../../../../../raw/code/rlm/tests/test_local_repl.py#L26) — Test that errors are captured in stderr.
  - `test_print_output(self)` — [`L19`](../../../../../raw/code/rlm/tests/test_local_repl.py#L19) — Test that print statements are captured.
  - `test_simple_execution(self)` — [`L11`](../../../../../raw/code/rlm/tests/test_local_repl.py#L11) — Test basic code execution.
  - `test_syntax_error(self)` — [`L33`](../../../../../raw/code/rlm/tests/test_local_repl.py#L33) — Test syntax error handling.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestLocalREPLBuiltins`
- def: [`tests/test_local_repl.py:88`](../../../../../raw/code/rlm/tests/test_local_repl.py#L88)
- doc: Tests for safe builtins and blocked functions.
- signature: `class TestLocalREPLBuiltins:`
- members:
  - `test_imports_work(self)` — [`L107`](../../../../../raw/code/rlm/tests/test_local_repl.py#L107) — Test that imports work.
  - `test_safe_builtins_available(self)` — [`L91`](../../../../../raw/code/rlm/tests/test_local_repl.py#L91) — Test that safe builtins are available.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestLocalREPLCleanup`
- def: [`tests/test_local_repl.py:226`](../../../../../raw/code/rlm/tests/test_local_repl.py#L226)
- doc: Tests for cleanup behavior.
- signature: `class TestLocalREPLCleanup:`
- members:
  - `test_cleanup_clears_state(self)` — [`L229`](../../../../../raw/code/rlm/tests/test_local_repl.py#L229) — Test that cleanup clears the namespace.
  - `test_temp_dir_created_and_cleaned(self)` — [`L237`](../../../../../raw/code/rlm/tests/test_local_repl.py#L237) — Test that temp directory is created and cleaned up.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`temp_dir`](../rlm/environments/local_repl.md#LocalREPL.temp_dir)

### `TestLocalREPLContext`
- def: [`tests/test_local_repl.py:165`](../../../../../raw/code/rlm/tests/test_local_repl.py#L165)
- doc: Tests for context loading.
- signature: `class TestLocalREPLContext:`
- members:
  - `test_dict_context(self)` — [`L175`](../../../../../raw/code/rlm/tests/test_local_repl.py#L175) — Test loading dict context.
  - `test_list_context(self)` — [`L183`](../../../../../raw/code/rlm/tests/test_local_repl.py#L183) — Test loading list context.
  - `test_string_context(self)` — [`L168`](../../../../../raw/code/rlm/tests/test_local_repl.py#L168) — Test loading string context.
- uses (calls/refs, reference-scoped): [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestLocalREPLContextManager`
- def: [`tests/test_local_repl.py:116`](../../../../../raw/code/rlm/tests/test_local_repl.py#L116)
- doc: Tests for context manager usage.
- signature: `class TestLocalREPLContextManager:`
- members:
  - `test_context_manager(self)` — [`L119`](../../../../../raw/code/rlm/tests/test_local_repl.py#L119) — Test using LocalREPL as context manager.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL)

### `TestLocalREPLHelpers`
- def: [`tests/test_local_repl.py:126`](../../../../../raw/code/rlm/tests/test_local_repl.py#L126)
- doc: Tests for helper functions and the answer-dict completion signal.
- signature: `class TestLocalREPLHelpers:`
- members:
  - `test_answer_dict_defaults(self)` — [`L129`](../../../../../raw/code/rlm/tests/test_local_repl.py#L129) — The ``answer`` dict starts unready with empty content.
  - `test_answer_ready_false_does_not_surface(self)` — [`L143`](../../../../../raw/code/rlm/tests/test_local_repl.py#L143) — Mutating ``content`` without flipping ``ready`` must not end the run.
  - `test_answer_ready_surfaces_final_answer(self)` — [`L136`](../../../../../raw/code/rlm/tests/test_local_repl.py#L136) — Setting ``answer['ready'] = True`` must surface ``content`` on REPLResult.final_answer.
  - `test_answer_rebind_to_plain_dict(self)` — [`L150`](../../../../../raw/code/rlm/tests/test_local_repl.py#L150) — Rebinding ``answer`` to a plain dict with ready=True is still picked up.
  - `test_llm_query_no_handler(self)` — [`L157`](../../../../../raw/code/rlm/tests/test_local_repl.py#L157) — Test llm_query without handler configured.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`final_answer`](../rlm/core/types.md#REPLResult.final_answer)

### `TestLocalREPLPersistence`
- def: [`tests/test_local_repl.py:41`](../../../../../raw/code/rlm/tests/test_local_repl.py#L41)
- doc: Tests for state persistence across executions.
- signature: `class TestLocalREPLPersistence:`
- members:
  - `test_function_persistence(self)` — [`L61`](../../../../../raw/code/rlm/tests/test_local_repl.py#L61) — Test that defined functions persist.
  - `test_list_comprehension(self)` — [`L76`](../../../../../raw/code/rlm/tests/test_local_repl.py#L76) — Test that list comprehensions work.
  - `test_variable_persistence(self)` — [`L44`](../../../../../raw/code/rlm/tests/test_local_repl.py#L44) — Test that variables persist across multiple code executions.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestLocalREPLScaffoldRestoration`
- def: [`tests/test_local_repl.py:191`](../../../../../raw/code/rlm/tests/test_local_repl.py#L191)
- doc: Tests that overwriting scaffold names (context, llm_query, etc.) is reverted after each execution.
- signature: `class TestLocalREPLScaffoldRestoration:`
- members:
  - `test_answer_rewrap_after_rebind(self)` — [`L215`](../../../../../raw/code/rlm/tests/test_local_repl.py#L215) — If the model rebinds ``answer`` to a plain dict, the next cell still triggers on ready=True.
  - `test_context_restored_after_overwrite(self)` — [`L194`](../../../../../raw/code/rlm/tests/test_local_repl.py#L194) — If the model does context = 'something', the next execution still sees the real context.
  - `test_llm_query_restored_after_overwrite(self)` — [`L206`](../../../../../raw/code/rlm/tests/test_local_repl.py#L206) — If the model does llm_query = lambda x: 'hijacked', the next execution still has real llm_query.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`final_answer`](../rlm/core/types.md#REPLResult.final_answer)

### `TestLocalREPLSimulatingRLMNoPersistence`
- def: [`tests/test_local_repl.py:246`](../../../../../raw/code/rlm/tests/test_local_repl.py#L246)
- doc: Tests simulating RLM's non-persistent completion behavior.
- signature: `class TestLocalREPLSimulatingRLMNoPersistence:`
- members:
  - `test_simulated_rlm_completions_functions_not_preserved(self)` — [`L279`](../../../../../raw/code/rlm/tests/test_local_repl.py#L279) — Simulates 2 RLM completions to show functions don't persist.
  - `test_simulated_rlm_completions_reset_environment(self)` — [`L260`](../../../../../raw/code/rlm/tests/test_local_repl.py#L260) — Simulates 2 RLM completions to show env resets between calls.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

