---
title: 'Module: OpenMLE-Gym/tests/test_process_isolation.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/tests/test_process_isolation.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.tests.test_process_isolation`/
symbols:
  ProcessIsolationTests.test_crashed_task_does_not_break_sibling_tasks: ProcessIsolationTests#test_crashed_task_does_not_break_sibling_tasks().
  ProcessIsolationTests.test_isolated_mode_never_falls_back: ProcessIsolationTests#test_isolated_mode_never_falls_back().
  ProcessIsolationTests.test_timeout_is_local_to_one_task: ProcessIsolationTests#test_timeout_is_local_to_one_task().
  ProcessIsolationTests.test_same_dynamic_module_name_is_isolated_between_tasks: ProcessIsolationTests#test_same_dynamic_module_name_is_isolated_between_tasks().
  _make_task: _make_task().
  GOOD_METRIC: GOOD_METRIC.
  ProcessIsolationTests.test_prepare_operation_uses_its_own_result_envelope: ProcessIsolationTests#test_prepare_operation_uses_its_own_result_envelope().
  ProcessIsolationTests.run: ProcessIsolationTests#run().
  ProcessIsolationTests.test_invalid_result_json_is_rejected: ProcessIsolationTests#test_invalid_result_json_is_rejected().
  ProcessIsolationTests.test_isolated_command_has_no_network_or_source_mount: ProcessIsolationTests#test_isolated_command_has_no_network_or_source_mount().
  HAS_PANDAS: HAS_PANDAS.
  ProcessIsolationTests: ProcessIsolationTests#
---
# Module: [`OpenMLE-Gym/tests/test_process_isolation.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py)

## Classes
### `ProcessIsolationTests`  ·  implements/extends TestCase
- def: [`OpenMLE-Gym/tests/test_process_isolation.py:46`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L46)
- signature: `class ProcessIsolationTests(unittest.TestCase):`
- members:
  - `run(task: Path)` — [`L65`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L65) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
  - `test_crashed_task_does_not_break_sibling_tasks(self)` — [`L54`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L54) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
  - `test_invalid_result_json_is_rejected(self)` — [`L47`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L47)
  - `test_isolated_command_has_no_network_or_source_mount(self)` — [`L147`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L147)
  - `test_isolated_mode_never_falls_back(self)` — [`L129`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L129) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
  - `test_prepare_operation_uses_its_own_result_envelope(self)` — [`L189`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L189) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
  - `test_same_dynamic_module_name_is_isolated_between_tasks(self)` — [`L83`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L83) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
  - `test_timeout_is_local_to_one_task(self)` — [`L108`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L108) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- uses (calls/refs, reference-scoped): [`run_task_process`](../openmle_gym/process_runner.md#run_task_process), [`ok`](../openmle_gym/process_runner.md#TaskProcessOutcome.ok), [`result`](../openmle_gym/process_runner.md#TaskProcessOutcome.result), [`error`](../openmle_gym/process_runner.md#TaskProcessOutcome.error), [`returncode`](../openmle_gym/process_runner.md#TaskProcessOutcome.returncode), [`_container_command`](../openmle_gym/process_runner.md#_container_command), [`_load_result_envelope`](../openmle_gym/process_runner.md#_load_result_envelope)  (2 test-only)

## Functions
- `_make_task(root: Path, name: str, metric_code: str)` — [`L21`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L21)

## Module values
- `GOOD_METRIC` — [`L35`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L35)
- `HAS_PANDAS` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Gym/tests/test_process_isolation.py#L18)

