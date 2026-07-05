---
title: 'Module: examples/algotune/convolve2d_full_fill/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/convolve2d_full_fill/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.convolve2d_full_fill.best_program`/
symbols:
  Convolve2DFullFill.is_solution: Convolve2DFullFill#is_solution().
  run_solver: run_solver().
  Convolve2DFullFill.solve: Convolve2DFullFill#solve().
  Convolve2DFullFill.mode: Convolve2DFullFill#mode.
  Convolve2DFullFill: Convolve2DFullFill#
  Convolve2DFullFill.boundary: Convolve2DFullFill#boundary.
  Convolve2DFullFill.__init__: Convolve2DFullFill#__init__().
---
# Module: [`examples/algotune/convolve2d_full_fill/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py)

## Classes
### `Convolve2DFullFill`
- def: [`examples/algotune/convolve2d_full_fill/best_program.py:59`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L59)
- doc: Initial implementation of convolve2d_full_fill task.
- signature: `class Convolve2DFullFill:`
- members:
  - `__init__(self)` — [`L65`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L65) — Initialize the Convolve2DFullFill.
  - `is_solution(self, problem, solution)` — [`L100`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L100) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L72`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L72) — Compute the 2D convolution of arrays a and b using "full" mode and "fill" boundary.
  - `boundary` — [`L70`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L70)
  - `mode` — [`L67`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L67)
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L129`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/best_program.py#L129) — Main function to run the solver.

