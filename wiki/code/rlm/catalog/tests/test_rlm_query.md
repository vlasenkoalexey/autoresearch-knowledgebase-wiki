---
title: 'Module: tests/test_rlm_query.py'
type: catalog
provenance: extracted
module: tests/test_rlm_query.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_rlm_query`/
symbols:
  _make_completion: _make_completion().
  TestRlmQueryBatchedWithSubcallFn.test_batched_calls_subcall_fn_per_prompt: TestRlmQueryBatchedWithSubcallFn#test_batched_calls_subcall_fn_per_prompt().
  TestRlmQueryBatchedParallel.test_batched_pending_calls_ordered: TestRlmQueryBatchedParallel#test_batched_pending_calls_ordered().
  TestMaxConcurrentSubcallsBounds.test_pending_calls_exclude_failures: TestMaxConcurrentSubcallsBounds#test_pending_calls_exclude_failures().
  TestRlmQueryWithSubcallFn.test_rlm_query_uses_subcall_fn: TestRlmQueryWithSubcallFn#test_rlm_query_uses_subcall_fn().
  TestRlmQueryWithSubcallFn.test_rlm_query_tracks_pending_calls: TestRlmQueryWithSubcallFn#test_rlm_query_tracks_pending_calls().
  TestRlmQueryBatchedWithSubcallFn.test_batched_tracks_all_pending_calls: TestRlmQueryBatchedWithSubcallFn#test_batched_tracks_all_pending_calls().
  TestRlmQueryBatchedWithSubcallFn.test_batched_partial_failure: TestRlmQueryBatchedWithSubcallFn#test_batched_partial_failure().
  TestRlmQueryBatchedParallel.test_batched_runs_in_parallel: TestRlmQueryBatchedParallel#test_batched_runs_in_parallel().
  TestRlmQueryBatchedParallel.test_batched_preserves_order_parallel: TestRlmQueryBatchedParallel#test_batched_preserves_order_parallel().
  TestRlmQueryBatchedParallel.test_batched_parallel_partial_failure: TestRlmQueryBatchedParallel#test_batched_parallel_partial_failure().
  TestMaxConcurrentSubcallsBounds.test_max_concurrent_subcalls_one: TestMaxConcurrentSubcallsBounds#test_max_concurrent_subcalls_one().
  TestMaxConcurrentSubcallsBounds.test_max_concurrent_subcalls_larger_than_prompts: TestMaxConcurrentSubcallsBounds#test_max_concurrent_subcalls_larger_than_prompts().
  TestMaxConcurrentSubcallsBounds.test_batched_all_failures_parallel: TestMaxConcurrentSubcallsBounds#test_batched_all_failures_parallel().
  TestMaxConcurrentSubcallsBounds.test_batched_large_batch_with_low_concurrency: TestMaxConcurrentSubcallsBounds#test_batched_large_batch_with_low_concurrency().
  TestRlmQueryWithSubcallFn.test_rlm_query_with_model_override: TestRlmQueryWithSubcallFn#test_rlm_query_with_model_override().
  TestRlmQueryWithSubcallFn.test_rlm_query_error_handling: TestRlmQueryWithSubcallFn#test_rlm_query_error_handling().
  TestRlmQueryBatchedWithSubcallFn.test_batched_single_prompt: TestRlmQueryBatchedWithSubcallFn#test_batched_single_prompt().
  TestLlmQueryDoesNotUseSubcallFn.test_llm_query_ignores_subcall_fn: TestLlmQueryDoesNotUseSubcallFn#test_llm_query_ignores_subcall_fn().
  TestLlmQueryDoesNotUseSubcallFn.test_llm_query_batched_ignores_subcall_fn: TestLlmQueryDoesNotUseSubcallFn#test_llm_query_batched_ignores_subcall_fn().
  TestRlmQueryBatchedParallel.test_batched_respects_max_concurrent: TestRlmQueryBatchedParallel#test_batched_respects_max_concurrent().
  TestRlmQueryBatchedParallel.test_single_prompt_skips_thread_pool: TestRlmQueryBatchedParallel#test_single_prompt_skips_thread_pool().
  TestMaxConcurrentSubcallsBounds.test_max_concurrent_subcalls_exact_match: TestMaxConcurrentSubcallsBounds#test_max_concurrent_subcalls_exact_match().
  TestRlmQueryScaffoldRestoration.test_rlm_query_restored_after_overwrite: TestRlmQueryScaffoldRestoration#test_rlm_query_restored_after_overwrite().
  TestRlmQueryScaffoldRestoration.test_rlm_query_batched_restored_after_overwrite: TestRlmQueryScaffoldRestoration#test_rlm_query_batched_restored_after_overwrite().
  TestRlmQueryWithoutSubcallFn.test_rlm_query_falls_back_to_llm_query: TestRlmQueryWithoutSubcallFn#test_rlm_query_falls_back_to_llm_query().
  TestRlmQueryBatchedWithSubcallFn.test_batched_with_model_override: TestRlmQueryBatchedWithSubcallFn#test_batched_with_model_override().
  TestRlmQueryBatchedWithSubcallFn.test_batched_empty_prompts: TestRlmQueryBatchedWithSubcallFn#test_batched_empty_prompts().
  TestRlmQueryBatchedWithoutSubcallFn.test_batched_falls_back_to_llm_query_batched: TestRlmQueryBatchedWithoutSubcallFn#test_batched_falls_back_to_llm_query_batched().
  TestMaxConcurrentSubcallsBounds.test_batched_empty_prompts_with_parallel: TestMaxConcurrentSubcallsBounds#test_batched_empty_prompts_with_parallel().
  TestMaxConcurrentSubcallsBounds.test_max_concurrent_subcalls_default_value: TestMaxConcurrentSubcallsBounds#test_max_concurrent_subcalls_default_value().
  TestMaxConcurrentSubcallsBounds.test_max_concurrent_subcalls_custom_value: TestMaxConcurrentSubcallsBounds#test_max_concurrent_subcalls_custom_value().
  TestMaxConcurrentSubcallsOnBaseEnv.test_base_env_has_max_concurrent_subcalls: TestMaxConcurrentSubcallsOnBaseEnv#test_base_env_has_max_concurrent_subcalls().
  TestMaxConcurrentSubcallsOnBaseEnv.test_base_env_default_max_concurrent_subcalls: TestMaxConcurrentSubcallsOnBaseEnv#test_base_env_default_max_concurrent_subcalls().
  TestMaxConcurrentSubcallsBounds.tracked_subcall: TestMaxConcurrentSubcallsBounds#tracked_subcall().
  TestRlmQueryBatchedParallel.slow_subcall: TestRlmQueryBatchedParallel#slow_subcall().
  TestRlmQueryBatchedParallel.tracked_subcall: TestRlmQueryBatchedParallel#tracked_subcall().
  TestRlmQueryBatchedParallel.varying_delay_subcall: TestRlmQueryBatchedParallel#varying_delay_subcall().
  TestRlmQueryBatchedParallel.sometimes_fail: TestRlmQueryBatchedParallel#sometimes_fail().
  TestRlmQueryBatchedParallel.delayed_subcall: TestRlmQueryBatchedParallel#delayed_subcall().
  TestMaxConcurrentSubcallsBounds.sequential_subcall: TestMaxConcurrentSubcallsBounds#sequential_subcall().
  TestMaxConcurrentSubcallsBounds.fail_second: TestMaxConcurrentSubcallsBounds#fail_second().
  TestMaxConcurrentSubcallsBounds.always_fail: TestMaxConcurrentSubcallsBounds#always_fail().
  TestRlmQueryWithSubcallFn: TestRlmQueryWithSubcallFn#
  TestRlmQueryWithoutSubcallFn: TestRlmQueryWithoutSubcallFn#
  TestRlmQueryBatchedWithSubcallFn: TestRlmQueryBatchedWithSubcallFn#
  TestRlmQueryBatchedWithoutSubcallFn: TestRlmQueryBatchedWithoutSubcallFn#
  TestLlmQueryDoesNotUseSubcallFn: TestLlmQueryDoesNotUseSubcallFn#
  TestRlmQueryBatchedParallel: TestRlmQueryBatchedParallel#
  TestMaxConcurrentSubcallsBounds: TestMaxConcurrentSubcallsBounds#
  TestMaxConcurrentSubcallsOnBaseEnv: TestMaxConcurrentSubcallsOnBaseEnv#
  TestRlmQueryScaffoldRestoration: TestRlmQueryScaffoldRestoration#
---
# Module: [`tests/test_rlm_query.py`](../../../../../raw/code/rlm/tests/test_rlm_query.py)

## Classes
### `TestLlmQueryDoesNotUseSubcallFn`
- def: [`tests/test_rlm_query.py:168`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L168)
- doc: Verify that llm_query never uses subcall_fn even when one is present.
- signature: `class TestLlmQueryDoesNotUseSubcallFn:`
- members:
  - `test_llm_query_batched_ignores_subcall_fn(self)` — [`L181`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L181) — llm_query_batched should never use subcall_fn.
  - `test_llm_query_ignores_subcall_fn(self)` — [`L171`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L171) — llm_query should always do a plain LM call, never use subcall_fn.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)  (1 test-only)

### `TestMaxConcurrentSubcallsBounds`
- def: [`tests/test_rlm_query.py:309`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L309)
- doc: Tests for edge cases and boundary conditions of max_concurrent_subcalls.
- signature: `class TestMaxConcurrentSubcallsBounds:`
- members:
  - `always_fail(prompt, model)` — [`L385`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L385)
  - `fail_second(prompt, model)` — [`L437`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L437)
  - `sequential_subcall(prompt, model)` — [`L329`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L329)
  - `test_batched_all_failures_parallel(self)` — [`L382`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L382) — All subcalls failing in parallel should return all error strings.
  - `test_batched_empty_prompts_with_parallel(self)` — [`L425`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L425) — Empty prompt list should return empty list regardless of concurrency setting.
  - `test_batched_large_batch_with_low_concurrency(self)` — [`L398`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L398) — Many prompts with low concurrency should still complete correctly.
  - `test_max_concurrent_subcalls_custom_value(self)` — [`L318`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L318) — Should accept custom max_concurrent_subcalls values.
  - `test_max_concurrent_subcalls_default_value(self)` — [`L312`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L312) — Default max_concurrent_subcalls should be 4.
  - `test_max_concurrent_subcalls_exact_match(self)` — [`L360`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L360) — max_concurrent_subcalls == prompt count should allow full parallelism.
  - `test_max_concurrent_subcalls_larger_than_prompts(self)` — [`L350`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L350) — max_concurrent_subcalls larger than prompt count should work fine.
  - `test_max_concurrent_subcalls_one(self)` — [`L324`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L324) — max_concurrent_subcalls=1 should force sequential execution.
  - `test_pending_calls_exclude_failures(self)` — [`L434`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L434) — Failed subcalls should not appear in pending_llm_calls.
  - `tracked_subcall(prompt, model)` — [`L366`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L366)
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls), [`max_concurrent_subcalls`](../rlm/environments/base_env.md#BaseEnv.max_concurrent_subcalls)  (1 test-only)

### `TestMaxConcurrentSubcallsOnBaseEnv`
- def: [`tests/test_rlm_query.py:452`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L452)
- doc: Tests that max_concurrent_subcalls is a property of BaseEnv, not just LocalREPL.
- signature: `class TestMaxConcurrentSubcallsOnBaseEnv:`
- members:
  - `test_base_env_default_max_concurrent_subcalls(self)` — [`L465`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L465) — BaseEnv default should be 4.
  - `test_base_env_has_max_concurrent_subcalls(self)` — [`L455`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L455) — BaseEnv should accept and store max_concurrent_subcalls.
- uses (calls/refs, reference-scoped): [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`max_concurrent_subcalls`](../rlm/environments/base_env.md#BaseEnv.max_concurrent_subcalls)

### `TestRlmQueryBatchedParallel`
- def: [`tests/test_rlm_query.py:191`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L191)
- doc: Tests for parallel execution of rlm_query_batched.
- signature: `class TestRlmQueryBatchedParallel:`
- members:
  - `delayed_subcall(prompt, model)` — [`L285`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L285)
  - `slow_subcall(prompt, model)` — [`L199`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L199)
  - `sometimes_fail(prompt, model)` — [`L264`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L264)
  - `test_batched_parallel_partial_failure(self)` — [`L259`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L259) — Failures in some threads should not affect others.
  - `test_batched_pending_calls_ordered(self)` — [`L282`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L282) — Pending LLM calls should be appended in prompt order for deterministic metadata.
  - `test_batched_preserves_order_parallel(self)` — [`L244`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L244) — Results must be in the same order as input prompts even with parallel execution.
  - `test_batched_respects_max_concurrent(self)` — [`L222`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L222) — Thread pool should not exceed max_concurrent_subcalls.
  - `test_batched_runs_in_parallel(self)` — [`L194`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L194) — Multiple subcalls should execute concurrently, not sequentially.
  - `test_single_prompt_skips_thread_pool(self)` — [`L299`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L299) — Single prompt should not use ThreadPoolExecutor (no overhead).
  - `tracked_subcall(prompt, model)` — [`L229`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L229)
  - `varying_delay_subcall(prompt, model)` — [`L248`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L248)
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls)  (1 test-only)

### `TestRlmQueryBatchedWithSubcallFn`
- def: [`tests/test_rlm_query.py:76`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L76)
- doc: Tests for rlm_query_batched when subcall_fn is provided.
- signature: `class TestRlmQueryBatchedWithSubcallFn:`
- members:
  - `test_batched_calls_subcall_fn_per_prompt(self)` — [`L79`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L79) — rlm_query_batched should call subcall_fn once per prompt.
  - `test_batched_empty_prompts(self)` — [`L136`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L136) — rlm_query_batched with empty list should return empty list.
  - `test_batched_partial_failure(self)` — [`L117`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L117) — If one subcall_fn call fails, others should still succeed.
  - `test_batched_single_prompt(self)` — [`L145`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L145) — rlm_query_batched with single prompt should work.
  - `test_batched_tracks_all_pending_calls(self)` — [`L97`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L97) — rlm_query_batched should track all completions in rlm_calls.
  - `test_batched_with_model_override(self)` — [`L107`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L107) — rlm_query_batched should pass model to each subcall_fn call.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls)  (1 test-only)

### `TestRlmQueryBatchedWithoutSubcallFn`
- def: [`tests/test_rlm_query.py:155`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L155)
- doc: Tests for rlm_query_batched when no subcall_fn.
- signature: `class TestRlmQueryBatchedWithoutSubcallFn:`
- members:
  - `test_batched_falls_back_to_llm_query_batched(self)` — [`L158`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L158) — Without subcall_fn, should fall back to llm_query_batched (error without handler).
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestRlmQueryScaffoldRestoration`
- def: [`tests/test_rlm_query.py:472`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L472)
- doc: Test that rlm_query and rlm_query_batched are restored after overwrite.
- signature: `class TestRlmQueryScaffoldRestoration:`
- members:
  - `test_rlm_query_batched_restored_after_overwrite(self)` — [`L486`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L486) — If model overwrites rlm_query_batched, the next execution should have the real one.
  - `test_rlm_query_restored_after_overwrite(self)` — [`L475`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L475) — If model overwrites rlm_query, the next execution should have the real one.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)  (1 test-only)

