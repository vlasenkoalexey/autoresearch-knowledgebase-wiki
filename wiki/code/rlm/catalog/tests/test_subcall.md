---
title: 'Module: tests/test_subcall.py'
type: catalog
provenance: extracted
module: tests/test_subcall.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_subcall`/
symbols:
  create_mock_lm: create_mock_lm().
  TestSubcallTimeoutPropagation.test_child_receives_remaining_timeout: TestSubcallTimeoutPropagation#test_child_receives_remaining_timeout().
  TestSubcallTimeoutPropagation.test_subcall_returns_error_when_timeout_exhausted: TestSubcallTimeoutPropagation#test_subcall_returns_error_when_timeout_exhausted().
  TestSubcallModelOverride.test_model_override_does_not_mutate_parent_kwargs: TestSubcallModelOverride#test_model_override_does_not_mutate_parent_kwargs().
  TestSubcallCombinedParameters.test_all_parameters_propagate_together: TestSubcallCombinedParameters#test_all_parameters_propagate_together().
  TestSubcallTimeoutPropagation.test_child_receives_none_timeout_when_parent_has_none: TestSubcallTimeoutPropagation#test_child_receives_none_timeout_when_parent_has_none().
  TestSubcallTokensPropagation.test_child_receives_max_tokens: TestSubcallTokensPropagation#test_child_receives_max_tokens().
  TestSubcallTokensPropagation.test_child_receives_none_tokens_when_parent_has_none: TestSubcallTokensPropagation#test_child_receives_none_tokens_when_parent_has_none().
  TestSubcallErrorsPropagation.test_child_receives_max_errors: TestSubcallErrorsPropagation#test_child_receives_max_errors().
  TestSubcallErrorsPropagation.test_child_receives_none_errors_when_parent_has_none: TestSubcallErrorsPropagation#test_child_receives_none_errors_when_parent_has_none().
  TestSubcallModelOverride.test_model_override_sets_child_backend_kwargs: TestSubcallModelOverride#test_model_override_sets_child_backend_kwargs().
  TestSubcallModelOverride.test_no_model_override_uses_parent_kwargs: TestSubcallModelOverride#test_no_model_override_uses_parent_kwargs().
  TestSubcallModelOverrideAtLeafDepth.test_model_override_at_leaf_depth_uses_overridden_model: TestSubcallModelOverrideAtLeafDepth#test_model_override_at_leaf_depth_uses_overridden_model().
  TestSubcallModelOverrideAtLeafDepth.test_leaf_depth_without_model_override_uses_parent_model: TestSubcallModelOverrideAtLeafDepth#test_leaf_depth_without_model_override_uses_parent_model().
  final: final().
  TestSubcallTimeoutPropagation.test_child_receives_remaining_timeout.CapturingRLM.__init__: TestSubcallTimeoutPropagation#test_child_receives_remaining_timeout().CapturingRLM#__init__().
  TestSubcallTimeoutPropagation.test_child_receives_none_timeout_when_parent_has_none.CapturingRLM.__init__: TestSubcallTimeoutPropagation#test_child_receives_none_timeout_when_parent_has_none().CapturingRLM#__init__().
  TestSubcallTokensPropagation.test_child_receives_max_tokens.CapturingRLM.__init__: TestSubcallTokensPropagation#test_child_receives_max_tokens().CapturingRLM#__init__().
  TestSubcallTokensPropagation.test_child_receives_none_tokens_when_parent_has_none.CapturingRLM.__init__: TestSubcallTokensPropagation#test_child_receives_none_tokens_when_parent_has_none().CapturingRLM#__init__().
  TestSubcallErrorsPropagation.test_child_receives_max_errors.CapturingRLM.__init__: TestSubcallErrorsPropagation#test_child_receives_max_errors().CapturingRLM#__init__().
  TestSubcallErrorsPropagation.test_child_receives_none_errors_when_parent_has_none.CapturingRLM.__init__: TestSubcallErrorsPropagation#test_child_receives_none_errors_when_parent_has_none().CapturingRLM#__init__().
  TestSubcallModelOverride.test_model_override_sets_child_backend_kwargs.CapturingRLM.__init__: TestSubcallModelOverride#test_model_override_sets_child_backend_kwargs().CapturingRLM#__init__().
  TestSubcallModelOverride.test_model_override_does_not_mutate_parent_kwargs.CapturingRLM.__init__: TestSubcallModelOverride#test_model_override_does_not_mutate_parent_kwargs().CapturingRLM#__init__().
  TestSubcallModelOverride.test_no_model_override_uses_parent_kwargs.CapturingRLM.__init__: TestSubcallModelOverride#test_no_model_override_uses_parent_kwargs().CapturingRLM#__init__().
  TestSubcallCombinedParameters.test_all_parameters_propagate_together.CapturingRLM.__init__: TestSubcallCombinedParameters#test_all_parameters_propagate_together().CapturingRLM#__init__().
  TestSubcallTimeoutPropagation.test_child_receives_remaining_timeout.CapturingRLM: TestSubcallTimeoutPropagation#test_child_receives_remaining_timeout().CapturingRLM#
  TestSubcallTimeoutPropagation.test_child_receives_none_timeout_when_parent_has_none.CapturingRLM: TestSubcallTimeoutPropagation#test_child_receives_none_timeout_when_parent_has_none().CapturingRLM#
  TestSubcallTokensPropagation.test_child_receives_max_tokens.CapturingRLM: TestSubcallTokensPropagation#test_child_receives_max_tokens().CapturingRLM#
  TestSubcallTokensPropagation.test_child_receives_none_tokens_when_parent_has_none.CapturingRLM: TestSubcallTokensPropagation#test_child_receives_none_tokens_when_parent_has_none().CapturingRLM#
  TestSubcallErrorsPropagation.test_child_receives_max_errors.CapturingRLM: TestSubcallErrorsPropagation#test_child_receives_max_errors().CapturingRLM#
  TestSubcallErrorsPropagation.test_child_receives_none_errors_when_parent_has_none.CapturingRLM: TestSubcallErrorsPropagation#test_child_receives_none_errors_when_parent_has_none().CapturingRLM#
  TestSubcallModelOverride.test_model_override_sets_child_backend_kwargs.CapturingRLM: TestSubcallModelOverride#test_model_override_sets_child_backend_kwargs().CapturingRLM#
  TestSubcallModelOverride.test_model_override_does_not_mutate_parent_kwargs.CapturingRLM: TestSubcallModelOverride#test_model_override_does_not_mutate_parent_kwargs().CapturingRLM#
  TestSubcallModelOverride.test_no_model_override_uses_parent_kwargs.CapturingRLM: TestSubcallModelOverride#test_no_model_override_uses_parent_kwargs().CapturingRLM#
  TestSubcallCombinedParameters.test_all_parameters_propagate_together.CapturingRLM: TestSubcallCombinedParameters#test_all_parameters_propagate_together().CapturingRLM#
  TestSubcallTimeoutPropagation: TestSubcallTimeoutPropagation#
  TestSubcallTokensPropagation: TestSubcallTokensPropagation#
  TestSubcallErrorsPropagation: TestSubcallErrorsPropagation#
  TestSubcallModelOverride: TestSubcallModelOverride#
  TestSubcallModelOverrideAtLeafDepth: TestSubcallModelOverrideAtLeafDepth#
  TestSubcallCombinedParameters: TestSubcallCombinedParameters#
---
# Module: [`tests/test_subcall.py`](../../../../../raw/code/rlm/tests/test_subcall.py)

## Classes
### `CapturingRLM`  ·  implements/extends RLM
- def: [`tests/test_subcall.py:440`](../../../../../raw/code/rlm/tests/test_subcall.py#L440)
- signature: `class CapturingRLM(original_rlm_class):`
- protocol/private: `__init__`[`L50`](../../../../../raw/code/rlm/tests/test_subcall.py#L50), `__init__`[`L90`](../../../../../raw/code/rlm/tests/test_subcall.py#L90), `__init__`[`L145`](../../../../../raw/code/rlm/tests/test_subcall.py#L145), `__init__`[`L174`](../../../../../raw/code/rlm/tests/test_subcall.py#L174), `__init__`[`L207`](../../../../../raw/code/rlm/tests/test_subcall.py#L207), `__init__`[`L236`](../../../../../raw/code/rlm/tests/test_subcall.py#L236), `__init__`[`L269`](../../../../../raw/code/rlm/tests/test_subcall.py#L269), `__init__`[`L302`](../../../../../raw/code/rlm/tests/test_subcall.py#L302), `__init__`[`L333`](../../../../../raw/code/rlm/tests/test_subcall.py#L333), `__init__`[`L441`](../../../../../raw/code/rlm/tests/test_subcall.py#L441)
- uses (calls/refs, reference-scoped): [`__init__`](../rlm/core/rlm.md#RLM.__init__)
- used by: [`RLM`](../rlm/core/rlm.md#RLM)  (1 test-only)

### `TestSubcallCombinedParameters`
- def: [`tests/test_subcall.py:431`](../../../../../raw/code/rlm/tests/test_subcall.py#L431)
- doc: Tests for combined parameter propagation.
- signature: `class TestSubcallCombinedParameters:`
- members:
  - `test_all_parameters_propagate_together(self)` — [`L434`](../../../../../raw/code/rlm/tests/test_subcall.py#L434) — All parameters (timeout, tokens, errors, model) should propagate correctly together.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`close`](../rlm/core/rlm.md#RLM.close), [`_completion_start_time`](../rlm/core/rlm.md#RLM._completion_start_time)  (3 test-only)

### `TestSubcallErrorsPropagation`
- def: [`tests/test_subcall.py:197`](../../../../../raw/code/rlm/tests/test_subcall.py#L197)
- doc: Tests for max_errors propagation to child RLM.
- signature: `class TestSubcallErrorsPropagation:`
- members:
  - `test_child_receives_max_errors(self)` — [`L200`](../../../../../raw/code/rlm/tests/test_subcall.py#L200) — Child RLM should get same max_errors as parent.
  - `test_child_receives_none_errors_when_parent_has_none(self)` — [`L229`](../../../../../raw/code/rlm/tests/test_subcall.py#L229) — When parent has no max_errors, child should also have None.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`close`](../rlm/core/rlm.md#RLM.close)  (4 test-only)

### `TestSubcallModelOverride`
- def: [`tests/test_subcall.py:259`](../../../../../raw/code/rlm/tests/test_subcall.py#L259)
- doc: Tests for model= parameter override in _subcall.
- signature: `class TestSubcallModelOverride:`
- members:
  - `test_model_override_does_not_mutate_parent_kwargs(self)` — [`L295`](../../../../../raw/code/rlm/tests/test_subcall.py#L295) — Model override should not mutate parent's backend_kwargs.
  - `test_model_override_sets_child_backend_kwargs(self)` — [`L262`](../../../../../raw/code/rlm/tests/test_subcall.py#L262) — When llm_query(prompt, model='test-model') is called, child's backend_kwargs should have model_name='test-model'.
  - `test_no_model_override_uses_parent_kwargs(self)` — [`L326`](../../../../../raw/code/rlm/tests/test_subcall.py#L326) — When no model override is provided, child uses parent's backend_kwargs.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`close`](../rlm/core/rlm.md#RLM.close), [`backend_kwargs`](../rlm/core/rlm.md#RLM.backend_kwargs)  (5 test-only)

### `TestSubcallModelOverrideAtLeafDepth`
- def: [`tests/test_subcall.py:358`](../../../../../raw/code/rlm/tests/test_subcall.py#L358)
- doc: Tests for model override at max_depth (leaf LM completion).
- signature: `class TestSubcallModelOverrideAtLeafDepth:`
- members:
  - `test_leaf_depth_without_model_override_uses_parent_model(self)` — [`L401`](../../../../../raw/code/rlm/tests/test_subcall.py#L401) — When at max_depth without model override, uses parent's model.
  - `test_model_override_at_leaf_depth_uses_overridden_model(self)` — [`L361`](../../../../../raw/code/rlm/tests/test_subcall.py#L361) — When at max_depth, the leaf LM completion should use the overridden model.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`close`](../rlm/core/rlm.md#RLM.close)  (2 test-only)

### `TestSubcallTimeoutPropagation`
- def: [`tests/test_subcall.py:39`](../../../../../raw/code/rlm/tests/test_subcall.py#L39)
- doc: Tests for max_timeout propagation to child RLM.
- signature: `class TestSubcallTimeoutPropagation:`
- members:
  - `test_child_receives_none_timeout_when_parent_has_none(self)` — [`L83`](../../../../../raw/code/rlm/tests/test_subcall.py#L83) — When parent has no max_timeout, child should also have None.
  - `test_child_receives_remaining_timeout(self)` — [`L42`](../../../../../raw/code/rlm/tests/test_subcall.py#L42) — When parent has max_timeout=60 and 10s have elapsed, child should get max_timeout approx 50.
  - `test_subcall_returns_error_when_timeout_exhausted(self)` — [`L112`](../../../../../raw/code/rlm/tests/test_subcall.py#L112) — When timeout is already exhausted, _subcall should return error message.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`close`](../rlm/core/rlm.md#RLM.close), [`_completion_start_time`](../rlm/core/rlm.md#RLM._completion_start_time)  (4 test-only)

### `TestSubcallTokensPropagation`
- def: [`tests/test_subcall.py:135`](../../../../../raw/code/rlm/tests/test_subcall.py#L135)
- doc: Tests for max_tokens propagation to child RLM.
- signature: `class TestSubcallTokensPropagation:`
- members:
  - `test_child_receives_max_tokens(self)` — [`L138`](../../../../../raw/code/rlm/tests/test_subcall.py#L138) — Child RLM should get same max_tokens as parent.
  - `test_child_receives_none_tokens_when_parent_has_none(self)` — [`L167`](../../../../../raw/code/rlm/tests/test_subcall.py#L167) — When parent has no max_tokens, child should also have None.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`_subcall`](../rlm/core/rlm.md#RLM._subcall), [`close`](../rlm/core/rlm.md#RLM.close)  (4 test-only)

## Functions
- `create_mock_lm(responses: list[str], model_name: str = "mock-model")` — [`L18`](../../../../../raw/code/rlm/tests/test_subcall.py#L18) — Create a mock LM that returns responses in order.
- `final(content: str)` — [`L34`](../../../../../raw/code/rlm/tests/test_subcall.py#L34) — Render a model response that submits ``content`` as the final answer.

