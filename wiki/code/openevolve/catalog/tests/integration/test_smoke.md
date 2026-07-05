---
title: 'Module: tests/integration/test_smoke.py'
type: catalog
provenance: extracted
module: tests/integration/test_smoke.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_smoke`/TestSmoke#
symbols:
  TestSmoke.test_llm_config_creation: test_llm_config_creation().
  TestSmoke.test_evolution_result_structure: test_evolution_result_structure().
  TestSmoke.test_config_validation: test_config_validation().
  TestSmoke.test_library_api_validation: test_library_api_validation().
  TestSmoke.simple_evaluator: simple_evaluator().
  TestSmoke: ''
---
# Module: [`tests/integration/test_smoke.py`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py)

## Classes
### `TestSmoke`
- def: [`tests/integration/test_smoke.py:14`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L14)
- doc: Fast smoke tests for CI
- signature: `class TestSmoke:`
- members:
  - `simple_evaluator(path)` — [`L28`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L28)
  - `test_config_validation(self)` — [`L42`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L42) — Test configuration validation works
  - `test_evolution_result_structure(self)` — [`L77`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L77) — Test that EvolutionResult has the expected structure
  - `test_library_api_validation(self)` — [`L17`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L17) — Test library API gives proper error messages when not configured
  - `test_llm_config_creation(self)` — [`L57`](../../../../../../raw/code/openevolve/tests/integration/test_smoke.py#L57) — Test that LLM configuration can be created properly
- uses (calls/refs, reference-scoped): [`Program`](../../openevolve/database.md#Program), [`Config`](../../openevolve/config.md#Config), [`database`](../../openevolve/config.md#Config.database), [`llm`](../../openevolve/config.md#Config.llm), [`models`](../../openevolve/config.md#LLMConfig.models), [`LLMModelConfig`](../../openevolve/config.md#LLMModelConfig), [`api_key`](../../openevolve/config.md#LLMModelConfig.api_key), [`name`](../../openevolve/config.md#LLMModelConfig.name), [`in_memory`](../../openevolve/config.md#DatabaseConfig.in_memory), [`best_score`](../../openevolve/api.md#EvolutionResult.best_score), [`EvolutionResult`](../../openevolve/api.md#EvolutionResult), [`weight`](../../openevolve/config.md#LLMModelConfig.weight), [`run_evolution`](../../openevolve/api.md#run_evolution), [`output_dir`](../../openevolve/api.md#EvolutionResult.output_dir), [`best_code`](../../openevolve/api.md#EvolutionResult.best_code), [`max_iterations`](../../openevolve/config.md#Config.max_iterations), [`best_program`](../../openevolve/api.md#EvolutionResult.best_program), [`api_base`](../../openevolve/config.md#LLMModelConfig.api_base), [`metrics`](../../openevolve/api.md#EvolutionResult.metrics), [`retries`](../../openevolve/config.md#LLMConfig.retries), [`retries`](../../openevolve/config.md#LLMModelConfig.retries), [`timeout`](../../openevolve/config.md#LLMModelConfig.timeout)

