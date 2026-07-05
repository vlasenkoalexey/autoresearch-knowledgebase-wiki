---
title: 'Module: tests/integration/test_examples_validation.py'
type: catalog
provenance: extracted
module: tests/integration/test_examples_validation.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_examples_validation`/
symbols:
  TestEndToEndWithMockedLLM.test_program_evolution_tracking: TestEndToEndWithMockedLLM#test_program_evolution_tracking().
  TestEndToEndWithMockedLLM.test_database_stores_and_retrieves_programs: TestEndToEndWithMockedLLM#test_database_stores_and_retrieves_programs().
  PROJECT_ROOT: PROJECT_ROOT.
  TestEvaluatorIntegration.test_evaluator_loads_function_minimization: TestEvaluatorIntegration#test_evaluator_loads_function_minimization().
  TestConfigIntegration.test_config_has_required_sections: TestConfigIntegration#test_config_has_required_sections().
  TestFunctionMinimizationExample.test_config_loads: TestFunctionMinimizationExample#test_config_loads().
  TestFunctionMinimizationExample.EXAMPLE_DIR: TestFunctionMinimizationExample#EXAMPLE_DIR.
  TestCirclePackingExample.test_config_loads: TestCirclePackingExample#test_config_loads().
  TestSignalProcessingExample.test_config_loads: TestSignalProcessingExample#test_config_loads().
  TestConfigIntegration.test_all_example_configs_load: TestConfigIntegration#test_all_example_configs_load().
  TestEndToEndWithMockedLLM.test_evaluator_returns_evaluation_result: TestEndToEndWithMockedLLM#test_evaluator_returns_evaluation_result().
  TestCirclePackingExample.EXAMPLE_DIR: TestCirclePackingExample#EXAMPLE_DIR.
  TestSignalProcessingExample.EXAMPLE_DIR: TestSignalProcessingExample#EXAMPLE_DIR.
  TestEndToEndWithMockedLLM.example_dir: TestEndToEndWithMockedLLM#example_dir.
  TestFunctionMinimizationExample.test_initial_program_exists: TestFunctionMinimizationExample#test_initial_program_exists().
  TestFunctionMinimizationExample.test_initial_program_has_evolve_block: TestFunctionMinimizationExample#test_initial_program_has_evolve_block().
  TestFunctionMinimizationExample.test_evaluator_exists: TestFunctionMinimizationExample#test_evaluator_exists().
  TestFunctionMinimizationExample.test_evaluator_has_evaluate_function: TestFunctionMinimizationExample#test_evaluator_has_evaluate_function().
  TestFunctionMinimizationExample.test_evaluator_runs_on_initial_program: TestFunctionMinimizationExample#test_evaluator_runs_on_initial_program().
  TestCirclePackingExample.test_evaluator_exists: TestCirclePackingExample#test_evaluator_exists().
  TestCirclePackingExample.test_evaluator_has_evaluate_function: TestCirclePackingExample#test_evaluator_has_evaluate_function().
  TestSignalProcessingExample.test_evaluator_exists: TestSignalProcessingExample#test_evaluator_exists().
  TestEvaluatorIntegration.test_evaluator_module_has_cascade_functions: TestEvaluatorIntegration#test_evaluator_module_has_cascade_functions().
  TestEndToEndWithMockedLLM.tearDown: TestEndToEndWithMockedLLM#tearDown().
  TestExampleStructure.test_examples_have_required_files: TestExampleStructure#test_examples_have_required_files().
  TestExampleStructure.test_evaluators_are_importable: TestExampleStructure#test_evaluators_are_importable().
  TestEndToEndWithMockedLLM.temp_dir: TestEndToEndWithMockedLLM#temp_dir.
  TestFunctionMinimizationExample: TestFunctionMinimizationExample#
  TestCirclePackingExample: TestCirclePackingExample#
  TestSignalProcessingExample: TestSignalProcessingExample#
  TestEvaluatorIntegration: TestEvaluatorIntegration#
  TestConfigIntegration: TestConfigIntegration#
  TestEndToEndWithMockedLLM: TestEndToEndWithMockedLLM#
  TestEndToEndWithMockedLLM.setUp: TestEndToEndWithMockedLLM#setUp().
  TestExampleStructure: TestExampleStructure#
---
# Module: [`tests/integration/test_examples_validation.py`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py)

## Classes
### `TestCirclePackingExample`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:99`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L99)
- doc: Integration tests for the circle_packing example
- signature: `class TestCirclePackingExample(unittest.TestCase):`
- members:
  - `test_config_loads(self)` — [`L104`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L104) — Test that config files load without errors
  - `test_evaluator_exists(self)` — [`L112`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L112) — Test that evaluator exists
  - `test_evaluator_has_evaluate_function(self)` — [`L117`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L117) — Test that the evaluator has required functions
  - `EXAMPLE_DIR` — [`L102`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L102)
