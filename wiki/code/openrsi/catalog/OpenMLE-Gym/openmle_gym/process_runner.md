---
title: 'Module: OpenMLE-Gym/openmle_gym/process_runner.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/process_runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.process_runner`/
symbols:
  run_task_process: run_task_process().
  TaskProcessOutcome.ok: TaskProcessOutcome#ok.
  TaskProcessOutcome.result: TaskProcessOutcome#result.
  TaskProcessOutcome.error: TaskProcessOutcome#error.
  TaskProcessOutcome.stdout: TaskProcessOutcome#stdout.
  TaskProcessOutcome.stderr: TaskProcessOutcome#stderr.
  TaskProcessOutcome: TaskProcessOutcome#
  TaskProcessOutcome.returncode: TaskProcessOutcome#returncode.
  _container_command: _container_command().
  _load_result_envelope: _load_result_envelope().
  _container_command.mount: _container_command().mount().
  FORWARDED_ENV: FORWARDED_ENV.
  _terminate_process_group: _terminate_process_group().
---
# Module: [`OpenMLE-Gym/openmle_gym/process_runner.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py)

## Classes
### `TaskProcessOutcome`
- def: [`OpenMLE-Gym/openmle_gym/process_runner.py:37`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L37) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- signature: `class TaskProcessOutcome:`
- members:
  - `error` — [`L40`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L40) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `ok` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L38) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `result` — [`L39`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L39) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `returncode` — [`L43`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L43) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `stderr` — [`L42`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L42) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `stdout` — [`L41`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L41) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- used by: [`run_task_process`](process_runner.md#run_task_process), [`prepare_single_competition`](../builder_core/utils/nodes.md#NodeExecutor.prepare_single_competition), [`evaluate_sample_submission_process`](metric_validation.md#evaluate_sample_submission_process), [`evaluate_one`](local_evaluator.md#evaluate_tasks.evaluate_one), [`run_one_impl`](overview.md#generate_overview.run_one_impl), [`worker`](build.md#_run_all.worker), [`analyze_in_process`](overview.md#_run_metadata_pipeline.analyze_in_process)  (6 test-only)

## Functions
- `_container_command(request_path: Path, result_path: Path, operation: str, readonly_paths: Iterable[Path], writable_paths: Iterable[Path])` — [`L71`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L71) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
- `_load_result_envelope(path: Path)` — [`L46`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L46) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `_terminate_process_group(process: subprocess.Popen[str])` — [`L55`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L55) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `mount(path: Path, mode: str)` — [`L113`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L113) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `run_task_process(operation: str, payload: dict[str, Any], *, timeout: float, execution_mode: str = "process", readonly_paths: Iterable[str | Path] = (), writable_paths: Iterable[str | Path] = ())` — [`L146`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L146) — Run one task in a disposable process and return a non-throwing outcome. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)

## Module values
- `FORWARDED_ENV` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/process_runner.py#L16) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)

