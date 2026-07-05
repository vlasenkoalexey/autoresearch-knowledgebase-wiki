---
title: 'Module: tests/test_cascade_validation.py'
type: catalog
provenance: extracted
module: tests/test_cascade_validation.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_cascade_validation`/TestCascadeValidation#
symbols:
  TestCascadeValidation.config: config.
  TestCascadeValidation.test_direct_evaluate_supports_evaluation_result: test_direct_evaluate_supports_evaluation_result().
  TestCascadeValidation.test_direct_evaluate_supports_dict_result: test_direct_evaluate_supports_dict_result().
  TestCascadeValidation.test_process_evaluation_result_with_artifacts: test_process_evaluation_result_with_artifacts().
  TestCascadeValidation.test_process_evaluation_result_with_dict: test_process_evaluation_result_with_dict().
  TestCascadeValidation._create_evaluator_file: _create_evaluator_file().
  TestCascadeValidation.test_cascade_validation_with_valid_evaluator: test_cascade_validation_with_valid_evaluator().
  TestCascadeValidation.test_cascade_validation_warning_for_missing_functions: test_cascade_validation_warning_for_missing_functions().
  TestCascadeValidation.test_cascade_validation_partial_functions: test_cascade_validation_partial_functions().
  TestCascadeValidation.test_no_cascade_validation_when_disabled: test_no_cascade_validation_when_disabled().
  TestCascadeValidation.test_cascade_validation_with_class_based_evaluator: test_cascade_validation_with_class_based_evaluator().
  TestCascadeValidation.test_cascade_validation_with_syntax_error: test_cascade_validation_with_syntax_error().
  TestCascadeValidation.test_cascade_validation_nonexistent_file: test_cascade_validation_nonexistent_file().
  TestCascadeValidation.mock_evaluate: mock_evaluate().
  TestCascadeValidation.tearDown: tearDown().
  TestCascadeValidation.temp_dir: temp_dir.
  TestCascadeValidation: ''
  TestCascadeValidation.setUp: setUp().
---
# Module: [`tests/test_cascade_validation.py`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py)

## Classes
### `TestCascadeValidation`  ·  implements/extends IsolatedAsyncioTestCase
- def: [`tests/test_cascade_validation.py:14`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L14)
- doc: Tests for cascade evaluation configuration validation
- signature: `class TestCascadeValidation(unittest.IsolatedAsyncioTestCase):`
- members:
  - `_create_evaluator_file(self, filename: str, content: str)` — [`L31`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L31) — Helper to create temporary evaluator file
  - `mock_evaluate(path)` — [`L161`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L161) — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `setUp(self)` — [`L17`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L17) — Set up test evaluator with cascade validation
  - `tearDown(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L24) — Clean up temporary files
  - `test_cascade_validation_nonexistent_file(self)` — [`L264`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L264) — Test cascade validation with nonexistent evaluator file — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_cascade_validation_partial_functions(self)` — [`L90`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L90) — Test cascade validation with only some cascade functions — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_cascade_validation_warning_for_missing_functions(self)` — [`L67`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L67) — Test cascade validation warns when cascade functions are missing — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_cascade_validation_with_class_based_evaluator(self)` — [`L208`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L208) — Test cascade validation with class-based evaluator — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_cascade_validation_with_syntax_error(self)` — [`L247`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L247) — Test cascade validation handles syntax errors gracefully — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_cascade_validation_with_valid_evaluator(self)` — [`L38`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L38) — Test cascade validation with evaluator that has cascade functions
  - `test_direct_evaluate_supports_dict_result(self)` — [`L176`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L176) — Test that _direct_evaluate still supports dict returns — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_direct_evaluate_supports_evaluation_result(self)` — [`L137`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L137) — Test that _direct_evaluate supports EvaluationResult returns — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_no_cascade_validation_when_disabled(self)` — [`L117`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L117) — Test no validation when cascade evaluation is disabled — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_process_evaluation_result_with_artifacts(self)` — [`L277`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L277) — Test that _process_evaluation_result handles artifacts correctly — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `test_process_evaluation_result_with_dict(self)` — [`L299`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L299) — Test that _process_evaluation_result handles dict results correctly — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `config` — [`L19`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L19)
  - `temp_dir` — [`L22`](../../../../../raw/code/openevolve/tests/test_cascade_validation.py#L22)
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`metrics`](../openevolve/evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](../openevolve/evaluation_result.md#EvaluationResult), [`artifacts`](../openevolve/evaluation_result.md#EvaluationResult.artifacts), [`evaluator`](../openevolve/config.md#Config.evaluator), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`cascade_evaluation`](../openevolve/config.md#EvaluatorConfig.cascade_evaluation), [`timeout`](../openevolve/config.md#EvaluatorConfig.timeout), [`_process_evaluation_result`](../openevolve/evaluator.md#Evaluator._process_evaluation_result), [`_direct_evaluate`](../openevolve/evaluator.md#Evaluator._direct_evaluate), [`evaluate_function`](../openevolve/evaluator.md#Evaluator.evaluate_function)

