---
title: 'Module: examples/algotune/lu_factorization/initial_program.py'
type: catalog
provenance: extracted
module: examples/algotune/lu_factorization/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.lu_factorization.initial_program`/
symbols:
  run_solver: run_solver().
  LUFactorization: LUFactorization#
  LUFactorization.solve: LUFactorization#solve().
  LUFactorization.__init__: LUFactorization#__init__().
  LUFactorization.is_solution: LUFactorization#is_solution().
---
# Module: [`examples/algotune/lu_factorization/initial_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py)

## Classes
### `LUFactorization`
- def: [`examples/algotune/lu_factorization/initial_program.py:63`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py#L63)
- doc: Initial implementation of lu_factorization task.
- signature: `class LUFactorization:`
- members:
  - `__init__(self)` — [`L69`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py#L69) — Initialize the LUFactorization.
  - `is_solution(self, problem, solution)` — [`L104`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py#L104) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L73`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py#L73) — Solve the lu_factorization problem.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L209`](../../../../../../../raw/code/openevolve/examples/algotune/lu_factorization/initial_program.py#L209) — Main function to run the solver.

