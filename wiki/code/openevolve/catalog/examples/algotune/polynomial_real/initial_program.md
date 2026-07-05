---
title: 'Module: examples/algotune/polynomial_real/initial_program.py'
type: catalog
provenance: extracted
module: examples/algotune/polynomial_real/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.polynomial_real.initial_program`/
symbols:
  run_solver: run_solver().
  PolynomialReal: PolynomialReal#
  PolynomialReal.solve: PolynomialReal#solve().
  PolynomialReal.__init__: PolynomialReal#__init__().
  PolynomialReal.is_solution: PolynomialReal#is_solution().
---
# Module: [`examples/algotune/polynomial_real/initial_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py)

## Classes
### `PolynomialReal`
- def: [`examples/algotune/polynomial_real/initial_program.py:47`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py#L47)
- doc: Initial implementation of polynomial_real task.
- signature: `class PolynomialReal:`
- members:
  - `__init__(self)` — [`L53`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py#L53) — Initialize the PolynomialReal.
  - `is_solution(self, problem, solution)` — [`L94`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py#L94) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L57`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py#L57) — Solve the polynomial_real problem.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L135`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/initial_program.py#L135) — Main function to run the solver.

