---
title: 'Module: examples/sldbench/evaluator.py'
type: catalog
provenance: extracted
module: examples/sldbench/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.sldbench.evaluator`/
symbols:
  r2_d: r2_d.
  final_results: final_results.
  evaluate_core: evaluate_core().
  get_failure_result: get_failure_result().
  param_str: param_str.
  args: args.
  evaluate: evaluate().
  params: params.
  param_val: param_val.
  task_name: task_name.
  parser: parser.
  calculate_final_metrics: calculate_final_metrics().
  resolve_task_name: resolve_task_name().
  nmse_vals: nmse_vals.
  nmae_vals: nmae_vals.
  r2_vals: r2_vals.
  val: val.
  SUPPORTED_TASKS: SUPPORTED_TASKS.
  run_with_timeout: run_with_timeout().
  _import_program: _import_program().
  i: i.
  nmse_d: nmse_d.
  nmae_d: nmae_d.
  key: key.
---
# Module: [`examples/sldbench/evaluator.py`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py)

## Functions
- `_import_program(program_path: str)` — [`L138`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L138) — Imports a Python module from a given file path.
- `calculate_final_metrics(predictions: np.ndarray, true_values: np.ndarray)` — [`L54`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L54) — Calculates evaluation metrics, correctly handling multi-dimensional outputs.
- `evaluate(program_path: str, verbose: bool = False)` — [`L229`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L229) — High-level, single-call evaluation function.
- `evaluate_core(program_path: str, task_name: str, use_test_data: bool = False, fitted_params_map: Dict[Any, Any] = None)` — [`L168`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L168) — Core evaluation logic: fits a model or evaluates it on test data.
- `get_failure_result(error_msg: str = "Evaluation failed or timed out.")` — [`L34`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L34) — Returns a standardized dictionary for failure cases.
- `resolve_task_name(program_path: str)` — [`L147`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L147) — Infers the task name from environment variables or the file path.
- `run_with_timeout(func, args=(), kwargs={}, timeout_seconds: int = 600)` — [`L44`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L44) — Runs a function with a specified timeout, raising an exception on timeout.

## Module values
- `SUPPORTED_TASKS` — [`L21`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L21)
- `args` — [`L278`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L278)
- `final_results` — [`L285`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L285)
- `i` — [`L307`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L307)
- `key` — [`L313`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L313)
- `nmae_d` — [`L307`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L307)
- `nmae_vals` — [`L305`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L305)
- `nmse_d` — [`L307`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L307)
- `nmse_vals` — [`L304`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L304)
- `param_str` — [`L316`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L316)
- `param_val` — [`L314`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L314)
- `params` — [`L310`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L310)
- `parser` — [`L276`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L276)
- `r2_d` — [`L307`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L307)
- `r2_vals` — [`L306`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L306)
- `task_name` — [`L287`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L287)
- `val` — [`L313`](../../../../../../raw/code/openevolve/examples/sldbench/evaluator.py#L313)

