---
title: 'Module: tests/integration/test_library_api.py'
type: catalog
provenance: extracted
module: tests/integration/test_library_api.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_library_api`/
symbols:
  _get_library_test_config: _get_library_test_config().
  TestLibraryAPIIntegration.test_evolve_function_real_integration: TestLibraryAPIIntegration#test_evolve_function_real_integration().
  TestLibraryAPIIntegration.test_evolve_code_real_integration: TestLibraryAPIIntegration#test_evolve_code_real_integration().
  TestLibraryAPIIntegration.test_run_evolution_real_integration: TestLibraryAPIIntegration#test_run_evolution_real_integration().
  TestLibraryAPIIntegration.simple_multiply: TestLibraryAPIIntegration#simple_multiply().
  TestLibraryAPIIntegration.fibonacci_evaluator: TestLibraryAPIIntegration#fibonacci_evaluator().
  TestLibraryAPIIntegration: TestLibraryAPIIntegration#
  temp_workspace: temp_workspace().
---
# Module: [`tests/integration/test_library_api.py`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py)

## Classes
### `TestLibraryAPIIntegration`
- def: [`tests/integration/test_library_api.py:43`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L43)
- doc: Test OpenEvolve library API with real LLM integration
- signature: `class TestLibraryAPIIntegration:`
- members:
  - `fibonacci_evaluator(program_path)` — [`L123`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L123) — Simple evaluator for fibonacci function
  - `simple_multiply(x, y)` — [`L54`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L54) — A simple function that can be optimized
  - `test_evolve_code_real_integration(self, optillm_server, temp_workspace)` — [`L105`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L105) — Test evolve_code with real optillm server - code string optimization
  - `test_evolve_function_real_integration(self, optillm_server, temp_workspace)` — [`L47`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L47) — Test evolve_function with real optillm server - simple optimization task
  - `test_run_evolution_real_integration(self, optillm_server, temp_workspace)` — [`L191`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L191) — Test run_evolution with real optillm server - basic program evolution
- uses (calls/refs, reference-scoped): [`best_score`](../../openevolve/api.md#EvolutionResult.best_score), [`run_evolution`](../../openevolve/api.md#run_evolution), [`output_dir`](../../openevolve/api.md#EvolutionResult.output_dir), [`best_code`](../../openevolve/api.md#EvolutionResult.best_code), [`evolve_function`](../../openevolve/api.md#evolve_function), [`evolve_code`](../../openevolve/api.md#evolve_code)  (1 test-only)

## Functions
- `_get_library_test_config(port: int = 8000)` — [`L15`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L15) — Get config for library API tests with optillm server
- `temp_workspace()` — [`L308`](../../../../../../raw/code/openevolve/tests/integration/test_library_api.py#L308) — Create a temporary workspace for integration tests

