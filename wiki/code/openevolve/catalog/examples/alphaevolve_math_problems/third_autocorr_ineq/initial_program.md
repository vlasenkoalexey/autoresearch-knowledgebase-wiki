---
title: 'Module: examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.third_autocorr_ineq.initial_program`/
symbols:
  C3Optimizer.optimizer: C3Optimizer#optimizer.
  C3Optimizer.hypers: C3Optimizer#hypers.
  C3Optimizer.run_optimization: C3Optimizer#run_optimization().
  run: run().
  C3Optimizer.dx: C3Optimizer#dx.
  C3Optimizer._objective_fn: C3Optimizer#_objective_fn().
  C3Optimizer.train_step: C3Optimizer#train_step().
  Hyperparameters.num_intervals: Hyperparameters#num_intervals.
  Hyperparameters.num_steps: Hyperparameters#num_steps.
  C3Optimizer.__init__: C3Optimizer#__init__().
  Hyperparameters: Hyperparameters#
  Hyperparameters.learning_rate: Hyperparameters#learning_rate.
  Hyperparameters.warmup_steps: Hyperparameters#warmup_steps.
  C3Optimizer: C3Optimizer#
  C3Optimizer.domain_width: C3Optimizer#domain_width.
---
# Module: [`examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py)

## Classes
### `C3Optimizer`
- def: [`examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py:19`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L19)
- doc: Optimizes a function f (with positive and negative values) to find an
- signature: `class C3Optimizer:`
- members:
  - `_objective_fn(self, f_values: jnp.ndarray)` — [`L30`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L30) — Computes the C3 ratio. The goal is to minimize this value.
  - `run_optimization(self)` — [`L64`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L64) — Sets up and runs the full optimization process.
  - `train_step(self, f_values: jnp.ndarray, opt_state: optax.OptState)` — [`L57`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L57) — Performs a single training step.
  - `domain_width` — [`L27`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L27)
  - `dx` — [`L28`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L28)
  - `hypers` — [`L26`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L26)
  - `optimizer` — [`L73`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L73)
- protocol/private: `__init__`[`L25`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L25)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py:10`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L10)
- doc: Hyperparameters for the optimization process.
- signature: `class Hyperparameters:`
- members:
  - `learning_rate` — [`L14`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L14)
  - `num_intervals` — [`L13`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L13)
  - `num_steps` — [`L15`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L15)
  - `warmup_steps` — [`L16`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L16)
- used by: (6 test-only callers)

## Functions
- `run()` — [`L95`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/third_autocorr_ineq/initial_program.py#L95) — Entry point for running the optimization.

