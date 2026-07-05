---
title: 'Module: tests/test_evaluator_timeout.py'
type: catalog
provenance: extracted
module: tests/test_evaluator_timeout.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_evaluator_timeout`/Test
symbols:
  TestEvaluatorTimeout.run_test: EvaluatorTimeout#run_test().
  TestEvaluatorTimeout._create_evaluator: EvaluatorTimeout#_create_evaluator().
  TestTimeoutIntegration.run_test: TimeoutIntegration#run_test().
  TestEvaluatorTimeout.test_eval_file: EvaluatorTimeout#test_eval_file.
  TestEvaluatorTimeout.tearDown: EvaluatorTimeout#tearDown().
  TestEvaluatorTimeout.test_fast_evaluation_completes: EvaluatorTimeout#test_fast_evaluation_completes().
  TestEvaluatorTimeout.test_short_evaluation_completes: EvaluatorTimeout#test_short_evaluation_completes().
  TestEvaluatorTimeout.test_long_evaluation_times_out: EvaluatorTimeout#test_long_evaluation_times_out().
  TestEvaluatorTimeout.test_cascade_evaluation_timeout_stage1: EvaluatorTimeout#test_cascade_evaluation_timeout_stage1().
  TestEvaluatorTimeout.test_cascade_evaluation_timeout_stage2: EvaluatorTimeout#test_cascade_evaluation_timeout_stage2().
  TestEvaluatorTimeout.test_cascade_evaluation_timeout_stage3: EvaluatorTimeout#test_cascade_evaluation_timeout_stage3().
  TestEvaluatorTimeout.test_timeout_config_respected: EvaluatorTimeout#test_timeout_config_respected().
  TestEvaluatorTimeout.test_multiple_retries_with_errors: EvaluatorTimeout#test_multiple_retries_with_errors().
  TestEvaluatorTimeout.test_timeout_does_not_trigger_retries: EvaluatorTimeout#test_timeout_does_not_trigger_retries().
  TestEvaluatorTimeout.test_artifacts_on_timeout: EvaluatorTimeout#test_artifacts_on_timeout().
  TestTimeoutIntegration.test_real_world_scenario: TimeoutIntegration#test_real_world_scenario().
  TestEvaluatorTimeout: EvaluatorTimeout#
  TestEvaluatorTimeout.setUp: EvaluatorTimeout#setUp().
  TestTimeoutIntegration: TimeoutIntegration#
---
# Module: [`tests/test_evaluator_timeout.py`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py)

## Classes
### `TestEvaluatorTimeout`  ·  implements/extends TestCase
- def: [`tests/test_evaluator_timeout.py:16`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L16)
- doc: Tests for evaluator timeout functionality
- signature: `class TestEvaluatorTimeout(unittest.TestCase):`
- members:
  - `_create_evaluator(self, timeout=3, cascade_evaluation=False)` — [`L87`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L87) — Helper to create evaluator with given settings (shorter timeout for faster tests) — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `run_test()` — [`L105`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L105)
  - `setUp(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L19) — Set up test evaluation file
  - `tearDown(self)` — [`L82`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L82) — Clean up test files
  - `test_artifacts_on_timeout(self)` — [`L347`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L347) — Test that timeout artifacts are properly captured
  - `test_cascade_evaluation_timeout_stage1(self)` — [`L172`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L172) — Test timeout in cascade evaluation stage 1
  - `test_cascade_evaluation_timeout_stage2(self)` — [`L196`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L196) — Test timeout in cascade evaluation stage 2
  - `test_cascade_evaluation_timeout_stage3(self)` — [`L222`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L222) — Test timeout in cascade evaluation stage 3
  - `test_fast_evaluation_completes(self)` — [`L102`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L102) — Test that fast evaluations complete successfully
  - `test_long_evaluation_times_out(self)` — [`L148`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L148) — Test that long evaluations time out properly
  - `test_multiple_retries_with_errors(self)` — [`L274`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L274) — Test that retries work correctly with actual errors (not timeouts)
  - `test_short_evaluation_completes(self)` — [`L125`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L125) — Test that evaluations shorter than timeout complete successfully
  - `test_timeout_config_respected(self)` — [`L250`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L250) — Test that the timeout configuration value is actually used
  - `test_timeout_does_not_trigger_retries(self)` — [`L311`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L311) — Test that timeouts do not trigger retries (correct behavior)
  - `test_eval_file` — [`L22`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L22)
- uses (calls/refs, reference-scoped): [`evaluate_program`](../openevolve/evaluator.md#Evaluator.evaluate_program), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`cascade_evaluation`](../openevolve/config.md#EvaluatorConfig.cascade_evaluation), [`timeout`](../openevolve/config.md#EvaluatorConfig.timeout), [`EvaluatorConfig`](../openevolve/config.md#EvaluatorConfig), [`get_pending_artifacts`](../openevolve/evaluator.md#Evaluator.get_pending_artifacts), [`max_retries`](../openevolve/config.md#EvaluatorConfig.max_retries), [`cascade_thresholds`](../openevolve/config.md#EvaluatorConfig.cascade_thresholds)

### `TestTimeoutIntegration`  ·  implements/extends TestCase
- def: [`tests/test_evaluator_timeout.py:393`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L393)
- doc: Integration tests for timeout functionality
- signature: `class TestTimeoutIntegration(unittest.TestCase):`
- members:
  - `run_test()` — [`L399`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L399) — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `test_real_world_scenario(self)` — [`L396`](../../../../../raw/code/openevolve/tests/test_evaluator_timeout.py#L396) — Test a scenario similar to the reported bug
- uses (calls/refs, reference-scoped): [`evaluate_program`](../openevolve/evaluator.md#Evaluator.evaluate_program), [`Evaluator`](../openevolve/evaluator.md#Evaluator), [`cascade_evaluation`](../openevolve/config.md#EvaluatorConfig.cascade_evaluation), [`timeout`](../openevolve/config.md#EvaluatorConfig.timeout), [`EvaluatorConfig`](../openevolve/config.md#EvaluatorConfig), [`parallel_evaluations`](../openevolve/config.md#EvaluatorConfig.parallel_evaluations), [`max_retries`](../openevolve/config.md#EvaluatorConfig.max_retries)

