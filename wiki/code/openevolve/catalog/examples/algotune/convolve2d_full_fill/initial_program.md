---
title: 'Module: examples/algotune/convolve2d_full_fill/initial_program.py'
type: catalog
provenance: extracted
module: examples/algotune/convolve2d_full_fill/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.convolve2d_full_fill.initial_program`/
symbols:
  Convolve2DFullFill.solve: Convolve2DFullFill#solve().
  Convolve2DFullFill.is_solution: Convolve2DFullFill#is_solution().
  run_solver: run_solver().
  Convolve2DFullFill.mode: Convolve2DFullFill#mode.
  Convolve2DFullFill.boundary: Convolve2DFullFill#boundary.
  Convolve2DFullFill: Convolve2DFullFill#
  Convolve2DFullFill.__init__: Convolve2DFullFill#__init__().
---
# Module: [`examples/algotune/convolve2d_full_fill/initial_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py)

## Classes
### `Convolve2DFullFill`
- def: [`examples/algotune/convolve2d_full_fill/initial_program.py:59`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L59)
- doc: Initial implementation of convolve2d_full_fill task.
- signature: `class Convolve2DFullFill:`
- members:
  - `__init__(self)` — [`L65`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L65) — Initialize the Convolve2DFullFill.
  - `is_solution(self, problem, solution)` — [`L95`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L95) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L70`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L70) — Solve the convolve2d_full_fill problem.
  - `boundary` — [`L68`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L68)
  - `mode` — [`L67`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L67)
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L130`](../../../../../../../raw/code/openevolve/examples/algotune/convolve2d_full_fill/initial_program.py#L130) — Main function to run the solver.

