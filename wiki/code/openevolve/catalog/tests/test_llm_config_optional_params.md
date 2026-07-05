---
title: 'Module: tests/test_llm_config_optional_params.py'
type: catalog
provenance: extracted
module: tests/test_llm_config_optional_params.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_llm_config_optional_params`/Test
symbols:
  TestConfigFromDictWithOptionalParams.test_config_with_only_temperature: ConfigFromDictWithOptionalParams#test_config_with_only_temperature().
  TestConfigFromDictWithOptionalParams.test_config_with_both_params: ConfigFromDictWithOptionalParams#test_config_with_both_params().
  TestConfigFromDictWithOptionalParams.test_models_inherit_optional_params: ConfigFromDictWithOptionalParams#test_models_inherit_optional_params().
  TestConfigFromDictWithOptionalParams.test_config_with_null_temperature_uses_default: ConfigFromDictWithOptionalParams#test_config_with_null_temperature_uses_default().
  TestConfigFromDictWithOptionalParams.test_config_with_null_top_p: ConfigFromDictWithOptionalParams#test_config_with_null_top_p().
  TestConfigFromDictWithOptionalParams.test_config_with_only_top_p: ConfigFromDictWithOptionalParams#test_config_with_only_top_p().
  TestOptionalTemperatureTopP.test_type_annotation_allows_none: OptionalTemperatureTopP#test_type_annotation_allows_none().
  TestOptionalTemperatureTopP.test_type_annotation_allows_float: OptionalTemperatureTopP#test_type_annotation_allows_float().
  TestOptionalTemperatureTopP.test_llm_config_temperature_default: OptionalTemperatureTopP#test_llm_config_temperature_default().
  TestOptionalTemperatureTopP.test_llm_config_top_p_default_is_none: OptionalTemperatureTopP#test_llm_config_top_p_default_is_none().
  TestOptionalTemperatureTopP.test_model_config_temperature_none_by_default: OptionalTemperatureTopP#test_model_config_temperature_none_by_default().
  TestOptionalTemperatureTopP.test_model_config_top_p_none_by_default: OptionalTemperatureTopP#test_model_config_top_p_none_by_default().
  TestOptionalTemperatureTopP: OptionalTemperatureTopP#
  TestConfigFromDictWithOptionalParams: ConfigFromDictWithOptionalParams#
---
# Module: [`tests/test_llm_config_optional_params.py`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py)

## Classes
### `TestConfigFromDictWithOptionalParams`  ·  implements/extends TestCase
- def: [`tests/test_llm_config_optional_params.py:47`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L47)
- doc: Tests for loading config with optional temperature/top_p from dict
- signature: `class TestConfigFromDictWithOptionalParams(unittest.TestCase):`
- members:
  - `test_config_with_both_params(self)` — [`L98`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L98) — Test config with both temperature and top_p set (OpenAI compatible)
  - `test_config_with_null_temperature_uses_default(self)` — [`L50`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L50) — Test loading config with null temperature uses default
  - `test_config_with_null_top_p(self)` — [`L63`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L63) — Test loading config with null top_p
  - `test_config_with_only_temperature(self)` — [`L74`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L74) — Test config with only temperature set (typical for Anthropic)
  - `test_config_with_only_top_p(self)` — [`L86`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L86) — Test config with only top_p set
  - `test_models_inherit_optional_params(self)` — [`L111`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L111) — Test that models inherit temperature/top_p from parent config
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`llm`](../openevolve/config.md#Config.llm), [`models`](../openevolve/config.md#LLMConfig.models), [`from_dict`](../openevolve/config.md#Config.from_dict), [`temperature`](../openevolve/config.md#LLMConfig.temperature), [`top_p`](../openevolve/config.md#LLMConfig.top_p), [`temperature`](../openevolve/config.md#LLMModelConfig.temperature)

### `TestOptionalTemperatureTopP`  ·  implements/extends TestCase
- def: [`tests/test_llm_config_optional_params.py:11`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L11)
- doc: Tests for optional temperature and top_p parameters
- signature: `class TestOptionalTemperatureTopP(unittest.TestCase):`
- members:
  - `test_llm_config_temperature_default(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L14) — Test that temperature defaults to 0.7 in LLMConfig
  - `test_llm_config_top_p_default_is_none(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L19) — Test that top_p defaults to None in LLMConfig (for Anthropic compatibility)
  - `test_model_config_temperature_none_by_default(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L24) — Test that LLMModelConfig temperature is None by default
  - `test_model_config_top_p_none_by_default(self)` — [`L29`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L29) — Test that LLMModelConfig top_p is None by default
  - `test_type_annotation_allows_float(self)` — [`L40`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L40) — Test that temperature and top_p can be set to float values
  - `test_type_annotation_allows_none(self)` — [`L34`](../../../../../raw/code/openevolve/tests/test_llm_config_optional_params.py#L34) — Test that temperature and top_p can be set to None
- uses (calls/refs, reference-scoped): [`LLMModelConfig`](../openevolve/config.md#LLMModelConfig), [`LLMConfig`](../openevolve/config.md#LLMConfig), [`temperature`](../openevolve/config.md#LLMConfig.temperature), [`top_p`](../openevolve/config.md#LLMConfig.top_p), [`temperature`](../openevolve/config.md#LLMModelConfig.temperature), [`top_p`](../openevolve/config.md#LLMModelConfig.top_p)

