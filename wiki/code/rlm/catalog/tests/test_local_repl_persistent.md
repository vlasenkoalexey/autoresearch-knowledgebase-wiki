---
title: 'Module: tests/test_local_repl_persistent.py'
type: catalog
provenance: extracted
module: tests/test_local_repl_persistent.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_local_repl_persistent`/TestLocalREPL
symbols:
  TestLocalREPLPersistentState.test_full_persistent_session_simulation: PersistentState#test_full_persistent_session_simulation().
  TestLocalREPLMultiContext.test_contexts_accessible_in_code: MultiContext#test_contexts_accessible_in_code().
  TestLocalREPLMultiContext.test_context_alias_points_to_first: MultiContext#test_context_alias_points_to_first().
  TestLocalREPLHistory.test_history_accessible_via_code: History#test_history_accessible_via_code().
  TestLocalREPLHistory.test_can_iterate_histories_in_code: History#test_can_iterate_histories_in_code().
  TestLocalREPLMultiContext.test_add_context_versioning: MultiContext#test_add_context_versioning().
  TestLocalREPLMultiContext.test_add_context_auto_increment: MultiContext#test_add_context_auto_increment().
  TestLocalREPLHistory.test_add_history_basic: History#test_add_history_basic().
  TestLocalREPLHistory.test_add_multiple_histories: History#test_add_multiple_histories().
  TestLocalREPLPersistentState.test_variables_persist_with_contexts: PersistentState#test_variables_persist_with_contexts().
  TestLocalREPLPersistentState.test_variables_persist_with_histories: PersistentState#test_variables_persist_with_histories().
  TestLocalREPLMultiContext.test_update_handler_address: MultiContext#test_update_handler_address().
  TestLocalREPLHistory.test_history_is_copy: History#test_history_is_copy().
  TestLocalREPLMultiContext: MultiContext#
  TestLocalREPLHistory: History#
  TestLocalREPLPersistentState: PersistentState#
---
# Module: [`tests/test_local_repl_persistent.py`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py)

## Classes
### `TestLocalREPLHistory`
- def: [`tests/test_local_repl_persistent.py:67`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L67)
- doc: Tests for message history storage in LocalREPL for persistent sessions.
- signature: `class TestLocalREPLHistory:`
- members:
  - `test_add_history_basic(self)` — [`L70`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L70) — Test that add_history stores message history correctly.
  - `test_add_multiple_histories(self)` — [`L91`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L91) — Test adding multiple conversation histories.
  - `test_can_iterate_histories_in_code(self)` — [`L134`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L134) — Test iterating through multiple histories in code.
  - `test_history_accessible_via_code(self)` — [`L108`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L108) — Test that stored history is accessible via code execution.
  - `test_history_is_copy(self)` — [`L121`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L121) — Test that stored history is a copy, not a reference.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`add_history`](../rlm/environments/local_repl.md#LocalREPL.add_history), [`get_history_count`](../rlm/environments/local_repl.md#LocalREPL.get_history_count)

### `TestLocalREPLMultiContext`
- def: [`tests/test_local_repl_persistent.py:10`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L10)
- doc: Tests for multi-context support in persistent mode.
- signature: `class TestLocalREPLMultiContext:`
- members:
  - `test_add_context_auto_increment(self)` — [`L31`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L31) — Test that add_context auto-increments when no index provided.
  - `test_add_context_versioning(self)` — [`L13`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L13) — Test that add_context creates versioned variables.
  - `test_context_alias_points_to_first(self)` — [`L54`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L54) — Test that 'context' always aliases context_0.
  - `test_contexts_accessible_in_code(self)` — [`L43`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L43) — Test that multiple contexts can be accessed in code execution.
  - `test_update_handler_address(self)` — [`L24`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L24) — Test handler address can be updated.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`add_context`](../rlm/environments/local_repl.md#LocalREPL.add_context), [`lm_handler_address`](../rlm/environments/local_repl.md#LocalREPL.lm_handler_address), [`get_context_count`](../rlm/environments/local_repl.md#LocalREPL.get_context_count), [`update_handler_address`](../rlm/environments/local_repl.md#LocalREPL.update_handler_address)

### `TestLocalREPLPersistentState`
- def: [`tests/test_local_repl_persistent.py:156`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L156)
- doc: Tests for state persistence across multiple operations in a single REPL instance.
- signature: `class TestLocalREPLPersistentState:`
- members:
  - `test_full_persistent_session_simulation(self)` — [`L189`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L189) — Simulate a multi-turn persistent session.
  - `test_variables_persist_with_contexts(self)` — [`L159`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L159) — Variables and contexts should coexist.
  - `test_variables_persist_with_histories(self)` — [`L174`](../../../../../raw/code/rlm/tests/test_local_repl_persistent.py#L174) — Variables and histories should coexist.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`add_context`](../rlm/environments/local_repl.md#LocalREPL.add_context), [`add_history`](../rlm/environments/local_repl.md#LocalREPL.add_history), [`get_context_count`](../rlm/environments/local_repl.md#LocalREPL.get_context_count), [`get_history_count`](../rlm/environments/local_repl.md#LocalREPL.get_history_count)

