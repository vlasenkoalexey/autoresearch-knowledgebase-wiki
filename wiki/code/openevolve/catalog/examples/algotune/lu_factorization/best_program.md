---
title: 'Module: examples/algotune/lu_factorization/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/lu_factorization/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.lu_factorization.best_program`/
symbols:
  run_solver: run_solver().
  LUFactorization: LUFactorization#
  LUFactorization.solve: LUFactorization#solve().
  LUFactorization.__init__: LUFactorization#__init__().
  LUFactorization.is_solution: LUFactorization#is_solution().
---
# Module: [`examples/algotune/lu_factorization/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py)

## Classes
### `LUFactorization`
- def: [`examples/algotune/lu_factorization/best_program.py:63`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py#L63)
- doc: Initial implementation of lu_factorization task.
- signature: `class LUFactorization:`
- members:
  - `__init__(self)` — [`L69`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py#L69) — Initialize the LUFactorization.
  - `is_solution(self, problem, solution)` — [`L89`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py#L89) — Validate an LU factorization A = P L U.
  - `solve(self, problem)` — [`L73`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py#L73) — Computes the LU factorization of a matrix using an optimized scipy call.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L184`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/best_program.py#L184) — Main function to run the solver.

