---
title: 'Module: tests/test_lm_handler.py'
type: catalog
provenance: extracted
module: tests/test_lm_handler.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_lm_handler`/test_lm_handler_
symbols:
  test_lm_handler_single_request: single_request().
  test_lm_handler_batched_partial_failure: batched_partial_failure().
  test_lm_handler_batched_request: batched_request().
  test_lm_handler_batched_many_prompts_semaphore_cap: batched_many_prompts_semaphore_cap().
  test_lm_handler_batched_partial_failure.response_fn: batched_partial_failure().response_fn().
---
# Module: [`tests/test_lm_handler.py`](../../../../../raw/code/rlm/tests/test_lm_handler.py)

## Functions
- `response_fn(prompt)` — [`L36`](../../../../../raw/code/rlm/tests/test_lm_handler.py#L36)
- `test_lm_handler_batched_many_prompts_semaphore_cap()` — [`L55`](../../../../../raw/code/rlm/tests/test_lm_handler.py#L55) — Many prompts complete successfully with semaphore limiting concurrency. — documented in [rlm-core-lm_handler](../../concepts/rlm-core-lm_handler.md)
- `test_lm_handler_batched_partial_failure()` — [`L33`](../../../../../raw/code/rlm/tests/test_lm_handler.py#L33) — One failing call returns an error for that slot; the rest still succeed. — documented in [rlm-core-lm_handler](../../concepts/rlm-core-lm_handler.md)
- `test_lm_handler_batched_request()` — [`L19`](../../../../../raw/code/rlm/tests/test_lm_handler.py#L19) — Batched prompts return one response per prompt in order.
- `test_lm_handler_single_request()` — [`L8`](../../../../../raw/code/rlm/tests/test_lm_handler.py#L8) — Single prompt request returns success and echo-style content.

