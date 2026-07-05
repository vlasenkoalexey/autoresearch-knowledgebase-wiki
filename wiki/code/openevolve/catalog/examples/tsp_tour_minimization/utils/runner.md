---
title: 'Module: examples/tsp_tour_minimization/utils/runner.py'
type: catalog
provenance: extracted
module: examples/tsp_tour_minimization/utils/runner.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.tsp_tour_minimization.utils.runner`/
symbols:
  run: run().
  BASE_DIR: BASE_DIR.
  format_input_file: format_input_file().
  change_config_file: change_config_file().
  parse_output_files: parse_output_files().
---
# Module: [`examples/tsp_tour_minimization/utils/runner.py`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py)

## Functions
- `change_config_file(input_config_file_path: str, output_config_file_path: str, cities_number: int, input_path: str, output_path: str)` — [`L21`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py#L21)
- `format_input_file(input_file_path: str, cities: np.ndarray, heat_map: np.ndarray)` — [`L14`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py#L14)
- `parse_output_files(output_files_paths: list[str])` — [`L32`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py#L32)
- `run(dir_path: str, cities: np.ndarray, heat_map_train_timeout: float = 360, heat_map_inference_timeout: float = 60, tsp_compilation_timeout: float = 10, tsp_run_timeout: float = 60, verbose: bool = False, output_saver: dict | None = None)` — [`L42`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py#L42)

## Module values
- `BASE_DIR` — [`L5`](../../../../../../../raw/code/openevolve/examples/tsp_tour_minimization/utils/runner.py#L5)

