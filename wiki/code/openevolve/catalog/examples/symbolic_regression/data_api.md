---
title: 'Module: examples/symbolic_regression/data_api.py'
type: catalog
provenance: extracted
module: examples/symbolic_regression/data_api.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.symbolic_regression.data_api`/
symbols:
  process_problem: process_problem().
  main: main().
  create_config: create_config().
  load_secret: load_secret().
  extract_problem_data_from_initialized_dataset: extract_problem_data_from_initialized_dataset().
  create_program: create_program().
  create_evaluator: create_evaluator().
  create_config.PreserveNewlinesDumper: create_config().PreserveNewlinesDumper#
  create_config.PreserveNewlinesDumper.represent_scalar: create_config().PreserveNewlinesDumper#represent_scalar().
---
# Module: [`examples/symbolic_regression/data_api.py`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py)

## Classes
### `PreserveNewlinesDumper`  ·  implements/extends SafeDumper
- def: [`examples/symbolic_regression/data_api.py:616`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L616)
- doc: Custom YAML dumper that preserves multi-line strings.
- signature: `class PreserveNewlinesDumper(yaml.SafeDumper):`
- members:
  - `represent_scalar(self, tag, value, style=None)` — [`L619`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L619)
- used by: (1 test-only callers)

## Functions
- `create_config(problem: Dict[str, Any])` — [`L521`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L521) — Create a YAML configuration file for the symbolic regression task.
- `create_evaluator(problem: Dict[str, Any])` — [`L185`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L185) — Create an evaluator script for the symbolic regression problem.
- `create_program(problem: Dict[str, Any])` — [`L70`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L70) — Create a Python script with a naive linear model for symbolic regression.
- `extract_problem_data_from_initialized_dataset(initialized_dataset, problem_id: int)` — [`L39`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L39) — Extract data for a specific problem from an initialized dataset.
- `load_secret(secrets_file: str = "secrets.yaml")` — [`L18`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L18) — Load API keys and configuration from a secrets file.
- `main()` — [`L701`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L701) — Main entry point for processing symbolic regression problems.
- `process_problem(initialized_dataset, problem_id: int, split_name: str)` — [`L637`](../../../../../../raw/code/openevolve/examples/symbolic_regression/data_api.py#L637) — Process a single problem using a pre-initialized dataset.

