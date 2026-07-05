---
title: 'Module: examples/algotune/task_adapter.py'
type: catalog
provenance: extracted
module: examples/algotune/task_adapter.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.task_adapter`/AlgoTuneTaskAdapter#
symbols:
  AlgoTuneTaskAdapter.available_tasks: available_tasks.
  AlgoTuneTaskAdapter.task: task.
  AlgoTuneTaskAdapter._generate_initial_program: _generate_initial_program().
  AlgoTuneTaskAdapter.create_task_files: create_task_files().
  AlgoTuneTaskAdapter._generate_evaluator: _generate_evaluator().
  AlgoTuneTaskAdapter._generate_config: _generate_config().
  AlgoTuneTaskAdapter._generate_task_specific_method: _generate_task_specific_method().
  AlgoTuneTaskAdapter.algotune_path: algotune_path.
  AlgoTuneTaskAdapter.algotune_tasks_path: algotune_tasks_path.
  AlgoTuneTaskAdapter.get_task_description: get_task_description().
  AlgoTuneTaskAdapter.task_info: task_info.
  AlgoTuneTaskAdapter.get_task_info: get_task_info().
  AlgoTuneTaskAdapter.algotuner_path: algotuner_path.
  AlgoTuneTaskAdapter._extract_task_class_info: _extract_task_class_info().
  AlgoTuneTaskAdapter.list_available_tasks: list_available_tasks().
  AlgoTuneTaskAdapter: ''
  AlgoTuneTaskAdapter._setup_import_paths: _setup_import_paths().
  AlgoTuneTaskAdapter.task_name: task_name.
  AlgoTuneTaskAdapter.output_path: output_path.
  AlgoTuneTaskAdapter._load_tasks: _load_tasks().
  AlgoTuneTaskAdapter._harmonize_solve_and_is_solution: _harmonize_solve_and_is_solution().
  AlgoTuneTaskAdapter._clean_init_method: _clean_init_method().
  AlgoTuneTaskAdapter.replace_latex_command: replace_latex_command().
  AlgoTuneTaskAdapter._get_task_data_size: _get_task_data_size().
  AlgoTuneTaskAdapter._extract_problem_keys: _extract_problem_keys().
  AlgoTuneTaskAdapter._infer_return_type: _infer_return_type().
  AlgoTuneTaskAdapter._generate_generic_method: _generate_generic_method().
  AlgoTuneTaskAdapter.__init__: __init__().
---
# Module: [`examples/algotune/task_adapter.py`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py)

## Classes
### `AlgoTuneTaskAdapter`
- def: [`examples/algotune/task_adapter.py:19`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L19)
- doc: Adapter to convert AlgoTune tasks to OpenEvolve format.
- signature: `class AlgoTuneTaskAdapter:`
- members:
  - `__init__(self, algotune_path: Optional[str] = None, task: Optional[str] = None)` — [`L22`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L22) — Initialize the adapter.
  - `_clean_init_method(self, init_method: str)` — [`L331`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L331) — Clean up extracted __init__ method body by removing docstrings and super() calls.
  - `_extract_problem_keys(self, solve_method: str)` — [`L1321`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1321) — Extract the expected problem keys from the solve method.
  - `_extract_task_class_info(self, task_name: str)` — [`L103`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L103) — Extract class information from the task file with improved method extraction.
  - `_generate_config(self, task_name: str)` — [`L1144`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1144) — Generate the configuration for OpenEvolve with baseline comparison.
  - `_generate_evaluator(self, task_name: str)` — [`L552`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L552) — Generate the evaluator for OpenEvolve using the actual task implementation with baseline comparison.
  - `_generate_generic_method(self, task_name: str, problem_keys: List[str], return_type: str)` — [`L1354`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1354) — Generate a generic method based on problem structure and return type.
  - `_generate_initial_program(self, task_name: str)` — [`L373`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L373) — Generate the initial program for OpenEvolve based on the actual task implementation.
  - `_generate_task_specific_method(self, task_name: str, solve_method: str, class_info: Dict[str, Any])` — [`L1312`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1312) — Generate a generic fallback method when the actual solve method cannot be extracted.
  - `_get_task_data_size(self, task_name: str)` — [`L1302`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1302) — Get task-specific data_size values.
  - `_harmonize_solve_and_is_solution(self, solve_method: str, is_solution_method: str, task_name: str)` — [`L246`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L246) — Harmonize the formats between solve() and is_solution() methods.
  - `_infer_return_type(self, solve_method: str, task_name: str)` — [`L1342`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1342) — Infer the expected return type from the solve method.
  - `_load_tasks(self)` — [`L74`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L74) — Load all available AlgoTune tasks.
  - `_setup_import_paths(self)` — [`L56`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L56) — Setup Python import paths for AlgoTune modules.
  - `create_task_files(self, task_name: str, output_dir: Optional[str] = None)` — [`L1385`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1385) — Create OpenEvolve files for a specific task.
  - `get_task_description(self, task_name: str)` — [`L94`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L94) — Get the description of a task.
  - `get_task_info(self, task_name: str)` — [`L1428`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1428) — Get detailed information about a task.
  - `list_available_tasks(self)` — [`L1424`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1424) — List all available AlgoTune tasks.
  - `replace_latex_command(match)` — [`L1170`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L1170)
  - `algotune_path` — [`L33`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L33)
  - `algotune_tasks_path` — [`L34`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L34)
  - `algotuner_path` — [`L35`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L35)
  - `available_tasks` — [`L76`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L76)
  - `output_path` — [`L36`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L36)
  - `task` — [`L37`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L37)
  - `task_info` — [`L53`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L53)
  - `task_name` — [`L54`](../../../../../../raw/code/openevolve/examples/algotune/task_adapter.py#L54)
- used by: (2 test-only callers)

