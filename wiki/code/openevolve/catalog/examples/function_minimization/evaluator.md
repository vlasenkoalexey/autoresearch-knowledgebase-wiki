---
title: 'Module: examples/function_minimization/evaluator.py'
type: catalog
provenance: extracted
module: examples/function_minimization/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.function_minimization.evaluator`/
symbols:
  evaluate: evaluate().
  evaluate_stage1: evaluate_stage1().
  safe_float: safe_float().
  evaluate_stage2: evaluate_stage2().
  run_with_timeout: run_with_timeout().
---
# Module: [`examples/function_minimization/evaluator.py`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py)

## Functions
- `evaluate(program_path)` — [`L45`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py#L45) — Evaluate the program by running it multiple times and checking how close — documented in [openevolve-evaluation_result](../../../concepts/openevolve-evaluation_result.md)
- `evaluate_stage1(program_path)` — [`L259`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py#L259) — First stage evaluation with fewer trials — documented in [openevolve-evaluation_result](../../../concepts/openevolve-evaluation_result.md)
- `evaluate_stage2(program_path)` — [`L490`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py#L490) — Second stage evaluation with more thorough testing
- `run_with_timeout(func, args=(), kwargs={}, timeout_seconds=5)` — [`L14`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py#L14) — Run a function with a timeout using concurrent.futures
- `safe_float(value)` — [`L36`](../../../../../../raw/code/openevolve/examples/function_minimization/evaluator.py#L36) — Convert a value to float safely

