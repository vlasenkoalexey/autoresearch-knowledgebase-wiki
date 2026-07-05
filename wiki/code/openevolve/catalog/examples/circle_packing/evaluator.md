---
title: 'Module: examples/circle_packing/evaluator.py'
type: catalog
provenance: extracted
module: examples/circle_packing/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.circle_packing.evaluator`/
symbols:
  evaluate: evaluate().
  evaluate_stage1: evaluate_stage1().
  evaluate_stage2: evaluate_stage2().
  validate_packing: validate_packing().
  run_with_timeout: run_with_timeout().
  timeout_handler: timeout_handler().
---
# Module: [`examples/circle_packing/evaluator.py`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py)

## Functions
- `evaluate(program_path)` — [`L186`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L186) — Evaluate the program by running it once and checking the sum of radii
- `evaluate_stage1(program_path)` — [`L281`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L281) — First stage evaluation - quick validation check
- `evaluate_stage2(program_path)` — [`L335`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L335) — Second stage evaluation - full evaluation
- `run_with_timeout(program_path, timeout_seconds=20)` — [`L76`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L76) — Run the program in a separate process with timeout
- `timeout_handler(signum, frame)` — [`L21`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L21) — Handle timeout signal
- `validate_packing(centers, radii)` — [`L26`](../../../../../../raw/code/openevolve/examples/circle_packing/evaluator.py#L26) — Validate that circles don't overlap and are inside the unit square

