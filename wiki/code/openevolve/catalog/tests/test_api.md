---
title: 'Module: tests/test_api.py'
type: catalog
provenance: extracted
module: tests/test_api.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_api`/TestAPIFunctions#
symbols:
  TestAPIFunctions.test_evolve_function_evaluator_works_in_subprocess: test_evolve_function_evaluator_works_in_subprocess().
  TestAPIFunctions.test_evolve_algorithm_basic: test_evolve_algorithm_basic().
  TestAPIFunctions.test_evolve_function_basic: test_evolve_function_basic().
  TestAPIFunctions.test_evolve_code_basic: test_evolve_code_basic().
  TestAPIFunctions.test_run_evolution_with_config_object: test_run_evolution_with_config_object().
  TestAPIFunctions.test_run_evolution_cleanup_false: test_run_evolution_cleanup_false().
  TestAPIFunctions.temp_dir: temp_dir.
  TestAPIFunctions.test_evolution_result_class: test_evolution_result_class().
  TestAPIFunctions.test_prepare_evaluator_from_callable: test_prepare_evaluator_from_callable().
  TestAPIFunctions.test_prepare_evaluator_callable_works_in_subprocess: test_prepare_evaluator_callable_works_in_subprocess().
  TestAPIFunctions.test_prepare_program_from_file: test_prepare_program_from_file().
  TestAPIFunctions.test_prepare_program_from_string: test_prepare_program_from_string().
  TestAPIFunctions.test_prepare_program_from_list: test_prepare_program_from_list().
  TestAPIFunctions.test_prepare_program_with_existing_markers: test_prepare_program_with_existing_markers().
  TestAPIFunctions.test_prepare_evaluator_from_file: test_prepare_evaluator_from_file().
  TestAPIFunctions.test_prepare_evaluator_from_string: test_prepare_evaluator_from_string().
  TestAPIFunctions.test_prepare_evaluator_string_without_evaluate_function: test_prepare_evaluator_string_without_evaluate_function().
  TestAPIFunctions.tearDown: tearDown().
  TestAPIFunctions.my_evaluator: my_evaluator().
  TestAPIFunctions.initial_sort: initial_sort().
  TestAPIFunctions.bubble_sort: bubble_sort().
  TestAPIFunctions.test_evolve_algorithm_basic.SimpleAlgorithm: test_evolve_algorithm_basic().SimpleAlgorithm#
  TestAPIFunctions.benchmark: benchmark().
  TestAPIFunctions.evaluator: evaluator().
  TestAPIFunctions: ''
  TestAPIFunctions.setUp: setUp().
  TestAPIFunctions.test_evolve_algorithm_basic.SimpleAlgorithm.process: test_evolve_algorithm_basic().SimpleAlgorithm#process().
---
# Module: [`tests/test_api.py`](../../../../../raw/code/openevolve/tests/test_api.py)

## Classes
### `SimpleAlgorithm`
- def: [`tests/test_api.py:290`](../../../../../raw/code/openevolve/tests/test_api.py#L290)
- signature: `class SimpleAlgorithm:`
- members:
  - `process(self, data)` — [`L291`](../../../../../raw/code/openevolve/tests/test_api.py#L291)
- used by: (1 test-only callers)

### `TestAPIFunctions`  ·  implements/extends TestCase
- def: [`tests/test_api.py:22`](../../../../../raw/code/openevolve/tests/test_api.py#L22)
- signature: `class TestAPIFunctions(unittest.TestCase):`
- members:
  - `benchmark(instance)` — [`L294`](../../../../../raw/code/openevolve/tests/test_api.py#L294)
  - `bubble_sort(arr)` — [`L231`](../../../../../raw/code/openevolve/tests/test_api.py#L231)
  - `evaluator(program_path)` — [`L318`](../../../../../raw/code/openevolve/tests/test_api.py#L318)
  - `initial_sort(arr)` — [`L193`](../../../../../raw/code/openevolve/tests/test_api.py#L193)
  - `my_evaluator(program_path)` — [`L117`](../../../../../raw/code/openevolve/tests/test_api.py#L117)
  - `setUp(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_api.py#L24)
  - `tearDown(self)` — [`L27`](../../../../../raw/code/openevolve/tests/test_api.py#L27)
  - `test_evolution_result_class(self)` — [`L31`](../../../../../raw/code/openevolve/tests/test_api.py#L31) — Test EvolutionResult dataclass
  - `test_evolve_algorithm_basic(self)` — [`L288`](../../../../../raw/code/openevolve/tests/test_api.py#L288) — Test evolve_algorithm with simple class
  - `test_evolve_code_basic(self)` — [`L314`](../../../../../raw/code/openevolve/tests/test_api.py#L314) — Test evolve_code with string input
  - `test_evolve_function_basic(self)` — [`L191`](../../../../../raw/code/openevolve/tests/test_api.py#L191) — Test evolve_function with simple test case
  - `test_evolve_function_evaluator_works_in_subprocess(self)` — [`L222`](../../../../../raw/code/openevolve/tests/test_api.py#L222) — Test that evolve_function generates an evaluator that works in a subprocess.
  - `test_prepare_evaluator_callable_works_in_subprocess(self)` — [`L131`](../../../../../raw/code/openevolve/tests/test_api.py#L131) — Test that callable evaluator can be executed in a subprocess
  - `test_prepare_evaluator_from_callable(self)` — [`L115`](../../../../../raw/code/openevolve/tests/test_api.py#L115) — Test _prepare_evaluator with callable function
  - `test_prepare_evaluator_from_file(self)` — [`L103`](../../../../../raw/code/openevolve/tests/test_api.py#L103) — Test _prepare_evaluator with existing file
  - `test_prepare_evaluator_from_string(self)` — [`L169`](../../../../../raw/code/openevolve/tests/test_api.py#L169) — Test _prepare_evaluator with code string
  - `test_prepare_evaluator_string_without_evaluate_function(self)` — [`L183`](../../../../../raw/code/openevolve/tests/test_api.py#L183) — Test _prepare_evaluator raises error for invalid code string
  - `test_prepare_program_from_file(self)` — [`L45`](../../../../../raw/code/openevolve/tests/test_api.py#L45) — Test _prepare_program with existing file
  - `test_prepare_program_from_list(self)` — [`L73`](../../../../../raw/code/openevolve/tests/test_api.py#L73) — Test _prepare_program with list of lines
  - `test_prepare_program_from_string(self)` — [`L57`](../../../../../raw/code/openevolve/tests/test_api.py#L57) — Test _prepare_program with code string
  - `test_prepare_program_with_existing_markers(self)` — [`L87`](../../../../../raw/code/openevolve/tests/test_api.py#L87) — Test _prepare_program doesn't add duplicate markers
  - `test_run_evolution_cleanup_false(self)` — [`L363`](../../../../../raw/code/openevolve/tests/test_api.py#L363) — Test run_evolution with cleanup=False
  - `test_run_evolution_with_config_object(self)` — [`L337`](../../../../../raw/code/openevolve/tests/test_api.py#L337) — Test run_evolution with Config object
  - `temp_dir` — [`L25`](../../../../../raw/code/openevolve/tests/test_api.py#L25)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`best_score`](../openevolve/api.md#EvolutionResult.best_score), [`EvolutionResult`](../openevolve/api.md#EvolutionResult), [`run_evolution`](../openevolve/api.md#run_evolution), [`output_dir`](../openevolve/api.md#EvolutionResult.output_dir), [`best_code`](../openevolve/api.md#EvolutionResult.best_code), [`evolve_function`](../openevolve/api.md#evolve_function), [`best_program`](../openevolve/api.md#EvolutionResult.best_program), [`evolve_code`](../openevolve/api.md#evolve_code), [`metrics`](../openevolve/api.md#EvolutionResult.metrics), [`evolve_algorithm`](../openevolve/api.md#evolve_algorithm), [`_prepare_evaluator`](../openevolve/api.md#_prepare_evaluator), [`_prepare_program`](../openevolve/api.md#_prepare_program)  (1 test-only)

