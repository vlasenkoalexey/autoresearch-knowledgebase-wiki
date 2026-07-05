---
title: 'Module: examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.uncertainty_ineq.initial_program`/
symbols:
  run_single_trial: run_single_trial().
  run: run().
  get_c4_from_params: get_c4_from_params().
  UncertaintyOptimizer.degrees: UncertaintyOptimizer#degrees.
  UncertaintyOptimizer.optimizer: UncertaintyOptimizer#optimizer.
  UncertaintyOptimizer.train_step: UncertaintyOptimizer#train_step().
  Hyperparameters.num_hermite_coeffs: Hyperparameters#num_hermite_coeffs.
  UncertaintyOptimizer: UncertaintyOptimizer#
  _c4_from_hermite_coeffs: _c4_from_hermite_coeffs().
  Hyperparameters: Hyperparameters#
  UncertaintyOptimizer.hypers: UncertaintyOptimizer#hypers.
  UncertaintyOptimizer.__init__: UncertaintyOptimizer#__init__().
  Hyperparameters.num_restarts: Hyperparameters#num_restarts.
  Hyperparameters.learning_rate: Hyperparameters#learning_rate.
  Hyperparameters.num_steps: Hyperparameters#num_steps.
  UncertaintyOptimizer.hermite_basis: UncertaintyOptimizer#hermite_basis.
  UncertaintyOptimizer.H_vals_at_zero: UncertaintyOptimizer#H_vals_at_zero.
  UncertaintyOptimizer.x_grid: UncertaintyOptimizer#x_grid.
  UncertaintyOptimizer._objective_fn: UncertaintyOptimizer#_objective_fn().
  _build_P_from_hermite_coeffs: _build_P_from_hermite_coeffs().
---
# Module: [`examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py)

## Classes
### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py:17`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L17)
- signature: `class Hyperparameters:`
- members:
  - `learning_rate` — [`L18`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L18)
  - `num_hermite_coeffs` — [`L21`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L21)
  - `num_restarts` — [`L20`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L20)
  - `num_steps` — [`L19`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L19)
- used by: (6 test-only callers)

### `UncertaintyOptimizer`
- def: [`examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py:24`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L24)
- doc: Finds coefficients for a generalized Hermite polynomial P(x) that minimize
- signature: `class UncertaintyOptimizer:`
- members:
  - `_objective_fn(params: jnp.ndarray, hermite_basis, H_vals_at_zero, x_grid)` — [`L47`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L47) — Penalize negative values of P(x) on [0, Xmax]; mild weighting to emphasize larger x.
  - `train_step(params: jnp.ndarray, opt_state: optax.OptState, optimizer, hermite_basis, H_vals_at_zero, x_grid)` — [`L68`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L68)
  - `H_vals_at_zero` — [`L42`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L42)
  - `degrees` — [`L32`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L32)
  - `hermite_basis` — [`L40`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L40)
  - `hypers` — [`L31`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L31)
  - `optimizer` — [`L44`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L44)
  - `x_grid` — [`L43`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L43)
- protocol/private: `__init__`[`L30`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L30)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (2 test-only callers)

## Functions
- `_build_P_from_hermite_coeffs(hermite_coeffs: np.ndarray, degrees: list[int])` — [`L112`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L112) — Build monomial-basis polynomial P from Hermite-basis coefficients.
- `_c4_from_hermite_coeffs(hermite_coeffs: np.ndarray, num_hermite_coeffs: int)` — [`L129`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L129) — Compute r_max and C4 from full Hermite coefficient vector (Google-style).
- `get_c4_from_params(params: np.ndarray, hypers: Hyperparameters)` — [`L160`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L160) — Calculates the precise C4 bound from a final set of parameters.
- `run()` — [`L181`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L181)
- `run_single_trial(optimizer: UncertaintyOptimizer, key: jax.random.PRNGKey)` — [`L84`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/initial_program.py#L84) — Runs one full optimization from a near-good starting point with small noise.

