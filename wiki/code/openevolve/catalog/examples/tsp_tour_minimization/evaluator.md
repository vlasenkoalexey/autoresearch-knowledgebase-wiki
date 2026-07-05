---
title: 'Module: examples/tsp_tour_minimization/evaluator.py'
type: catalog
provenance: extracted
module: examples/tsp_tour_minimization/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.tsp_tour_minimization.evaluator`/
symbols:
  evaluate: evaluate().
  build_artifacts_from_saver: build_artifacts_from_saver().
  BASE_DIR: BASE_DIR.
  PROJECT_TEMP_DIRECTORY: PROJECT_TEMP_DIRECTORY.
  SOLUTIONS_DIRECTORY: SOLUTIONS_DIRECTORY.
  HEAT_MAP_TRAIN_TIMEOUT: HEAT_MAP_TRAIN_TIMEOUT.
  HEAT_MAP_INFERENCE_TIMEOUT: HEAT_MAP_INFERENCE_TIMEOUT.
  TSP_RUN_TIMEOUT: TSP_RUN_TIMEOUT.
  calc_average_elapsed_time: calc_average_elapsed_time().
  N: N.
  INSTANCES_COUNT: INSTANCES_COUNT.
  TSP_COMPILATION_TIMEOUT: TSP_COMPILATION_TIMEOUT.
  calc_combined_score: calc_combined_score().
---
# Module: [`examples/tsp_tour_minimization/evaluator.py`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py)

## Functions
- `build_artifacts_from_saver(artifacts: dict, metrics: dict, output_saver: dict)` — [`L62`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L62)
- `calc_average_elapsed_time(time_elapsed: list[float | int | None])` — [`L40`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L40) — Calculate the average of non-None times
- `calc_combined_score(n: int, distances: np.ndarray, time_elapsed: tp.Sequence[float | int | None], h: float = 1, w: float = 1, *, alpha: float = 30, g_cut: float | None = 0.15, time_limit: float | None = 160, time_weight: float = 0.1, time_beta: float = 1)` — [`L89`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L89) — Distance-first combined score for TSP on [0, 1] x [0, 1] with n cities.
- `evaluate(program_path: str)` — [`L194`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L194) — Main stage evaluation with thorough testing on test dataset

## Module values
- `BASE_DIR` — [`L13`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L13)
- `HEAT_MAP_INFERENCE_TIMEOUT` — [`L35`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L35)
- `HEAT_MAP_TRAIN_TIMEOUT` — [`L34`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L34)
- `INSTANCES_COUNT` — [`L32`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L32)
- `N` — [`L31`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L31)
- `PROJECT_TEMP_DIRECTORY` — [`L29`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L29)
- `SOLUTIONS_DIRECTORY` — [`L30`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L30)
- `TSP_COMPILATION_TIMEOUT` — [`L36`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L36)
- `TSP_RUN_TIMEOUT` — [`L37`](../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/evaluator.py#L37)

