---
title: 'Module: tests/test_reasoning_effort_config.py'
type: catalog
provenance: extracted
module: tests/test_reasoning_effort_config.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_reasoning_effort_config`/TestReasoningEffortConfig#
symbols:
  TestReasoningEffortConfig.test_reasoning_effort_in_llm_config: test_reasoning_effort_in_llm_config().
  TestReasoningEffortConfig.test_reasoning_effort_inheritance: test_reasoning_effort_inheritance().
  TestReasoningEffortConfig.test_reasoning_effort_model_override: test_reasoning_effort_model_override().
  TestReasoningEffortConfig.test_yaml_file_loading_with_reasoning_effort: test_yaml_file_loading_with_reasoning_effort().
  TestReasoningEffortConfig.test_reasoning_effort_in_model_config: test_reasoning_effort_in_model_config().
  TestReasoningEffortConfig.test_reasoning_effort_passed_to_api_params: test_reasoning_effort_passed_to_api_params().
  TestReasoningEffortConfig.test_openai_llm_uses_reasoning_effort: test_openai_llm_uses_reasoning_effort().
  TestReasoningEffortConfig: ''
---
# Module: [`tests/test_reasoning_effort_config.py`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py)

## Classes
### `TestReasoningEffortConfig`  ·  implements/extends TestCase
- def: [`tests/test_reasoning_effort_config.py:16`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L16)
- doc: Tests for reasoning_effort parameter handling in configuration
- signature: `class TestReasoningEffortConfig(unittest.TestCase):`
- members:
  - `test_openai_llm_uses_reasoning_effort(self)` — [`L119`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L119) — Test that OpenAILLM stores and uses reasoning_effort from config
  - `test_reasoning_effort_in_llm_config(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L19) — Test that reasoning_effort can be loaded from YAML config at LLM level
  - `test_reasoning_effort_in_model_config(self)` — [`L46`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L46) — Test that reasoning_effort can be specified per model
  - `test_reasoning_effort_inheritance(self)` — [`L73`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L73) — Test that model configs inherit reasoning_effort from parent LLM config
  - `test_reasoning_effort_model_override(self)` — [`L96`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L96) — Test that model-level reasoning_effort overrides LLM-level
  - `test_reasoning_effort_passed_to_api_params(self)` — [`L143`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L143) — Test that reasoning_effort is included in API call parameters — documented in [openevolve-llm-openai](../../concepts/openevolve-llm-openai.md)
  - `test_yaml_file_loading_with_reasoning_effort(self)` — [`L181`](../../../../../raw/code/openevolve/tests/test_reasoning_effort_config.py#L181) — Test loading reasoning_effort from actual YAML file
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`llm`](../openevolve/config.md#Config.llm), [`models`](../openevolve/config.md#LLMConfig.models), [`from_dict`](../openevolve/config.md#Config.from_dict), [`client`](../openevolve/llm/openai.md#OpenAILLM.client), [`from_yaml`](../openevolve/config.md#Config.from_yaml), [`OpenAILLM`](../openevolve/llm/openai.md#OpenAILLM), [`reasoning_effort`](../openevolve/config.md#LLMConfig.reasoning_effort), [`reasoning_effort`](../openevolve/config.md#LLMModelConfig.reasoning_effort), [`_call_api`](../openevolve/llm/openai.md#OpenAILLM._call_api), [`reasoning_effort`](../openevolve/llm/openai.md#OpenAILLM.reasoning_effort)

