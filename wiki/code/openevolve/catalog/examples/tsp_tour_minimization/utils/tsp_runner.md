---
title: 'Module: examples/tsp_tour_minimization/utils/tsp_runner.py'
type: catalog
provenance: extracted
module: examples/tsp_tour_minimization/utils/tsp_runner.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.tsp_tour_minimization.utils.tsp_runner`/
symbols:
  _run_one: _run_one().
  RunnerError: RunnerError#
  _decide_workers: _decide_workers().
  run_runner_parallel: run_runner_parallel().
  BASE_DIR: BASE_DIR.
  RunnerTimeout: RunnerTimeout#
  RunnerExitCodeError: RunnerExitCodeError#
  RunnerInternalError: RunnerInternalError#
  run_runner_parallel._driver: run_runner_parallel()._driver().
  run_runner_parallel._driver._one: run_runner_parallel()._driver()._one().
  _terminate_process: _terminate_process().
  _available_ram_gb: _available_ram_gb().
  _estimate_mem_gb_for_config: _estimate_mem_gb_for_config().
  compile_tsp_executable: compile_tsp_executable().
---
# Module: [`examples/tsp_tour_minimization/utils/tsp_runner.py`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py)

## Classes
### `RunnerError`  ·  implements/extends Exception
- def: [`examples/tsp_tour_minimization/utils/tsp_runner.py:21`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L21)
- doc: Base for runner errors
- signature: `class RunnerError(Exception):`
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (4 test-only callers)

### `RunnerExitCodeError`  ·  implements/extends RunnerError
- def: [`examples/tsp_tour_minimization/utils/tsp_runner.py:29`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L29)
- doc: Subprocess exited with non-zero code
- signature: `class RunnerExitCodeError(RunnerError):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `RunnerInternalError`  ·  implements/extends RunnerError
- def: [`examples/tsp_tour_minimization/utils/tsp_runner.py:33`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L33)
- doc: Unexpected internal failure while running subprocess
- signature: `class RunnerInternalError(RunnerError):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `RunnerTimeout`  ·  implements/extends RunnerError
- def: [`examples/tsp_tour_minimization/utils/tsp_runner.py:25`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L25)
- doc: Subprocess exceeded time limit
- signature: `class RunnerTimeout(RunnerError):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

## Functions
- `_available_ram_gb()` — [`L129`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L129)
- `_decide_workers(config_paths: list[str], max_workers: int | None = None, mem_per_proc_gb: float | None = None, alpha: float = 2, beta_gb: float = 0.5, safety_margin_gb: float = 2)` — [`L145`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L145)
- `_driver()` — [`L307`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L307)
- `_estimate_mem_gb_for_config(config_file_path: str, default_dtype_bytes: int = 4, alpha: float = 2, beta_gb: float = 0.5)` — [`L133`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L133)
- `_one(i: int)` — [`L313`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L313)
- `_run_one(index: int, runner_path: str, config_path: str, timeout: float | None, capture_stdout: bool, env_overrides: dict[str, str] | None)` — [`L193`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L193) — On success: (idx, returncode, elapsed, stdout_or_None, stderr)
- `_terminate_process(proc: asyncio.subprocess.Process)` — [`L172`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L172) — Kill process (and its group on POSIX) and await .wait()
- `compile_tsp_executable(dir_path: str, timeout: float = 120, cxx: str = "g++", extra_flags: tp.Optional[tp.Sequence[str]] = None)` — [`L37`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L37) — Compile TSP.cpp in `dir_path`, creating an executable `dir_path/bin/runner`
- `run_runner_parallel(runner_path: str, config_paths: tp.Sequence[str], timeout: float | None = None, max_workers: int | None = 12, mem_per_proc_gb: float | None = None, alpha: float = 2, beta_gb: float = 0.5, safety_margin_gb: float = 2, capture_index: int = 0, env_overrides: dict[str, str] | None = None)` — [`L280`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L280) — Run all configs in parallel

## Module values
- `BASE_DIR` — [`L14`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/tsp_runner.py#L14)

