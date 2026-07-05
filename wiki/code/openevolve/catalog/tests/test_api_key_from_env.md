---
title: 'Module: tests/test_api_key_from_env.py'
type: catalog
provenance: extracted
module: tests/test_api_key_from_env.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_api_key_from_env`/TestEnvVarSubstitution#
symbols:
  TestEnvVarSubstitution.test_api_key_env_var_in_llm_config: test_api_key_env_var_in_llm_config().
  TestEnvVarSubstitution.test_api_key_env_var_per_model: test_api_key_env_var_per_model().
  TestEnvVarSubstitution.test_api_key_env_var_in_evaluator_models: test_api_key_env_var_in_evaluator_models().
  TestEnvVarSubstitution.test_mixed_api_key_sources: test_mixed_api_key_sources().
  TestEnvVarSubstitution.test_yaml_file_loading_with_env_var: test_yaml_file_loading_with_env_var().
  TestEnvVarSubstitution.test_api_key: test_api_key.
  TestEnvVarSubstitution.test_api_key_env_var_in_model_config: test_api_key_env_var_in_model_config().
  TestEnvVarSubstitution.test_env_var: test_env_var.
  TestEnvVarSubstitution.test_resolve_env_var_with_match: test_resolve_env_var_with_match().
  TestEnvVarSubstitution.test_api_key_direct_value: test_api_key_direct_value().
  TestEnvVarSubstitution.test_api_key_none: test_api_key_none().
  TestEnvVarSubstitution.tearDown: tearDown().
  TestEnvVarSubstitution.test_resolve_env_var_no_match: test_resolve_env_var_no_match().
  TestEnvVarSubstitution.test_resolve_env_var_none: test_resolve_env_var_none().
  TestEnvVarSubstitution.test_resolve_env_var_missing_var: test_resolve_env_var_missing_var().
  TestEnvVarSubstitution: ''
  TestEnvVarSubstitution.setUp: setUp().
---
# Module: [`tests/test_api_key_from_env.py`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py)

## Classes
### `TestEnvVarSubstitution`  ·  implements/extends TestCase
- def: [`tests/test_api_key_from_env.py:12`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L12)
- doc: Tests for ${VAR} environment variable substitution in api_key fields
- signature: `class TestEnvVarSubstitution(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L15`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L15) — Set up test environment variables
  - `tearDown(self)` — [`L21`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L21) — Clean up test environment variables
  - `test_api_key_direct_value(self)` — [`L55`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L55) — Test that direct api_key value still works
  - `test_api_key_env_var_in_evaluator_models(self)` — [`L120`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L120) — Test that api_key ${VAR} works in evaluator_models
  - `test_api_key_env_var_in_llm_config(self)` — [`L68`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L68) — Test that api_key ${VAR} works at LLM config level
  - `test_api_key_env_var_in_model_config(self)` — [`L49`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L49) — Test that api_key ${VAR} works in LLMModelConfig
  - `test_api_key_env_var_per_model(self)` — [`L85`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L85) — Test that api_key ${VAR} can be specified per model
  - `test_api_key_none(self)` — [`L62`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L62) — Test that api_key can be None
  - `test_mixed_api_key_sources(self)` — [`L163`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L163) — Test mixing direct api_key and ${VAR} in same config
  - `test_resolve_env_var_missing_var(self)` — [`L41`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L41) — Test that missing environment variable raises ValueError
  - `test_resolve_env_var_no_match(self)` — [`L31`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L31) — Test that strings without ${VAR} are returned unchanged
  - `test_resolve_env_var_none(self)` — [`L36`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L36) — Test that None is returned unchanged
  - `test_resolve_env_var_with_match(self)` — [`L26`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L26) — Test that _resolve_env_var resolves ${VAR} syntax
  - `test_yaml_file_loading_with_env_var(self)` — [`L141`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L141) — Test loading api_key ${VAR} from actual YAML file
  - `test_api_key` — [`L18`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L18)
  - `test_env_var` — [`L17`](../../../../../raw/code/openevolve/tests/test_api_key_from_env.py#L17)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`llm`](../openevolve/config.md#Config.llm), [`models`](../openevolve/config.md#LLMConfig.models), [`from_dict`](../openevolve/config.md#Config.from_dict), [`LLMModelConfig`](../openevolve/config.md#LLMModelConfig), [`api_key`](../openevolve/config.md#LLMModelConfig.api_key), [`name`](../openevolve/config.md#LLMModelConfig.name), [`from_yaml`](../openevolve/config.md#Config.from_yaml), [`evaluator_models`](../openevolve/config.md#LLMConfig.evaluator_models), [`_resolve_env_var`](../openevolve/config.md#_resolve_env_var)

