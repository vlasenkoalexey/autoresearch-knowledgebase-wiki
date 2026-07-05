---
title: 'Module: examples/tsp_tour_minimization/utils/utils.py'
type: catalog
provenance: extracted
module: examples/tsp_tour_minimization/utils/utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.tsp_tour_minimization.utils.utils`/
symbols:
  approximation_using_BHH_constant: approximation_using_BHH_constant().
  calc_total_cycle_distance: calc_total_cycle_distance().
  check_on_hamiltonian_cycle: check_on_hamiltonian_cycle().
  BHH_CONSTANT_2D: BHH_CONSTANT_2D.
  get_cpu_cores_number: get_cpu_cores_number().
  default_for_none: default_for_none().
  create_dir: create_dir().
  remove_dir: remove_dir().
  touch_file: touch_file().
  read_file: read_file().
  is_file_exist: is_file_exist().
  expected_random_cycle_length: expected_random_cycle_length().
  run_with_timeout: run_with_timeout().
---
# Module: [`examples/tsp_tour_minimization/utils/utils.py`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py)

## Functions
- `approximation_using_BHH_constant(n: int, h: float = 1, w: float = 1)` — [`L72`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L72)
- `calc_total_cycle_distance(cities: np.ndarray, solutions: list[np.ndarray] | np.ndarray)` — [`L138`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L138) — Compute total cycle distances for a batch of instances
- `check_on_hamiltonian_cycle(cities: np.ndarray, solution: np.ndarray)` — [`L98`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L98) — Return True if:
- `create_dir(dir_path: str)` — [`L24`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L24)
- `default_for_none(value: tp.Any, default: tp.Any)` — [`L19`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L19)
- `expected_random_cycle_length(n: int, h: float = 1, w: float = 1)` — [`L55`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L55)
- `get_cpu_cores_number()` — [`L15`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L15)
- `is_file_exist(file_path: str)` — [`L51`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L51)
- `read_file(file_path: str)` — [`L46`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L46)
- `remove_dir(dir_path: str)` — [`L28`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L28)
- `run_with_timeout(func: tp.Callable, args=(), kwargs={}, timeout: float = 5)` — [`L76`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L76) — Run a function with a timeout using concurrent.futures
- `touch_file(file_path: str)` — [`L40`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L40)

## Module values
- `BHH_CONSTANT_2D` — [`L12`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/utils.py#L12)

