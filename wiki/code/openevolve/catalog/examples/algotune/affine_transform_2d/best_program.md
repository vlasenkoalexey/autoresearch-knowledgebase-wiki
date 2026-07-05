---
title: 'Module: examples/algotune/affine_transform_2d/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/affine_transform_2d/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.affine_transform_2d.best_program`/
symbols:
  AffineTransform2D.solve: AffineTransform2D#solve().
  AffineTransform2D.is_solution: AffineTransform2D#is_solution().
  run_solver: run_solver().
  AffineTransform2D.order: AffineTransform2D#order.
  AffineTransform2D.mode: AffineTransform2D#mode.
  AffineTransform2D: AffineTransform2D#
  AffineTransform2D.__init__: AffineTransform2D#__init__().
---
# Module: [`examples/algotune/affine_transform_2d/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py)

## Classes
### `AffineTransform2D`
- def: [`examples/algotune/affine_transform_2d/best_program.py:61`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L61)
- doc: Initial implementation of affine_transform_2d task.
- signature: `class AffineTransform2D:`
- members:
  - `__init__(self)` — [`L67`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L67) — Initialize the AffineTransform2D.
  - `is_solution(self, problem, solution)` — [`L113`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L113) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L72`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L72) — Solve the affine_transform_2d problem.
  - `mode` — [`L70`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L70)
  - `order` — [`L69`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L69)
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L229`](../../../../../../../raw/code/openevolve/examples/algotune/affine_transform_2d/best_program.py#L229) — Main function to run the solver.

