---
title: 'Module: tests/test_docker_repl_robustness.py'
type: catalog
provenance: extracted
module: tests/test_docker_repl_robustness.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_docker_repl_robustness`/
symbols:
  make_repl: make_repl().
  teardown_repl: teardown_repl().
  _completion: _completion().
  TestIsolationAndLifecycle.test_two_repls_isolated_state_and_tracking: TestIsolationAndLifecycle#test_two_repls_isolated_state_and_tracking().
  TestRLMQuery.test_rlm_query_batched_basic_order_and_tracking: TestRLMQuery#test_rlm_query_batched_basic_order_and_tracking().
  TestRLMQuery.test_rlm_query_batched_order_preserved_under_varying_delays: TestRLMQuery#test_rlm_query_batched_order_preserved_under_varying_delays().
  TestLLMQuery.test_concurrent_llm_query_from_container_threads: TestLLMQuery#test_concurrent_llm_query_from_container_threads().
  TestRLMQuery.test_rlm_query_uses_subcall_fn: TestRLMQuery#test_rlm_query_uses_subcall_fn().
  TestRLMQuery.test_rlm_query_error_is_caught: TestRLMQuery#test_rlm_query_error_is_caught().
  TestRLMQuery.test_rlm_query_batched_partial_failure_excludes_from_tracking: TestRLMQuery#test_rlm_query_batched_partial_failure_excludes_from_tracking().
  TestRLMQuery.test_rlm_query_batched_respects_max_concurrent: TestRLMQuery#test_rlm_query_batched_respects_max_concurrent().
  TestAnswerSemantics.test_update_handler_address_resets_stale_answer: TestAnswerSemantics#test_update_handler_address_resets_stale_answer().
  TestLLMQuery.test_llm_query_and_tracking: TestLLMQuery#test_llm_query_and_tracking().
  TestRLMQuery.test_rlm_query_fallback_to_llm_when_no_subcall: TestRLMQuery#test_rlm_query_fallback_to_llm_when_no_subcall().
  TestRLMQuery.test_rlm_query_batched_empty: TestRLMQuery#test_rlm_query_batched_empty().
  TestRLMQuery.test_rlm_query_batched_single: TestRLMQuery#test_rlm_query_batched_single().
  TestRLMQuery.test_malformed_subcall_result_does_not_hang: TestRLMQuery#test_malformed_subcall_result_does_not_hang().
  TestRLMQuery.test_mixed_llm_and_rlm_calls_tracked_in_order: TestRLMQuery#test_mixed_llm_and_rlm_calls_tracked_in_order().
  TestStateAndOutput.test_exception_produces_stderr_not_crash: TestStateAndOutput#test_exception_produces_stderr_not_crash().
  TestLLMQuery.test_llm_query_batched_order_and_tracking: TestLLMQuery#test_llm_query_batched_order_and_tracking().
  TestLLMQuery.test_llm_query_no_handler_errors_gracefully: TestLLMQuery#test_llm_query_no_handler_errors_gracefully().
  TestRLMQuery.test_rlm_query_batched_fallback_when_no_subcall: TestRLMQuery#test_rlm_query_batched_fallback_when_no_subcall().
  TestScaffoldRestoration.test_overwritten_rlm_query_restored_next_cell: TestScaffoldRestoration#test_overwritten_rlm_query_restored_next_cell().
  TestCustomTools.test_code_string_and_data_tools: TestCustomTools#test_code_string_and_data_tools().
  TestCustomTools.test_host_callable_tool_skipped_without_crash: TestCustomTools#test_host_callable_tool_skipped_without_crash().
  TestCustomTools.test_data_tool_with_special_characters_roundtrips: TestCustomTools#test_data_tool_with_special_characters_roundtrips().
  TestStateAndOutput.test_large_context_via_mount: TestStateAndOutput#test_large_context_via_mount().
  TestLLMQuery.test_pending_calls_cleared_between_executions: TestLLMQuery#test_pending_calls_cleared_between_executions().
  TestRLMQuery.test_rlm_query_model_override_propagates: TestRLMQuery#test_rlm_query_model_override_propagates().
  TestScaffoldRestoration.test_overwritten_llm_query_restored_next_cell: TestScaffoldRestoration#test_overwritten_llm_query_restored_next_cell().
  TestScaffoldRestoration.test_overwritten_show_vars_restored: TestScaffoldRestoration#test_overwritten_show_vars_restored().
  TestScaffoldRestoration.test_context_alias_restored_after_overwrite: TestScaffoldRestoration#test_context_alias_restored_after_overwrite().
  TestAnswerSemantics.test_answer_ready_surfaces_final_answer: TestAnswerSemantics#test_answer_ready_surfaces_final_answer().
  TestAnswerSemantics.test_answer_not_ready_is_none: TestAnswerSemantics#test_answer_not_ready_is_none().
  TestAnswerSemantics.test_answer_empty_content_surfaces_empty_string: TestAnswerSemantics#test_answer_empty_content_surfaces_empty_string().
  TestAnswerSemantics.test_answer_nonstring_content_coerced: TestAnswerSemantics#test_answer_nonstring_content_coerced().
  TestAnswerSemantics.test_answer_plain_dict_reassignment_surfaces: TestAnswerSemantics#test_answer_plain_dict_reassignment_surfaces().
  TestStateAndOutput.test_unpicklable_dropped_picklable_survives: TestStateAndOutput#test_unpicklable_dropped_picklable_survives().
  TestStateAndOutput.test_unicode_stdout: TestStateAndOutput#test_unicode_stdout().
  TestStateAndOutput.test_output_that_looks_like_json_is_preserved: TestStateAndOutput#test_output_that_looks_like_json_is_preserved().
  TestStateAndOutput.test_empty_code: TestStateAndOutput#test_empty_code().
  TestStateAndOutput.test_dict_context_nested_access: TestStateAndOutput#test_dict_context_nested_access().
  TestIsolationAndLifecycle.test_double_cleanup_idempotent: TestIsolationAndLifecycle#test_double_cleanup_idempotent().
  TestIsolationAndLifecycle.test_context_manager_cleans_up: TestIsolationAndLifecycle#test_context_manager_cleans_up().
  TestRLMQuery.sub: TestRLMQuery#sub().
  EchoLM.get_usage_summary: EchoLM#get_usage_summary().
  EchoLM: EchoLM#
  EchoLM.delay: EchoLM#delay.
  pytestmark: pytestmark.
  EchoLM.__init__: EchoLM#__init__().
  EchoLM.completion: EchoLM#completion().
  EchoLM.acompletion: EchoLM#acompletion().
  EchoLM.get_last_usage: EchoLM#get_last_usage().
  TestCustomTools.test_reserved_name_rejected: TestCustomTools#test_reserved_name_rejected().
  _docker_available: _docker_available().
  TestRLMQuery.boom: TestRLMQuery#boom().
  TestLLMQuery: TestLLMQuery#
  TestRLMQuery: TestRLMQuery#
  TestScaffoldRestoration: TestScaffoldRestoration#
  TestAnswerSemantics: TestAnswerSemantics#
  TestCustomTools: TestCustomTools#
  TestStateAndOutput: TestStateAndOutput#
  TestIsolationAndLifecycle: TestIsolationAndLifecycle#
---
# Module: [`tests/test_docker_repl_robustness.py`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py)

## Classes
### `EchoLM`  ·  implements/extends BaseLM
- def: [`tests/test_docker_repl_robustness.py:44`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L44)
- doc: Deterministic mock LM. Optional delay to exercise concurrency.
- signature: `class EchoLM(BaseLM):`
- members:
  - `acompletion(self, prompt, model=None)` — [`L56`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L56)
  - `completion(self, prompt, model=None)` — [`L51`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L51)
  - `get_last_usage(self)` — [`L64`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L64)
  - `get_usage_summary(self)` — [`L61`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L61)
  - `delay` — [`L49`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L49)
- protocol/private: `__init__`[`L47`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L47)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`__init__`](../rlm/clients/base_lm.md#BaseLM.__init__)
- used by: [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`get_last_usage`](../rlm/clients/base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](../rlm/clients/base_lm.md#BaseLM.get_usage_summary), [`completion`](../rlm/clients/base_lm.md#BaseLM.completion), [`acompletion`](../rlm/clients/base_lm.md#BaseLM.acompletion)  (2 test-only)

### `TestAnswerSemantics`
- def: [`tests/test_docker_repl_robustness.py:385`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L385)
- signature: `class TestAnswerSemantics:`
- members:
  - `test_answer_empty_content_surfaces_empty_string(self)` — [`L402`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L402)
  - `test_answer_nonstring_content_coerced(self)` — [`L410`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L410)
  - `test_answer_not_ready_is_none(self)` — [`L394`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L394)
  - `test_answer_plain_dict_reassignment_surfaces(self)` — [`L418`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L418)
  - `test_answer_ready_surfaces_final_answer(self)` — [`L386`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L386)
  - `test_update_handler_address_resets_stale_answer(self)` — [`L426`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L426) — Regression: stale answer.ready from a prior turn must not leak into
- uses (calls/refs, reference-scoped): [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`final_answer`](../rlm/core/types.md#REPLResult.final_answer), [`update_handler_address`](../rlm/environments/docker_repl.md#DockerREPL.update_handler_address), [`lm_handler_address`](../rlm/environments/docker_repl.md#DockerREPL.lm_handler_address)  (2 test-only)

### `TestCustomTools`
- def: [`tests/test_docker_repl_robustness.py:444`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L444)
- signature: `class TestCustomTools:`
- members:
  - `test_code_string_and_data_tools(self)` — [`L451`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L451)
  - `test_data_tool_with_special_characters_roundtrips(self)` — [`L476`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L476)
  - `test_host_callable_tool_skipped_without_crash(self)` — [`L465`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L465)
  - `test_reserved_name_rejected(self)` — [`L445`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L445)
- uses (calls/refs, reference-scoped): [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`DockerREPL`](../rlm/environments/docker_repl.md#DockerREPL)  (2 test-only)

### `TestIsolationAndLifecycle`
- def: [`tests/test_docker_repl_robustness.py:570`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L570)
- signature: `class TestIsolationAndLifecycle:`
- members:
  - `test_context_manager_cleans_up(self)` — [`L608`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L608)
  - `test_double_cleanup_idempotent(self)` — [`L592`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L592)
  - `test_two_repls_isolated_state_and_tracking(self)` — [`L571`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L571)
- uses (calls/refs, reference-scoped): [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls), [`DockerREPL`](../rlm/environments/docker_repl.md#DockerREPL), [`cleanup`](../rlm/environments/docker_repl.md#DockerREPL.cleanup), [`container_id`](../rlm/environments/docker_repl.md#DockerREPL.container_id), [`temp_dir`](../rlm/environments/docker_repl.md#DockerREPL.temp_dir), [`proxy_port`](../rlm/environments/docker_repl.md#DockerREPL.proxy_port)  (3 test-only)

### `TestLLMQuery`
- def: [`tests/test_docker_repl_robustness.py:102`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L102)
- signature: `class TestLLMQuery:`
- members:
  - `test_concurrent_llm_query_from_container_threads(self)` — [`L141`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L141) — Many concurrent llm_query calls from container threads must all
  - `test_llm_query_and_tracking(self)` — [`L103`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L103)
  - `test_llm_query_batched_order_and_tracking(self)` — [`L112`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L112)
  - `test_llm_query_no_handler_errors_gracefully(self)` — [`L132`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L132)
  - `test_pending_calls_cleared_between_executions(self)` — [`L121`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L121) — A subsequent execution with no LM calls must report zero rlm_calls.
- uses (calls/refs, reference-scoped): [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls)  (3 test-only)

### `TestRLMQuery`
- def: [`tests/test_docker_repl_robustness.py:174`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L174)
- signature: `class TestRLMQuery:`
- members:
  - `boom(p, m=None)` — [`L209`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L209)
  - `sub(p, m=None)` — [`L187`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L187)
  - `test_malformed_subcall_result_does_not_hang(self)` — [`L314`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L314) — If subcall_fn returns a non-completion object, the container must get
  - `test_mixed_llm_and_rlm_calls_tracked_in_order(self)` — [`L329`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L329)
  - `test_rlm_query_batched_basic_order_and_tracking(self)` — [`L221`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L221)
  - `test_rlm_query_batched_empty(self)` — [`L230`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L230)
  - `test_rlm_query_batched_fallback_when_no_subcall(self)` — [`L305`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L305)
  - `test_rlm_query_batched_order_preserved_under_varying_delays(self)` — [`L250`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L250)
  - `test_rlm_query_batched_partial_failure_excludes_from_tracking(self)` — [`L266`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L266)
  - `test_rlm_query_batched_respects_max_concurrent(self)` — [`L282`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L282)
  - `test_rlm_query_batched_single(self)` — [`L241`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L241)
  - `test_rlm_query_error_is_caught(self)` — [`L208`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L208)
  - `test_rlm_query_fallback_to_llm_when_no_subcall(self)` — [`L198`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L198) — No subcall_fn but a handler -> rlm_query degrades to a plain LM call.
  - `test_rlm_query_model_override_propagates(self)` — [`L184`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L184)
  - `test_rlm_query_uses_subcall_fn(self)` — [`L175`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L175)
- uses (calls/refs, reference-scoped): [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls)  (3 test-only)

### `TestScaffoldRestoration`
- def: [`tests/test_docker_repl_robustness.py:344`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L344)
- signature: `class TestScaffoldRestoration:`
- members:
  - `test_context_alias_restored_after_overwrite(self)` — [`L372`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L372)
  - `test_overwritten_llm_query_restored_next_cell(self)` — [`L345`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L345)
  - `test_overwritten_rlm_query_restored_next_cell(self)` — [`L354`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L354)
  - `test_overwritten_show_vars_restored(self)` — [`L363`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L363)
- uses (calls/refs, reference-scoped): [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code)  (3 test-only)

### `TestStateAndOutput`
- def: [`tests/test_docker_repl_robustness.py:495`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L495)
- signature: `class TestStateAndOutput:`
- members:
  - `test_dict_context_nested_access(self)` — [`L558`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L558)
  - `test_empty_code(self)` — [`L537`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L537)
  - `test_exception_produces_stderr_not_crash(self)` — [`L527`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L527)
  - `test_large_context_via_mount(self)` — [`L545`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L545)
  - `test_output_that_looks_like_json_is_preserved(self)` — [`L518`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L518)
  - `test_unicode_stdout(self)` — [`L510`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L510)
  - `test_unpicklable_dropped_picklable_survives(self)` — [`L496`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L496)
- uses (calls/refs, reference-scoped): [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`execute_code`](../rlm/environments/docker_repl.md#DockerREPL.execute_code), [`final_answer`](../rlm/core/types.md#REPLResult.final_answer)  (2 test-only)

## Functions
- `_completion(response: str, model: str | None = None)` — [`L68`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L68)
- `_docker_available()` — [`L29`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L29)
- `make_repl(subcall_fn=None, with_handler=True, **kwargs)` — [`L78`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L78) — Create a DockerREPL (optionally) wired to an EchoLM handler.
- `teardown_repl(repl)` — [`L93`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L93)

## Module values
- `pytestmark` — [`L38`](../../../../../raw/code/rlm/tests/test_docker_repl_robustness.py#L38)

