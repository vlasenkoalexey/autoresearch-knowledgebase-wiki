---
title: 'Module: OpenMLE-Gym/tests/test_batch_independence.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_batch_independence.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_batch_independence`/
symbols:
  BatchIndependenceTests.fake_runner: BatchIndependenceTests#fake_runner().
  BatchIndependenceTests.test_evaluate_item_write_failure_keeps_sibling_and_aggregates: BatchIndependenceTests#test_evaluate_item_write_failure_keeps_sibling_and_aggregates().
  GOOD_METRIC: GOOD_METRIC.
  _make_task: _make_task().
  BatchIndependenceTests.test_overview_crash_keeps_sibling_rows: BatchIndependenceTests#test_overview_crash_keeps_sibling_rows().
  BatchIndependenceTests.test_overview_rejects_task_symlink_outside_batch_root: BatchIndependenceTests#test_overview_rejects_task_symlink_outside_batch_root().
  BatchIndependenceTests.test_evaluate_crash_keeps_sibling_results: BatchIndependenceTests#test_evaluate_crash_keeps_sibling_results().
  BatchIndependenceTests.test_evaluate_duplicate_task_is_an_item_failure: BatchIndependenceTests#test_evaluate_duplicate_task_is_an_item_failure().
  BatchIndependenceTests.test_build_collects_failure_without_cancelling_siblings: BatchIndependenceTests#test_build_collects_failure_without_cancelling_siblings().
  BatchIndependenceTests.test_build_isolated_mode_keeps_outer_task_process: BatchIndependenceTests#test_build_isolated_mode_keeps_outer_task_process().
  BatchIndependenceTests.flaky_write: BatchIndependenceTests#flaky_write().
  HAS_BATCH_DEPS: HAS_BATCH_DEPS.
  BatchIndependenceTests: BatchIndependenceTests#
---
# Module: [`OpenMLE-Gym/tests/test_batch_independence.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py)

## Classes
### `BatchIndependenceTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_batch_independence.py:51`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L51)
- signature: `class BatchIndependenceTests(unittest.TestCase):`
- members:
  - `fake_runner(operation, payload, **kwargs)` — [`L53`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L53)
  - `flaky_write(path, value)` — [`L205`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L205)
  - `test_build_collects_failure_without_cancelling_siblings(self)` — [`L52`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L52)
  - `test_build_isolated_mode_keeps_outer_task_process(self)` — [`L83`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L83)
  - `test_evaluate_crash_keeps_sibling_results(self)` — [`L145`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L145)
  - `test_evaluate_duplicate_task_is_an_item_failure(self)` — [`L229`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L229)
  - `test_evaluate_item_write_failure_keeps_sibling_and_aggregates(self)` — [`L187`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L187)
  - `test_overview_crash_keeps_sibling_rows(self)` — [`L111`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L111)
  - `test_overview_rejects_task_symlink_outside_batch_root(self)` — [`L128`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L128)
- uses (calls/refs, reference-scoped): [`evaluate_tasks`](../openmle_gym/local_evaluator.md#evaluate_tasks), [`ok`](../openmle_gym/process_runner.md#TaskProcessOutcome.ok), [`result`](../openmle_gym/process_runner.md#TaskProcessOutcome.result), [`generate_overview`](../openmle_gym/overview.md#generate_overview), [`atomic_write_json`](../openmle_gym/common.md#atomic_write_json), [`error`](../openmle_gym/process_runner.md#TaskProcessOutcome.error), [`TaskProcessOutcome`](../openmle_gym/process_runner.md#TaskProcessOutcome), [`returncode`](../openmle_gym/process_runner.md#TaskProcessOutcome.returncode), [`_run_all`](../openmle_gym/build.md#_run_all)  (2 test-only)

## Functions
- `_make_task(root: Path, name: str, metric_code: str)` — [`L23`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L23)

## Module values
- `GOOD_METRIC` — [`L43`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L43)
- `HAS_BATCH_DEPS` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_batch_independence.py#L17)

