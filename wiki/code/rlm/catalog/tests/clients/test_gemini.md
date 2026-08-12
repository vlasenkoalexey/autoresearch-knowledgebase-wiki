---
title: 'Module: tests/clients/test_gemini.py'
type: catalog
provenance: extracted
module: tests/clients/test_gemini.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.clients.test_gemini`/
symbols:
  TestGeminiClientUnit.test_get_last_usage: TestGeminiClientUnit#test_get_last_usage().
  TestGeminiClientUnit.test_usage_tracking_initialization: TestGeminiClientUnit#test_usage_tracking_initialization().
  TestGeminiClientIntegration.test_simple_completion: TestGeminiClientIntegration#test_simple_completion().
  TestGeminiClientUnit.test_completion_with_mocked_response: TestGeminiClientUnit#test_completion_with_mocked_response().
  test: test.
  TestGeminiClientUnit.test_get_usage_summary_empty: TestGeminiClientUnit#test_get_usage_summary_empty().
  TestGeminiClientIntegration.test_message_list_completion: TestGeminiClientIntegration#test_message_list_completion().
  TestGeminiClientUnit.test_init_with_api_key: TestGeminiClientUnit#test_init_with_api_key().
  TestGeminiClientUnit.test_init_default_model: TestGeminiClientUnit#test_init_default_model().
  TestGeminiClientUnit.test_prepare_contents_string: TestGeminiClientUnit#test_prepare_contents_string().
  TestGeminiClientUnit.test_prepare_contents_messages_with_system: TestGeminiClientUnit#test_prepare_contents_messages_with_system().
  TestGeminiClientUnit.test_prepare_contents_role_mapping: TestGeminiClientUnit#test_prepare_contents_role_mapping().
  TestGeminiClientUnit.test_prepare_contents_invalid_type: TestGeminiClientUnit#test_prepare_contents_invalid_type().
  TestGeminiClientUnit.test_completion_requires_model: TestGeminiClientUnit#test_completion_requires_model().
  TestGeminiClientIntegration.test_async_completion: TestGeminiClientIntegration#test_async_completion().
  TestGeminiClientUnit.test_init_requires_api_key: TestGeminiClientUnit#test_init_requires_api_key().
  TestGeminiClientIntegration: TestGeminiClientIntegration#
  TestGeminiClientUnit: TestGeminiClientUnit#
---
# Module: [`tests/clients/test_gemini.py`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py)

## Classes
### `TestGeminiClientIntegration`
- def: [`tests/clients/test_gemini.py:139`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L139)
- doc: Integration tests that require a real API key.
- signature: `class TestGeminiClientIntegration:`
- members:
  - `test_async_completion(self)` — [`L175`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L175) — Test async completion.
  - `test_message_list_completion(self)` — [`L161`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L161) — Test completion with message list format.
  - `test_simple_completion(self)` — [`L146`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L146) — Test a simple completion with real API.
- uses (calls/refs, reference-scoped): [`model_usage_summaries`](../../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../../rlm/core/types.md#ModelUsageSummary.total_calls), [`get_usage_summary`](../../rlm/clients/gemini.md#GeminiClient.get_usage_summary), [`GeminiClient`](../../rlm/clients/gemini.md#GeminiClient), [`completion`](../../rlm/clients/gemini.md#GeminiClient.completion), [`acompletion`](../../rlm/clients/gemini.md#GeminiClient.acompletion)
- used by: (1 test-only callers)

### `TestGeminiClientUnit`
- def: [`tests/clients/test_gemini.py:15`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L15)
- doc: Unit tests that don't require API calls.
- signature: `class TestGeminiClientUnit:`
- members:
  - `test_completion_requires_model(self)` — [`L111`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L111) — Test completion raises when no model specified.
  - `test_completion_with_mocked_response(self)` — [`L118`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L118) — Test completion with mocked API response.
  - `test_get_last_usage(self)` — [`L55`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L55) — Test last usage returns correct format.
  - `test_get_usage_summary_empty(self)` — [`L47`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L47) — Test usage summary when no calls have been made.
  - `test_init_default_model(self)` — [`L24`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L24) — Test client uses default model name.
  - `test_init_requires_api_key(self)` — [`L30`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L30) — Test client raises error when no API key provided.
  - `test_init_with_api_key(self)` — [`L18`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L18) — Test client initialization with explicit API key.
  - `test_prepare_contents_invalid_type(self)` — [`L104`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L104) — Test _prepare_contents raises on invalid input.
  - `test_prepare_contents_messages_with_system(self)` — [`L75`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L75) — Test _prepare_contents extracts system message.
  - `test_prepare_contents_role_mapping(self)` — [`L88`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L88) — Test _prepare_contents maps assistant to model.
  - `test_prepare_contents_string(self)` — [`L67`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L67) — Test _prepare_contents with string input.
  - `test_usage_tracking_initialization(self)` — [`L37`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L37) — Test that usage tracking is properly initialized.
- uses (calls/refs, reference-scoped): [`UsageSummary`](../../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../../rlm/core/types.md#ModelUsageSummary), [`model_usage_summaries`](../../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`get_usage_summary`](../../rlm/clients/gemini.md#GeminiClient.get_usage_summary), [`GeminiClient`](../../rlm/clients/gemini.md#GeminiClient), [`get_last_usage`](../../rlm/clients/gemini.md#GeminiClient.get_last_usage), [`completion`](../../rlm/clients/gemini.md#GeminiClient.completion), [`_prepare_contents`](../../rlm/clients/gemini.md#GeminiClient._prepare_contents), [`last_completion_tokens`](../../rlm/clients/gemini.md#GeminiClient.last_completion_tokens), [`last_prompt_tokens`](../../rlm/clients/gemini.md#GeminiClient.last_prompt_tokens), [`model_call_counts`](../../rlm/clients/gemini.md#GeminiClient.model_call_counts), [`model_input_tokens`](../../rlm/clients/gemini.md#GeminiClient.model_input_tokens), [`model_name`](../../rlm/clients/gemini.md#GeminiClient.model_name), [`model_output_tokens`](../../rlm/clients/gemini.md#GeminiClient.model_output_tokens)

## Module values
- `test` — [`L184`](../../../../../../raw/code/rlm/tests/clients/test_gemini.py#L184)

