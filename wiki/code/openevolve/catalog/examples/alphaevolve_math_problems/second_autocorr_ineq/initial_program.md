---
title: 'Module: examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.second_autocorr_ineq.initial_program`/
symbols:
  C2Optimizer.optimizer: C2Optimizer#optimizer.
  C2Optimizer.hypers: C2Optimizer#hypers.
  C2Optimizer.run_optimization: C2Optimizer#run_optimization().
  run: run().
  C2Optimizer._objective_fn: C2Optimizer#_objective_fn().
  C2Optimizer.train_step: C2Optimizer#train_step().
  Hyperparameters.num_intervals: Hyperparameters#num_intervals.
  Hyperparameters.num_steps: Hyperparameters#num_steps.
  C2Optimizer.__init__: C2Optimizer#__init__().
  Hyperparameters: Hyperparameters#
  Hyperparameters.learning_rate: Hyperparameters#learning_rate.
  Hyperparameters.warmup_steps: Hyperparameters#warmup_steps.
  C2Optimizer: C2Optimizer#
---
# Module: [`examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py)

## Classes
### `C2Optimizer`
- def: [`examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py:19`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L19)
- doc: Optimizes a discretized function to find a lower bound for the C2 constant
- signature: `class C2Optimizer:`
- members:
  - `_objective_fn(self, f_values: jnp.ndarray)` — [`L28`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L28) — Computes the objective function using the unitless norm calculation.
  - `run_optimization(self)` — [`L67`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L67) — Sets up and runs the full optimization process.
  - `train_step(self, f_values: jnp.ndarray, opt_state: optax.OptState)` — [`L60`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L60) — Performs a single training step.
  - `hypers` — [`L26`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L26)
  - `optimizer` — [`L76`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L76)
- protocol/private: `__init__`[`L25`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L25)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py:10`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L10)
- doc: Hyperparameters for the optimization process.
- signature: `class Hyperparameters:`
- members:
  - `learning_rate` — [`L14`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L14)
  - `num_intervals` — [`L13`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L13)
  - `num_steps` — [`L15`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L15)
  - `warmup_steps` — [`L16`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L16)
- used by: (5 test-only callers)

## Functions
- `run()` — [`L98`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/second_autocorr_ineq/initial_program.py#L98) — Entry point for running the optimization.

