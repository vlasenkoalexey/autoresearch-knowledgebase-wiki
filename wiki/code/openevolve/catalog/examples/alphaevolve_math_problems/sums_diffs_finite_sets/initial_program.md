---
title: 'Module: examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.sums_diffs_finite_sets.initial_program`/
symbols:
  run_single_trial: run_single_trial().
  run: run().
  C6Searcher.anneal_step: C6Searcher#anneal_step().
  C6Searcher.__init__: C6Searcher#__init__().
  Hyperparameters: Hyperparameters#
  Hyperparameters.num_restarts: Hyperparameters#num_restarts.
  C6Searcher._objective_fn: C6Searcher#_objective_fn().
  C6Searcher: C6Searcher#
  Hyperparameters.max_integer: Hyperparameters#max_integer.
  Hyperparameters.num_search_steps: Hyperparameters#num_search_steps.
  Hyperparameters.initial_temperature: Hyperparameters#initial_temperature.
  C6Searcher.hypers: C6Searcher#hypers.
  C6Searcher.allowed_values: C6Searcher#allowed_values.
---
# Module: [`examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py)

## Classes
### `C6Searcher`
- def: [`examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py:17`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L17)
- doc: Searches for a set U by running the search in pure Python for correctness.
- signature: `class C6Searcher:`
- members:
  - `_objective_fn(u_mask: jnp.ndarray)` — [`L27`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L27) — Calculates the C6 lower bound using jnp.unique
  - `anneal_step(self, key, temp, current_mask, current_loss)` — [`L47`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L47) — Performs one step of Simulated Annealing (not JIT-compiled).
  - `allowed_values` — [`L24`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L24)
  - `hypers` — [`L23`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L23)
- protocol/private: `__init__`[`L22`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L22)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py:10`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L10)
- signature: `class Hyperparameters:`
- members:
  - `initial_temperature` — [`L14`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L14)
  - `max_integer` — [`L11`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L11)
  - `num_restarts` — [`L12`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L12)
  - `num_search_steps` — [`L13`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L13)
- used by: (2 test-only callers)

## Functions
- `run()` — [`L71`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L71)
- `run_single_trial(hypers, key)` — [`L93`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/sums_diffs_finite_sets/initial_program.py#L93)

