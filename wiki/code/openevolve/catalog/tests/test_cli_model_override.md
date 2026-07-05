---
title: 'Module: tests/test_cli_model_override.py'
type: catalog
provenance: extracted
module: tests/test_cli_model_override.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_cli_model_override`/TestCLIModelOverride#
symbols:
  TestCLIModelOverride.test_rebuild_models_with_weights: test_rebuild_models_with_weights().
  TestCLIModelOverride.test_rebuild_preserves_shared_config: test_rebuild_preserves_shared_config().
  TestCLIModelOverride.test_rebuild_models_with_both_models: test_rebuild_models_with_both_models().
  TestCLIModelOverride.test_rebuild_models_zero_weight_secondary: test_rebuild_models_zero_weight_secondary().
  TestCLIModelOverride.test_rebuild_models_primary_only: test_rebuild_models_primary_only().
  TestCLIModelOverride.test_rebuild_models_with_config_file_override: test_rebuild_models_with_config_file_override().
  TestCLIModelOverride.test_evaluator_models_updated_after_rebuild: test_evaluator_models_updated_after_rebuild().
  TestCLIModelOverride: ''
---
# Module: [`tests/test_cli_model_override.py`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py)

## Classes
### `TestCLIModelOverride`  ·  implements/extends TestCase
- def: [`tests/test_cli_model_override.py:11`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L11)
- doc: Test that CLI model overrides work correctly
- signature: `class TestCLIModelOverride(unittest.TestCase):`
- members:
  - `test_evaluator_models_updated_after_rebuild(self)` — [`L121`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L121) — Test that evaluator_models list is also updated after rebuild
  - `test_rebuild_models_primary_only(self)` — [`L38`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L38) — Test rebuilding with only primary model
  - `test_rebuild_models_with_both_models(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L14) — Test rebuilding models with both primary and secondary models
  - `test_rebuild_models_with_config_file_override(self)` — [`L89`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L89) — Test CLI override of config file models
  - `test_rebuild_models_with_weights(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L49) — Test rebuilding with custom weights
  - `test_rebuild_models_zero_weight_secondary(self)` — [`L63`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L63) — Test that secondary model with zero weight is excluded
  - `test_rebuild_preserves_shared_config(self)` — [`L76`](../../../../../raw/code/openevolve/tests/test_cli_model_override.py#L76) — Test that rebuilding preserves shared configuration
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`llm`](../openevolve/config.md#Config.llm), [`models`](../openevolve/config.md#LLMConfig.models), [`rebuild_models`](../openevolve/config.md#LLMConfig.rebuild_models), [`load_config`](../openevolve/config.md#load_config), [`name`](../openevolve/config.md#LLMModelConfig.name), [`weight`](../openevolve/config.md#LLMModelConfig.weight), [`evaluator_models`](../openevolve/config.md#LLMConfig.evaluator_models), [`primary_model`](../openevolve/config.md#LLMConfig.primary_model), [`secondary_model_weight`](../openevolve/config.md#LLMConfig.secondary_model_weight), [`api_base`](../openevolve/config.md#LLMModelConfig.api_base), [`secondary_model`](../openevolve/config.md#LLMConfig.secondary_model), [`api_base`](../openevolve/config.md#LLMConfig.api_base), [`temperature`](../openevolve/config.md#LLMConfig.temperature), [`temperature`](../openevolve/config.md#LLMModelConfig.temperature), [`primary_model_weight`](../openevolve/config.md#LLMConfig.primary_model_weight)

