---
title: 'Module: tests/mock_lm.py'
type: catalog
provenance: extracted
module: tests/mock_lm.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.mock_lm`/MockLM#
symbols:
  MockLM.get_usage_summary: get_usage_summary().
  MockLM.get_last_usage: get_last_usage().
  MockLM.completion: completion().
  MockLM: ''
  MockLM._call_count: _call_count.
  MockLM._responses: _responses.
  MockLM.__init__: __init__().
  MockLM.acompletion: acompletion().
  MockLM._response_fn: _response_fn.
---
# Module: [`tests/mock_lm.py`](../../../../../raw/code/rlm/tests/mock_lm.py)

## Classes
### `MockLM`  ·  implements/extends BaseLM
- def: [`tests/mock_lm.py:10`](../../../../../raw/code/rlm/tests/mock_lm.py#L10)
- doc: In-memory mock LM that implements BaseLM for testing.
- signature: `class MockLM(BaseLM):`
- members:
  - `acompletion(self, prompt: str | dict[str, Any])` — [`L42`](../../../../../raw/code/rlm/tests/mock_lm.py#L42)
  - `completion(self, prompt: str | dict[str, Any])` — [`L31`](../../../../../raw/code/rlm/tests/mock_lm.py#L31)
  - `get_last_usage(self)` — [`L56`](../../../../../raw/code/rlm/tests/mock_lm.py#L56)
  - `get_usage_summary(self)` — [`L45`](../../../../../raw/code/rlm/tests/mock_lm.py#L45)
- protocol/private: `__init__`[`L19`](../../../../../raw/code/rlm/tests/mock_lm.py#L19), `_call_count`[`L29`](../../../../../raw/code/rlm/tests/mock_lm.py#L29), `_response_fn`[`L28`](../../../../../raw/code/rlm/tests/mock_lm.py#L28), `_responses`[`L27`](../../../../../raw/code/rlm/tests/mock_lm.py#L27)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](../rlm/clients/base_lm.md#BaseLM.__init__), [`model_name`](../rlm/clients/base_lm.md#BaseLM.model_name)
- used by: [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`get_last_usage`](../rlm/clients/base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](../rlm/clients/base_lm.md#BaseLM.get_usage_summary), [`completion`](../rlm/clients/base_lm.md#BaseLM.completion), [`acompletion`](../rlm/clients/base_lm.md#BaseLM.acompletion)  (4 test-only)