- uses (calls/refs, reference-scoped): [`Config`](../../openevolve/config.md#Config), [`load_config`](../../openevolve/config.md#load_config)  (1 test-only)

### `TestConfigIntegration`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:186`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L186)
- doc: Integration tests for config loading across examples
- signature: `class TestConfigIntegration(unittest.TestCase):`
- members:
  - `test_all_example_configs_load(self)` — [`L190`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L190) — Test that all example config files can be loaded
  - `test_config_has_required_sections(self)` — [`L206`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L206) — Test that loaded configs have required sections
- uses (calls/refs, reference-scoped): [`Config`](../../openevolve/config.md#Config), [`database`](../../openevolve/config.md#Config.database), [`llm`](../../openevolve/config.md#Config.llm), [`evaluator`](../../openevolve/config.md#Config.evaluator), [`prompt`](../../openevolve/config.md#Config.prompt), [`load_config`](../../openevolve/config.md#load_config)  (1 test-only)

### `TestEndToEndWithMockedLLM`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:221`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L221)
- doc: End-to-end tests with mocked LLM responses
- signature: `class TestEndToEndWithMockedLLM(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L224`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L224) — Set up test fixtures
  - `tearDown(self)` — [`L229`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L229) — Clean up
  - `test_database_stores_and_retrieves_programs(self)` — [`L233`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L233) — Test that the database can store and retrieve programs
  - `test_evaluator_returns_evaluation_result(self)` — [`L284`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L284) — Test that evaluators return proper EvaluationResult objects
  - `test_program_evolution_tracking(self)` — [`L254`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L254) — Test that program generations are tracked correctly
  - `example_dir` — [`L227`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L227)
  - `temp_dir` — [`L226`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L226)
- uses (calls/refs, reference-scoped): [`id`](../../openevolve/database.md#Program.id), [`add`](../../openevolve/database.md#ProgramDatabase.add), [`metrics`](../../openevolve/database.md#Program.metrics), [`Program`](../../openevolve/database.md#Program), [`programs`](../../openevolve/database.md#ProgramDatabase.programs), [`code`](../../openevolve/database.md#Program.code), [`metrics`](../../openevolve/evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](../../openevolve/evaluation_result.md#EvaluationResult), [`ProgramDatabase`](../../openevolve/database.md#ProgramDatabase), [`DatabaseConfig`](../../openevolve/config.md#DatabaseConfig), [`generation`](../../openevolve/database.md#Program.generation), [`parent_id`](../../openevolve/database.md#Program.parent_id), [`population_size`](../../openevolve/config.md#DatabaseConfig.population_size)  (1 test-only)

### `TestEvaluatorIntegration`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:152`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L152)
- doc: Integration tests for the Evaluator class with real examples
- signature: `class TestEvaluatorIntegration(unittest.TestCase):`
- members:
  - `test_evaluator_loads_function_minimization(self)` — [`L155`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L155) — Test that Evaluator can load the function_minimization evaluator
  - `test_evaluator_module_has_cascade_functions(self)` — [`L168`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L168) — Test that function_minimization evaluator has cascade functions
- uses (calls/refs, reference-scoped): [`Evaluator`](../../openevolve/evaluator.md#Evaluator), [`cascade_evaluation`](../../openevolve/config.md#EvaluatorConfig.cascade_evaluation), [`timeout`](../../openevolve/config.md#EvaluatorConfig.timeout), [`EvaluatorConfig`](../../openevolve/config.md#EvaluatorConfig), [`evaluate_function`](../../openevolve/evaluator.md#Evaluator.evaluate_function)  (1 test-only)

### `TestExampleStructure`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:307`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L307)
- doc: Tests to verify example directory structure is correct
- signature: `class TestExampleStructure(unittest.TestCase):`
- members:
  - `test_evaluators_are_importable(self)` — [`L339`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L339) — Test that all evaluators can be imported without errors
  - `test_examples_have_required_files(self)` — [`L310`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L310) — Test that examples have the minimum required files
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestFunctionMinimizationExample`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:23`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L23)
- doc: Integration tests for the function_minimization example
- signature: `class TestFunctionMinimizationExample(unittest.TestCase):`
- members:
  - `test_config_loads(self)` — [`L28`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L28) — Test that the config file loads without errors
  - `test_evaluator_exists(self)` — [`L53`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L53) — Test that the evaluator file exists
  - `test_evaluator_has_evaluate_function(self)` — [`L58`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L58) — Test that the evaluator has an evaluate function
  - `test_evaluator_runs_on_initial_program(self)` — [`L71`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L71) — Test that the evaluator can evaluate the initial program
  - `test_initial_program_exists(self)` — [`L38`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L38) — Test that the initial program file exists
  - `test_initial_program_has_evolve_block(self)` — [`L43`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L43) — Test that the initial program has EVOLVE-BLOCK markers
  - `EXAMPLE_DIR` — [`L26`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L26)
- uses (calls/refs, reference-scoped): [`Config`](../../openevolve/config.md#Config), [`load_config`](../../openevolve/config.md#load_config), [`max_iterations`](../../openevolve/config.md#Config.max_iterations)  (1 test-only)

### `TestSignalProcessingExample`  ·  implements/extends TestCase
- def: [`tests/integration/test_examples_validation.py:130`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L130)
- doc: Integration tests for the signal_processing example
- signature: `class TestSignalProcessingExample(unittest.TestCase):`
- members:
  - `test_config_loads(self)` — [`L135`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L135) — Test that the config file loads
  - `test_evaluator_exists(self)` — [`L144`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L144) — Test that evaluator exists
  - `EXAMPLE_DIR` — [`L133`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L133)
- uses (calls/refs, reference-scoped): [`Config`](../../openevolve/config.md#Config), [`load_config`](../../openevolve/config.md#load_config)  (1 test-only)

## Module values
- `PROJECT_ROOT` — [`L16`](../../../../../../raw/code/openevolve/tests/integration/test_examples_validation.py#L16)