### `TestRlmQueryWithSubcallFn`
- def: [`tests/test_rlm_query.py:22`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L22)
- doc: Tests for rlm_query when subcall_fn is provided (depth &gt; 1).
- signature: `class TestRlmQueryWithSubcallFn:`
- members:
  - `test_rlm_query_error_handling(self)` — [`L54`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L54) — rlm_query should return error string if subcall_fn raises.
  - `test_rlm_query_tracks_pending_calls(self)` — [`L44`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L44) — rlm_query should append completion to _pending_llm_calls.
  - `test_rlm_query_uses_subcall_fn(self)` — [`L25`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L25) — rlm_query should use subcall_fn when available.
  - `test_rlm_query_with_model_override(self)` — [`L35`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L35) — rlm_query should pass model to subcall_fn.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`rlm_calls`](../rlm/core/types.md#REPLResult.rlm_calls)  (1 test-only)

### `TestRlmQueryWithoutSubcallFn`
- def: [`tests/test_rlm_query.py:65`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L65)
- doc: Tests for rlm_query when no subcall_fn (depth == 1 or max_depth reached).
- signature: `class TestRlmQueryWithoutSubcallFn:`
- members:
  - `test_rlm_query_falls_back_to_llm_query(self)` — [`L68`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L68) — Without subcall_fn, rlm_query should fall back to llm_query (which returns error without handler).
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`locals`](../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup)

## Functions
- `_make_completion(response: str)` — [`L11`](../../../../../raw/code/rlm/tests/test_rlm_query.py#L11) — Create a minimal RLMChatCompletion for testing.

