---
title: 'Module: examples/algotune/polynomial_real/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/polynomial_real/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.polynomial_real.best_program`/
symbols:
  run_solver: run_solver().
  PolynomialReal.solve: PolynomialReal#solve().
  _solve_roots_jax: _solve_roots_jax().
  PolynomialReal: PolynomialReal#
  PolynomialReal.__init__: PolynomialReal#__init__().
  PolynomialReal.is_solution: PolynomialReal#is_solution().
---
# Module: [`examples/algotune/polynomial_real/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py)

## Classes
### `PolynomialReal`
- def: [`examples/algotune/polynomial_real/best_program.py:64`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L64)
- doc: Initial implementation of polynomial_real task.
- signature: `class PolynomialReal:`
- members:
  - `__init__(self)` — [`L70`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L70) — Initialize the PolynomialReal.
  - `is_solution(self, problem, solution)` — [`L115`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L115) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L74`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L74) — Solve the polynomial_real problem using a JIT-compiled JAX function.
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_solve_roots_jax(coefficients)` — [`L50`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L50) — JIT-compiled function to find polynomial roots using JAX.
- `run_solver(problem)` — [`L155`](../../../../../../../raw/code/openevolve/examples/algotune/polynomial_real/best_program.py#L155) — Main function to run the solver.

