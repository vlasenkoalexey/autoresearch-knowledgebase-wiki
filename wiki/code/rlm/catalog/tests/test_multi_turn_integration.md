---
title: 'Module: tests/test_multi_turn_integration.py'
type: catalog
provenance: extracted
module: tests/test_multi_turn_integration.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_multi_turn_integration`/
symbols:
  create_mock_lm: create_mock_lm().
  TestMultiTurnEndToEnd.test_three_turn_conversation: TestMultiTurnEndToEnd#test_three_turn_conversation().
  final: final().
  TestMultiTurnPersistentEnvironment.test_context_accumulation_across_calls: TestMultiTurnPersistentEnvironment#test_context_accumulation_across_calls().
  TestMultiTurnPersistentEnvironment.test_history_accumulation_across_calls: TestMultiTurnPersistentEnvironment#test_history_accumulation_across_calls().
  TestPersistentModeResourceManagement.test_explicit_close: TestPersistentModeResourceManagement#test_explicit_close().
  TestMultiTurnPersistentEnvironment.test_environment_reused_in_persistent_mode: TestMultiTurnPersistentEnvironment#test_environment_reused_in_persistent_mode().
  TestMultiTurnPersistentEnvironment.test_variable_persistence_across_completions: TestMultiTurnPersistentEnvironment#test_variable_persistence_across_completions().
  TestMultiTurnCodeExecution.test_can_access_previous_context_in_code: TestMultiTurnCodeExecution#test_can_access_previous_context_in_code().
  TestMultiTurnCodeExecution.test_can_access_history_in_code: TestMultiTurnCodeExecution#test_can_access_history_in_code().
  TestNonPersistentMode.test_non_persistent_creates_fresh_environment: TestNonPersistentMode#test_non_persistent_creates_fresh_environment().
  TestPersistentModeResourceManagement.test_context_manager_cleanup: TestPersistentModeResourceManagement#test_context_manager_cleanup().
  TestMultiTurnPromptAwareness.test_prompt_includes_context_count: TestMultiTurnPromptAwareness#test_prompt_includes_context_count().
  TestMultiTurnPromptAwareness.test_prompt_includes_history_count: TestMultiTurnPromptAwareness#test_prompt_includes_history_count().
  TestNonPersistentMode.test_default_is_non_persistent: TestNonPersistentMode#test_default_is_non_persistent().
  TestPersistentModeValidation.test_local_environment_supported: TestPersistentModeValidation#test_local_environment_supported().
  TestPersistentModeValidation.test_docker_environment_supported: TestPersistentModeValidation#test_docker_environment_supported().
  TestPersistentModeValidation.test_unsupported_environment_raises_error: TestPersistentModeValidation#test_unsupported_environment_raises_error().
  TestMultiTurnPersistentEnvironment: TestMultiTurnPersistentEnvironment#
  TestMultiTurnPromptAwareness: TestMultiTurnPromptAwareness#
  TestMultiTurnCodeExecution: TestMultiTurnCodeExecution#
  TestNonPersistentMode: TestNonPersistentMode#
  TestPersistentModeResourceManagement: TestPersistentModeResourceManagement#
  TestPersistentModeValidation: TestPersistentModeValidation#
  TestMultiTurnEndToEnd: TestMultiTurnEndToEnd#
---
# Module: [`tests/test_multi_turn_integration.py`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py)

## Classes
### `TestMultiTurnCodeExecution`
- def: [`tests/test_multi_turn_integration.py:199`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L199)
- doc: Tests for code execution in multi-turn sessions.
- signature: `class TestMultiTurnCodeExecution:`
- members:
  - `test_can_access_history_in_code(self)` — [`L228`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L228) — Code should be able to reference stored histories.
  - `test_can_access_previous_context_in_code(self)` — [`L202`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L202) — Code should be able to reference earlier contexts.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`_persistent_env`](../rlm/core/rlm.md#RLM._persistent_env)  (2 test-only)

### `TestMultiTurnEndToEnd`
- def: [`tests/test_multi_turn_integration.py:366`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L366)
- doc: End-to-end tests simulating realistic multi-turn usage.
- signature: `class TestMultiTurnEndToEnd:`
- members:
  - `test_three_turn_conversation(self)` — [`L369`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L369) — Simulate a 3-turn conversation with context accumulation.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`_persistent_env`](../rlm/core/rlm.md#RLM._persistent_env), [`get_context_count`](../rlm/environments/base_env.md#SupportsPersistence.get_context_count), [`get_history_count`](../rlm/environments/base_env.md#SupportsPersistence.get_history_count)  (2 test-only)

### `TestMultiTurnPersistentEnvironment`
- def: [`tests/test_multi_turn_integration.py:38`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L38)
- doc: Tests for environment persistence across completion calls.
- signature: `class TestMultiTurnPersistentEnvironment:`
- members:
  - `test_context_accumulation_across_calls(self)` — [`L65`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L65) — Verify contexts accumulate: context_0, context_1, etc.
  - `test_environment_reused_in_persistent_mode(self)` — [`L41`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L41) — Verify the same environment instance is reused across completion calls.
  - `test_history_accumulation_across_calls(self)` — [`L91`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L91) — Verify message histories accumulate: history_0, history_1, etc.
  - `test_variable_persistence_across_completions(self)` — [`L119`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L119) — Variables computed in one completion should be available in subsequent ones.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`_persistent_env`](../rlm/core/rlm.md#RLM._persistent_env), [`get_context_count`](../rlm/environments/base_env.md#SupportsPersistence.get_context_count), [`get_history_count`](../rlm/environments/base_env.md#SupportsPersistence.get_history_count)  (2 test-only)

### `TestMultiTurnPromptAwareness`
- def: [`tests/test_multi_turn_integration.py:149`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L149)
- doc: Tests that prompts correctly inform the model about contexts/histories.
- signature: `class TestMultiTurnPromptAwareness:`
- members:
  - `test_prompt_includes_context_count(self)` — [`L152`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L152) — Model should be informed about available contexts.
  - `test_prompt_includes_history_count(self)` — [`L175`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L175) — Model should be informed about available histories.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM)  (2 test-only)

### `TestNonPersistentMode`
- def: [`tests/test_multi_turn_integration.py:255`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L255)
- doc: Tests to ensure non-persistent mode still works correctly.
- signature: `class TestNonPersistentMode:`
- members:
  - `test_default_is_non_persistent(self)` — [`L279`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L279) — Default behavior should be non-persistent.
  - `test_non_persistent_creates_fresh_environment(self)` — [`L258`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L258) — Non-persistent mode should create new environment each call.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`_persistent_env`](../rlm/core/rlm.md#RLM._persistent_env), [`persistent`](../rlm/core/rlm.md#RLM.persistent)  (2 test-only)

### `TestPersistentModeResourceManagement`
- def: [`tests/test_multi_turn_integration.py:288`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L288)
- doc: Tests for proper resource cleanup in persistent mode.
- signature: `class TestPersistentModeResourceManagement:`
- members:
  - `test_context_manager_cleanup(self)` — [`L291`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L291) — Environment should be cleaned up when exiting context manager.
  - `test_explicit_close(self)` — [`L309`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L309) — Calling close() should clean up persistent environment.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`_persistent_env`](../rlm/core/rlm.md#RLM._persistent_env), [`close`](../rlm/core/rlm.md#RLM.close)  (2 test-only)

### `TestPersistentModeValidation`
- def: [`tests/test_multi_turn_integration.py:329`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L329)
- doc: Tests for persistent mode validation.
- signature: `class TestPersistentModeValidation:`
- members:
  - `test_docker_environment_supported(self)` — [`L353`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L353) — Docker environment should support persistent mode (no error at init).
  - `test_local_environment_supported(self)` — [`L342`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L342) — Local environment should support persistent mode.
  - `test_unsupported_environment_raises_error(self)` — [`L332`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L332) — Persistent mode should raise error for unsupported environments.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`persistent`](../rlm/core/rlm.md#RLM.persistent)

## Functions
- `create_mock_lm(responses: list[str])` — [`L20`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L20) — Create a mock LM that returns responses in order.
- `final(content: str)` — [`L33`](../../../../../raw/code/rlm/tests/test_multi_turn_integration.py#L33) — Render a model response that submits ``content`` as the final answer.

