---
title: 'Module: examples/k_module_problem/evaluator.py'
type: catalog
provenance: extracted
module: examples/k_module_problem/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.k_module_problem.evaluator`/
symbols:
  NUM_MODULES: NUM_MODULES.
  evaluate: evaluate().
  initial_program: initial_program.
  VALID_OPTIONS: VALID_OPTIONS.
  result: result.
  build_artifacts: build_artifacts().
  validate_config: validate_config().
  CORRECT_CONFIG: CORRECT_CONFIG.
  score_config: score_config().
  _error_result: _error_result().
  _validation_error_result: _validation_error_result().
  _exception_result: _exception_result().
  RICH_FEEDBACK: RICH_FEEDBACK.
  script_dir: script_dir.
---
# Module: [`examples/k_module_problem/evaluator.py`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py)

## Functions
- `_error_result(message: str)` — [`L209`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L209) — Return an error result.
- `_exception_result(e: Exception)` — [`L242`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L242) — Return an exception result.
- `_validation_error_result(errors: list)` — [`L225`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L225) — Return a validation error result.
- `build_artifacts(config: dict, correct_count: int, module_results: dict, eval_time: float)` — [`L150`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L150) — Build artifacts that provide useful feedback.
- `evaluate(program_path: str)` — [`L48`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L48) — Evaluate a pipeline configuration program.
- `score_config(config: dict)` — [`L131`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L131) — Score the configuration against the target.
- `validate_config(config: dict)` — [`L110`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L110) — Validate that the configuration has valid values.

## Module values
- `CORRECT_CONFIG` — [`L30`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L30)
- `NUM_MODULES` — [`L45`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L45)
- `RICH_FEEDBACK` — [`L25`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L25)
- `VALID_OPTIONS` — [`L38`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L38)
- `initial_program` — [`L269`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L269)
- `result` — [`L262`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L262)
- `script_dir` — [`L268`](../../../../../../raw/code/openevolve/examples/k_module_problem/evaluator.py#L268)

