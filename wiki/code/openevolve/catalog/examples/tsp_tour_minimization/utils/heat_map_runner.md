---
title: 'Module: examples/tsp_tour_minimization/utils/heat_map_runner.py'
type: catalog
provenance: extracted
module: examples/tsp_tour_minimization/utils/heat_map_runner.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.tsp_tour_minimization.utils.heat_map_runner`/
symbols:
  _run_one_inference: _run_one_inference().
  run_heat_maps_parallel._runner: run_heat_maps_parallel()._runner().
  run_heat_maps_parallel._runner._guarded: run_heat_maps_parallel()._runner()._guarded().
  BASE_DIR: BASE_DIR.
  run_python_heat_map_train: run_python_heat_map_train().
  run_heat_maps_parallel: run_heat_maps_parallel().
  THREAD_ENV: THREAD_ENV.
  format_heat_map_stdin: format_heat_map_stdin().
  _default_workers: _default_workers().
  parse_heat_map_stdout: parse_heat_map_stdout().
---
# Module: [`examples/tsp_tour_minimization/utils/heat_map_runner.py`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py)

## Functions
- `_default_workers(n: tp.Optional[int])` — [`L101`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L101)
- `_guarded(i: int)` — [`L237`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L237)
- `_run_one_inference(index: int, program_path: str, python_executable: str, cities_i: np.ndarray, out_path: str, timeout: float)` — [`L109`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L109) — Launch one child, send coordinates via stdin, child writes .npy to out_path
- `_runner()` — [`L231`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L231)
- `format_heat_map_stdin(cities: np.ndarray)` — [`L88`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L88)
- `parse_heat_map_stdout(stdout: str, n: int)` — [`L92`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L92)
- `run_heat_maps_parallel(program_path: str, cities: np.ndarray, out_dir: str, timeout: float, max_workers: tp.Optional[int] = None, capture_index: int = 0, python_executable: str = sys.executable)` — [`L209`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L209) — Runs batch_size instances in parallel (max_workers concurrently)
- `run_python_heat_map_train(program_path: str, timeout: float, python_executable: str = sys.executable)` — [`L30`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L30) — Runs python program as a subprocess, returns stdout/stderr + elapsed time

## Module values
- `BASE_DIR` — [`L12`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L12)
- `THREAD_ENV` — [`L23`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/heat_map_runner.py#L23)

