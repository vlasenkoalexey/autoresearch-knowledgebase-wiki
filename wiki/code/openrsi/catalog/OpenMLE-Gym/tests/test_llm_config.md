---
title: 'Module: OpenMLE-Gym/tests/test_llm_config.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_llm_config.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_llm_config`/LLMConfigTests#
symbols:
  LLMConfigTests.test_stage_settings_are_independent: test_stage_settings_are_independent().
  LLMConfigTests.test_legacy_openai_settings_are_fallbacks: test_legacy_openai_settings_are_fallbacks().
  LLMConfigTests.test_explicit_eval_settings_select_openai_quality_path: test_explicit_eval_settings_select_openai_quality_path().
  LLMConfigTests: ''
---
# Module: [`OpenMLE-Gym/tests/test_llm_config.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_llm_config.py)

## Classes
### `LLMConfigTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_llm_config.py:10`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_llm_config.py#L10)
- signature: `class LLMConfigTests(unittest.TestCase):`
- members:
  - `test_explicit_eval_settings_select_openai_quality_path(self)` — [`L41`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_llm_config.py#L41)
  - `test_legacy_openai_settings_are_fallbacks(self)` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_llm_config.py#L28)
  - `test_stage_settings_are_independent(self)` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_llm_config.py#L11)
- uses (calls/refs, reference-scoped): [`_evaluate_with_ai`](../openmle_gym/local_evaluator.md#_evaluate_with_ai), [`eval_llm_config`](../openmle_gym/llm_config.md#eval_llm_config), [`build_llm_config`](../openmle_gym/llm_config.md#build_llm_config), [`api_key`](../openmle_gym/llm_config.md#OpenAICompatibleConfig.api_key), [`model`](../openmle_gym/llm_config.md#OpenAICompatibleConfig.model), [`base_url`](../openmle_gym/llm_config.md#OpenAICompatibleConfig.base_url)

