---
title: 'Module: tests/test_openai_model_detection.py'
type: catalog
provenance: extracted
module: tests/test_openai_model_detection.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_openai_model_detection`/TestOpenAIReasoningModelDetection#
symbols:
  TestOpenAIReasoningModelDetection.test_reasoning_model_detection: test_reasoning_model_detection().
  TestOpenAIReasoningModelDetection.test_non_openai_api_base: test_non_openai_api_base().
  TestOpenAIReasoningModelDetection.is_reasoning_model: is_reasoning_model().
  TestOpenAIReasoningModelDetection: ''
---
# Module: [`tests/test_openai_model_detection.py`](../../../../../raw/code/openevolve/tests/test_openai_model_detection.py)

## Classes
### `TestOpenAIReasoningModelDetection`  ·  implements/extends TestCase
- def: [`tests/test_openai_model_detection.py:9`](../../../../../raw/code/openevolve/tests/test_openai_model_detection.py#L9)
- doc: Test that OpenAI reasoning models are correctly identified
- signature: `class TestOpenAIReasoningModelDetection(unittest.TestCase):`
- members:
  - `is_reasoning_model(model_name, api_base="https://api.openai.com/v1")` — [`L28`](../../../../../raw/code/openevolve/tests/test_openai_model_detection.py#L28) — Test function that mimics the logic in openai.py
  - `test_non_openai_api_base(self)` — [`L70`](../../../../../raw/code/openevolve/tests/test_openai_model_detection.py#L70) — Test that non-OpenAI API bases don't trigger reasoning model logic
  - `test_reasoning_model_detection(self)` — [`L12`](../../../../../raw/code/openevolve/tests/test_openai_model_detection.py#L12) — Test various model names to ensure correct reasoning model detection

