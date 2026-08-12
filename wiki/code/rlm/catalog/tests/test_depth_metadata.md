---
title: 'Module: tests/test_depth_metadata.py'
type: catalog
provenance: extracted
module: tests/test_depth_metadata.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_depth_metadata`/
symbols:
  TestDepth1LimitChecks.test_error_threshold_check: TestDepth1LimitChecks#test_error_threshold_check().
  TestDepth1LimitChecks.test_error_count_resets_on_success: TestDepth1LimitChecks#test_error_count_resets_on_success().
  TestDepth1LimitChecks.test_budget_check_raises: TestDepth1LimitChecks#test_budget_check_raises().
  TestDepth1LimitChecks.test_token_limit_check_raises: TestDepth1LimitChecks#test_token_limit_check_raises().
  create_mock_lm: create_mock_lm().
  TestSubcallLoggerPropagation.test_child_gets_logger_when_parent_has_logger: TestSubcallLoggerPropagation#test_child_gets_logger_when_parent_has_logger().
  TestSubcallLoggerPropagation.test_leaf_subcall_returns_no_metadata: TestSubcallLoggerPropagation#test_leaf_subcall_returns_no_metadata().
  TestSubcallLoggerPropagation.test_subcall_metadata_has_trajectory: TestSubcallLoggerPropagation#test_subcall_metadata_has_trajectory().
  TestDepth1CompletionLoop.test_basic_completion_with_final_answer: TestDepth1CompletionLoop#test_basic_completion_with_final_answer().
  TestDepth1LoggerMetadata.test_completion_returns_metadata_with_logger: TestDepth1LoggerMetadata#test_completion_returns_metadata_with_logger().
  TestDepth1LoggerMetadata.test_metadata_has_multiple_iterations: TestDepth1LoggerMetadata#test_metadata_has_multiple_iterations().
  TestSubcallLoggerPropagation.test_child_gets_no_logger_when_parent_has_none: TestSubcallLoggerPropagation#test_child_gets_no_logger_when_parent_has_none().
  TestSubcallCustomToolsPropagation.test_sub_tools_propagated_to_child: TestSubcallCustomToolsPropagation#test_sub_tools_propagated_to_child().
  TestSubcallCustomToolsPropagation.test_empty_sub_tools_propagated: TestSubcallCustomToolsPropagation#test_empty_sub_tools_propagated().
  TestDepth1CompletionLoop.test_multi_iteration_before_final: TestDepth1CompletionLoop#test_multi_iteration_before_final().
  TestDepth1LimitChecks.test_timeout_check_raises: TestDepth1LimitChecks#test_timeout_check_raises().
  TestDepth1LoggerMetadata.test_completion_returns_no_metadata_without_logger: TestDepth1LoggerMetadata#test_completion_returns_no_metadata_without_logger().
  final: final().
  TestDepth1CompletionLoop.test_no_subcall_fn_at_depth_1: TestDepth1CompletionLoop#test_no_subcall_fn_at_depth_1().
  TestDepth1CompletionLoop.test_subcall_fn_passed_at_depth_gt_1: TestDepth1CompletionLoop#test_subcall_fn_passed_at_depth_gt_1().
  TestDepth1LimitChecks.test_timeout_check_no_raise_within_limit: TestDepth1LimitChecks#test_timeout_check_no_raise_within_limit().
  TestDepth1LimitChecks.test_timeout_check_noop_when_none: TestDepth1LimitChecks#test_timeout_check_noop_when_none().
  TestSubcallLoggerPropagation.test_child_gets_logger_when_parent_has_logger.CapturingRLM.__init__: TestSubcallLoggerPropagation#test_child_gets_logger_when_parent_has_logger().CapturingRLM#__init__().
  TestSubcallLoggerPropagation.test_child_gets_no_logger_when_parent_has_none.CapturingRLM.__init__: TestSubcallLoggerPropagation#test_child_gets_no_logger_when_parent_has_none().CapturingRLM#__init__().
  TestSubcallCustomToolsPropagation.test_sub_tools_propagated_to_child.CapturingRLM.__init__: TestSubcallCustomToolsPropagation#test_sub_tools_propagated_to_child().CapturingRLM#__init__().
  TestSubcallCustomToolsPropagation.test_empty_sub_tools_propagated.CapturingRLM.__init__: TestSubcallCustomToolsPropagation#test_empty_sub_tools_propagated().CapturingRLM#__init__().
  TestSubcallLoggerPropagation.test_child_gets_logger_when_parent_has_logger.CapturingRLM: TestSubcallLoggerPropagation#test_child_gets_logger_when_parent_has_logger().CapturingRLM#
  TestSubcallLoggerPropagation.test_child_gets_no_logger_when_parent_has_none.CapturingRLM: TestSubcallLoggerPropagation#test_child_gets_no_logger_when_parent_has_none().CapturingRLM#
  TestSubcallCustomToolsPropagation.test_sub_tools_propagated_to_child.CapturingRLM: TestSubcallCustomToolsPropagation#test_sub_tools_propagated_to_child().CapturingRLM#
  TestSubcallCustomToolsPropagation.test_empty_sub_tools_propagated.CapturingRLM: TestSubcallCustomToolsPropagation#test_empty_sub_tools_propagated().CapturingRLM#
  TestDepth1CompletionLoop: TestDepth1CompletionLoop#
  TestDepth1LimitChecks: TestDepth1LimitChecks#
  TestDepth1LoggerMetadata: TestDepth1LoggerMetadata#
  TestSubcallLoggerPropagation: TestSubcallLoggerPropagation#
  TestSubcallCustomToolsPropagation: TestSubcallCustomToolsPropagation#
---
# Module: [`tests/test_depth_metadata.py`](../../../../../raw/code/rlm/tests/test_depth_metadata.py)

## Classes
### `CapturingRLM`  ·  implements/extends RLM
- def: [`tests/test_depth_metadata.py:540`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L540)
- signature: `class CapturingRLM(original_rlm_class):`
- protocol/private: `__init__`[`L394`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L394), `__init__`[`L429`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L429), `__init__`[`L509`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L509), `__init__`[`L541`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L541)
- uses (calls/refs, reference-scoped): [`__init__`](../rlm/core/rlm.md#RLM.__init__)
- used by: [`RLM`](../rlm/core/rlm.md#RLM)  (1 test-only)

### `TestDepth1CompletionLoop`
- def: [`tests/test_depth_metadata.py:49`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L49)
- doc: Verify depth=1 completion loop works identically to before refactoring.
- signature: `class TestDepth1CompletionLoop:`
- members:
  - `test_basic_completion_with_final_answer(self)` — [`L52`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L52) — depth=1 RLM should complete normally when the model sets answer['ready'] = True.
  - `test_multi_iteration_before_final(self)` — [`L67`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L67) — depth=1 should iterate multiple times before the model signals ready.
  - `test_no_subcall_fn_at_depth_1(self)` — [`L87`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L87) — depth=1 (max_depth=1) should NOT pass subcall_fn to environment.
  - `test_subcall_fn_passed_at_depth_gt_1(self)` — [`L114`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L114) — max_depth>1 SHOULD pass subcall_fn to environment.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`root_model`](../rlm/core/types.md#RLMChatCompletion.root_model)  (2 test-only)

### `TestDepth1LimitChecks`
- def: [`tests/test_depth_metadata.py:141`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L141)
- doc: Verify limit checks work correctly in the refactored helpers.
- signature: `class TestDepth1LimitChecks:`
- members:
  - `test_budget_check_raises(self)` — [`L258`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L258) — _check_iteration_limits should raise BudgetExceededError when budget exceeded.
  - `test_error_count_resets_on_success(self)` — [`L220`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L220) — Consecutive error count should reset on a successful iteration.
  - `test_error_threshold_check(self)` — [`L186`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L186) — _check_iteration_limits should raise on consecutive errors.
  - `test_timeout_check_no_raise_within_limit(self)` — [`L161`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L161) — _check_timeout should not raise when within limit.
  - `test_timeout_check_noop_when_none(self)` — [`L174`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L174) — _check_timeout should be a no-op when max_timeout is None.
  - `test_timeout_check_raises(self)` — [`L144`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L144) — _check_timeout should raise TimeoutExceededError when exceeded.
  - `test_token_limit_check_raises(self)` — [`L287`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L287) — _check_iteration_limits should raise TokenLimitExceededError when tokens exceeded.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`_check_iteration_limits`](../rlm/core/rlm.md#RLM._check_iteration_limits), [`REPLResult`](../rlm/core/types.md#REPLResult), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`RLMIteration`](../rlm/core/types.md#RLMIteration), [`code_blocks`](../rlm/core/types.md#RLMIteration.code_blocks), [`result`](../rlm/core/types.md#CodeBlock.result), [`response`](../rlm/core/types.md#RLMIteration.response), [`CodeBlock`](../rlm/core/types.md#CodeBlock), [`_check_timeout`](../rlm/core/rlm.md#RLM._check_timeout), [`prompt`](../rlm/core/types.md#RLMIteration.prompt), [`_consecutive_errors`](../rlm/core/rlm.md#RLM._consecutive_errors), [`code`](../rlm/core/types.md#CodeBlock.code), [`total_cost`](../rlm/core/types.md#ModelUsageSummary.total_cost), [`BudgetExceededError`](../rlm/utils/exceptions.md#BudgetExceededError), [`ErrorThresholdExceededError`](../rlm/utils/exceptions.md#ErrorThresholdExceededError), [`TimeoutExceededError`](../rlm/utils/exceptions.md#TimeoutExceededError), [`TokenLimitExceededError`](../rlm/utils/exceptions.md#TokenLimitExceededError), [`spent`](../rlm/utils/exceptions.md#BudgetExceededError.spent), [`budget`](../rlm/utils/exceptions.md#BudgetExceededError.budget), [`elapsed`](../rlm/utils/exceptions.md#TimeoutExceededError.elapsed), [`error_count`](../rlm/utils/exceptions.md#ErrorThresholdExceededError.error_count), [`threshold`](../rlm/utils/exceptions.md#ErrorThresholdExceededError.threshold), [`timeout`](../rlm/utils/exceptions.md#TimeoutExceededError.timeout), [`token_limit`](../rlm/utils/exceptions.md#TokenLimitExceededError.token_limit), [`tokens_used`](../rlm/utils/exceptions.md#TokenLimitExceededError.tokens_used)

### `TestDepth1LoggerMetadata`
- def: [`tests/test_depth_metadata.py:316`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L316)
- doc: Verify depth=1 logger metadata is captured correctly.
- signature: `class TestDepth1LoggerMetadata:`
- members:
  - `test_completion_returns_metadata_with_logger(self)` — [`L319`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L319) — When logger is provided, completion result should have metadata.
  - `test_completion_returns_no_metadata_without_logger(self)` — [`L340`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L340) — When no logger is provided, metadata should be None.
  - `test_metadata_has_multiple_iterations(self)` — [`L354`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L354) — Logger should capture all iterations.
- uses (calls/refs, reference-scoped): [`completion`](../rlm/core/rlm.md#RLM.completion), [`RLM`](../rlm/core/rlm.md#RLM), [`metadata`](../rlm/core/types.md#RLMChatCompletion.metadata), [`RLMLogger`](../rlm/logger/rlm_logger.md#RLMLogger)  (2 test-only)

### `TestSubcallCustomToolsPropagation`
- def: [`tests/test_depth_metadata.py:499`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L499)
- doc: Verify custom_tools propagation to child RLM in _subcall.
- signature: `class TestSubcallCustomToolsPropagation:`
- members:
  - `test_empty_sub_tools_propagated(self)` — [`L534`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L534) — When custom_sub_tools is empty dict, child should get empty dict (no tools).
  - `test_sub_tools_propagated_to_child(self)` — [`L502`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L502) — Child should receive parent's custom_sub_tools as its custom_tools.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`close`](../rlm/core/rlm.md#RLM.close)  (4 test-only)

### `TestSubcallLoggerPropagation`
- def: [`tests/test_depth_metadata.py:384`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L384)
- doc: Verify child RLM gets a logger when parent has one, and metadata flows back.
- signature: `class TestSubcallLoggerPropagation:`
- members:
  - `test_child_gets_logger_when_parent_has_logger(self)` — [`L387`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L387) — When parent has a logger, child RLM should also get a logger. — documented in [rlm-core-rlm](../../concepts/rlm-core-rlm.md)
  - `test_child_gets_no_logger_when_parent_has_none(self)` — [`L422`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L422) — When parent has no logger, child should also get None.
  - `test_leaf_subcall_returns_no_metadata(self)` — [`L451`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L451) — At max_depth (leaf), subcall returns plain LM completion with no metadata. — documented in [rlm-core-rlm](../../concepts/rlm-core-rlm.md)
  - `test_subcall_metadata_has_trajectory(self)` — [`L473`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L473) — When child RLM completes with a logger, the returned RLMChatCompletion should have metadata.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`metadata`](../rlm/core/types.md#RLMChatCompletion.metadata), [`RLMLogger`](../rlm/logger/rlm_logger.md#RLMLogger), [`close`](../rlm/core/rlm.md#RLM.close)  (4 test-only)

## Functions
- `create_mock_lm(responses: list[str], model_name: str = "mock-model")` — [`L23`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L23) — Create a mock LM that returns responses in order.
- `final(content: str)` — [`L39`](../../../../../raw/code/rlm/tests/test_depth_metadata.py#L39) — Render a model response that submits ``content`` as the final answer.

