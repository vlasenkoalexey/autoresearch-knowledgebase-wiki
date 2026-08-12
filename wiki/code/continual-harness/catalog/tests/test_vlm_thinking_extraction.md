---
title: 'Module: tests/test_vlm_thinking_extraction.py'
type: catalog
provenance: extracted
module: tests/test_vlm_thinking_extraction.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_vlm_thinking_extraction`/
symbols:
  TestThinkingFromContentParts.test_interleaved_text_and_calls_preserves_order: TestThinkingFromContentParts#test_interleaved_text_and_calls_preserves_order().
  TestExtractThinkingFromGeminiLikeResponse.test_adapter_with_two_calls: TestExtractThinkingFromGeminiLikeResponse#test_adapter_with_two_calls().
  TestThinkingFromContentParts.test_multiple_function_calls_newline_separated: TestThinkingFromContentParts#test_multiple_function_calls_newline_separated().
  TestThinkingFromContentParts.test_empty_parts_fallback: TestThinkingFromContentParts#test_empty_parts_fallback().
  TestExtractThinkingFromGeminiLikeResponse.test_missing_candidates: TestExtractThinkingFromGeminiLikeResponse#test_missing_candidates().
  _adapter_from_parts: _adapter_from_parts().
  TestThinkingFromContentParts: TestThinkingFromContentParts#
  TestExtractThinkingFromGeminiLikeResponse: TestExtractThinkingFromGeminiLikeResponse#
---
# Module: [`tests/test_vlm_thinking_extraction.py`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py)

## Classes
### `TestExtractThinkingFromGeminiLikeResponse`
- def: [`tests/test_vlm_thinking_extraction.py:46`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L46)
- signature: `class TestExtractThinkingFromGeminiLikeResponse:`
- members:
  - `test_adapter_with_two_calls(self)` — [`L47`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L47)
  - `test_missing_candidates(self)` — [`L58`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L58)
- uses (calls/refs, reference-scoped): [`_extract_thinking_from_gemini_like_response`](../utils/agent_infrastructure/vlm_backends.md#_extract_thinking_from_gemini_like_response), [`_openai_tool_call_part`](../utils/agent_infrastructure/vlm_backends.md#_openai_tool_call_part)  (1 test-only)

### `TestThinkingFromContentParts`
- def: [`tests/test_vlm_thinking_extraction.py:22`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L22)
- signature: `class TestThinkingFromContentParts:`
- members:
  - `test_empty_parts_fallback(self)` — [`L42`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L42)
  - `test_interleaved_text_and_calls_preserves_order(self)` — [`L34`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L34)
  - `test_multiple_function_calls_newline_separated(self)` — [`L23`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L23)
- uses (calls/refs, reference-scoped): [`_openai_text_part`](../utils/agent_infrastructure/vlm_backends.md#_openai_text_part), [`_openai_tool_call_part`](../utils/agent_infrastructure/vlm_backends.md#_openai_tool_call_part), [`_thinking_from_content_parts`](../utils/agent_infrastructure/vlm_backends.md#_thinking_from_content_parts)

## Functions
- `_adapter_from_parts(parts)` — [`L16`](../../../../../raw/code/continual-harness/tests/test_vlm_thinking_extraction.py#L16)

