---
title: 'Module: examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.first_autocorr_ineq.initial_program`/
symbols:
  AutocorrelationOptimizer.optimizer: AutocorrelationOptimizer#optimizer.
  AutocorrelationOptimizer.run_optimization: AutocorrelationOptimizer#run_optimization().
  AutocorrelationOptimizer.hypers: AutocorrelationOptimizer#hypers.
  run: run().
  AutocorrelationOptimizer.dx: AutocorrelationOptimizer#dx.
  AutocorrelationOptimizer._objective_fn: AutocorrelationOptimizer#_objective_fn().
  AutocorrelationOptimizer.train_step: AutocorrelationOptimizer#train_step().
  Hyperparameters.num_intervals: Hyperparameters#num_intervals.
  Hyperparameters.num_steps: Hyperparameters#num_steps.
  AutocorrelationOptimizer.__init__: AutocorrelationOptimizer#__init__().
  Hyperparameters: Hyperparameters#
  Hyperparameters.learning_rate: Hyperparameters#learning_rate.
  Hyperparameters.warmup_steps: Hyperparameters#warmup_steps.
  Hyperparameters.end_lr_factor: Hyperparameters#end_lr_factor.
  AutocorrelationOptimizer: AutocorrelationOptimizer#
  AutocorrelationOptimizer.domain_width: AutocorrelationOptimizer#domain_width.
---
# Module: [`examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py)

## Classes
### `AutocorrelationOptimizer`
- def: [`examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py:20`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L20)
- doc: Optimizes a discretized function to find the minimal C1 constant.
- signature: `class AutocorrelationOptimizer:`
- members:
  - `_objective_fn(self, f_values: jnp.ndarray)` — [`L30`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L30) — Computes the objective function, which is the C1 ratio.
  - `run_optimization(self)` — [`L65`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L65) — Sets up and runs the full optimization process.
  - `train_step(self, f_values: jnp.ndarray, opt_state: optax.OptState)` — [`L57`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L57) — Performs a single training step.
  - `domain_width` — [`L27`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L27)
  - `dx` — [`L28`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L28)
  - `hypers` — [`L26`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L26)
  - `optimizer` — [`L74`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L74)
- protocol/private: `__init__`[`L25`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L25)
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py:10`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L10)
- doc: Hyperparameters for the optimization process.
- signature: `class Hyperparameters:`
- members:
  - `end_lr_factor` — [`L15`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L15)
  - `learning_rate` — [`L14`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L14)
  - `num_intervals` — [`L13`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L13)
  - `num_steps` — [`L16`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L16)
  - `warmup_steps` — [`L17`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L17)
- used by: (6 test-only callers)

## Functions
- `run()` — [`L103`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/first_autocorr_ineq/initial_program.py#L103) — Entry point for running the optimization and returning results.

