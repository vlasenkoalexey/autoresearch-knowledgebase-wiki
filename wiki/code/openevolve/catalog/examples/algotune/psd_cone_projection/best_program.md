---
title: 'Module: examples/algotune/psd_cone_projection/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/psd_cone_projection/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.psd_cone_projection.best_program`/
symbols:
  run_solver: run_solver().
  PSDConeProjection.is_solution: PSDConeProjection#is_solution().
  PSDConeProjection.solve: PSDConeProjection#solve().
  PSDConeProjection: PSDConeProjection#
  PSDConeProjection.__init__: PSDConeProjection#__init__().
---
# Module: [`examples/algotune/psd_cone_projection/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py)

## Classes
### `PSDConeProjection`
- def: [`examples/algotune/psd_cone_projection/best_program.py:72`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py#L72)
- doc: Initial implementation of psd_cone_projection task.
- signature: `class PSDConeProjection:`
- members:
  - `__init__(self)` — [`L78`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py#L78) — Initialize the PSDConeProjection.
  - `is_solution(self, problem, solution)` — [`L112`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py#L112) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L82`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py#L82) — Solve the psd_cone_projection problem.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L178`](../../../../../../../raw/code/openevolve/examples/algotune/psd_cone_projection/best_program.py#L178) — Main function to run the solver.

