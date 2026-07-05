---
title: 'Module: examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.erdos_min_overlap.initial_program`/
symbols:
  ErdosOptimizer.run_optimization: ErdosOptimizer#run_optimization().
  ErdosOptimizer._objective_fn: ErdosOptimizer#_objective_fn().
  ErdosOptimizer.dx: ErdosOptimizer#dx.
  run: run().
  ErdosOptimizer.hypers: ErdosOptimizer#hypers.
  Hyperparameters.num_intervals: Hyperparameters#num_intervals.
  ErdosOptimizer.train_step: ErdosOptimizer#train_step().
  ErdosOptimizer.__init__: ErdosOptimizer#__init__().
  Hyperparameters: Hyperparameters#
  Hyperparameters.learning_rate: Hyperparameters#learning_rate.
  Hyperparameters.num_steps: Hyperparameters#num_steps.
  Hyperparameters.penalty_strength: Hyperparameters#penalty_strength.
  ErdosOptimizer: ErdosOptimizer#
  ErdosOptimizer.domain_width: ErdosOptimizer#domain_width.
---
# Module: [`examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py)

## Classes
### `ErdosOptimizer`
- def: [`examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py:18`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L18)
- doc: Finds a step function h that minimizes the maximum overlap integral.
- signature: `class ErdosOptimizer:`
- members:
  - `_objective_fn(self, latent_h_values: jnp.ndarray)` — [`L28`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L28) — The loss function includes the objective and a penalty for the constraint.
  - `run_optimization(self)` — [`L53`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L53)
  - `train_step(latent_h_values, opt_state)` — [`L62`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L62)
  - `domain_width` — [`L25`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L25)
  - `dx` — [`L26`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L26)
  - `hypers` — [`L24`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L24)
- protocol/private: `__init__`[`L23`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L23)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py:11`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L11)
- signature: `class Hyperparameters:`
- members:
  - `learning_rate` — [`L13`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L13)
  - `num_intervals` — [`L12`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L12)
  - `num_steps` — [`L14`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L14)
  - `penalty_strength` — [`L15`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L15)
- used by: (5 test-only callers)

## Functions
- `run()` — [`L88`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/erdos_min_overlap/initial_program.py#L88)

