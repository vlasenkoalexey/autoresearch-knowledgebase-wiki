---
title: 'Module: examples/circle_packing_with_artifacts/evaluator.py'
type: catalog
provenance: extracted
module: examples/circle_packing_with_artifacts/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.circle_packing_with_artifacts.evaluator`/
symbols:
  evaluate: evaluate().
  evaluate_stage1: evaluate_stage1().
  evaluate_stage2: evaluate_stage2().
  validate_packing: validate_packing().
  run_with_timeout: run_with_timeout().
  timeout_handler: timeout_handler().
---
# Module: [`examples/circle_packing_with_artifacts/evaluator.py`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py)

## Functions
- `evaluate(program_path)` — [`L192`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L192) — Evaluate the program by running it once and checking the sum of radii — documented in [openevolve-evaluation_result](../../../concepts/openevolve-evaluation_result.md)
- `evaluate_stage1(program_path)` — [`L375`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L375) — First stage evaluation - quick validation check — documented in [openevolve-evaluation_result](../../../concepts/openevolve-evaluation_result.md)
- `evaluate_stage2(program_path)` — [`L504`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L504) — Second stage evaluation - full evaluation
- `run_with_timeout(program_path, timeout_seconds=20)` — [`L82`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L82) — Run the program in a separate process with timeout
- `timeout_handler(signum, frame)` — [`L25`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L25) — Handle timeout signal
- `validate_packing(centers, radii)` — [`L30`](../../../../../../raw/code/openevolve/examples/circle_packing_with_artifacts/evaluator.py#L30) — Validate that circles don't overlap and are inside the unit square

