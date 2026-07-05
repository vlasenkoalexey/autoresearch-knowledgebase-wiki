---
title: 'Module: examples/alphaevolve_math_problems/matmul/initial_program.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/matmul/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.matmul.initial_program`/
symbols:
  run: run().
  ContinuousOptimizer._loss_fn: ContinuousOptimizer#_loss_fn().
  DiscreteOptimizer._loss_fn: DiscreteOptimizer#_loss_fn().
  ContinuousOptimizer._get_constrained_decomposition: ContinuousOptimizer#_get_constrained_decomposition().
  ContinuousOptimizer.opt: ContinuousOptimizer#opt.
  DiscreteOptimizer.opt: DiscreteOptimizer#opt.
  round_to_half_ste: round_to_half_ste().
  Hyperparameters.rank: Hyperparameters#rank.
  n: n.
  m: m.
  p: p.
  round_ste_fwd: round_ste_fwd().
  l2_loss_real: l2_loss_real().
  Hyperparameters: Hyperparameters#
  ContinuousOptimizer.__init__: ContinuousOptimizer#__init__().
  DiscreteOptimizer.__init__: DiscreteOptimizer#__init__().
  Hyperparameters.num_restarts: Hyperparameters#num_restarts.
  ContinuousOptimizer.hypers: ContinuousOptimizer#hypers.
  train_step: train_step().
  round_ste_bwd: round_ste_bwd().
  weighted_l2_loss: weighted_l2_loss().
  Hyperparameters.phase1_steps: Hyperparameters#phase1_steps.
  Hyperparameters.phase1_lr: Hyperparameters#phase1_lr.
  Hyperparameters.init_scale: Hyperparameters#init_scale.
  Hyperparameters.l1_strength: Hyperparameters#l1_strength.
  Hyperparameters.clamp_range: Hyperparameters#clamp_range.
  Hyperparameters.phase2_steps: Hyperparameters#phase2_steps.
  Hyperparameters.phase2_lr: Hyperparameters#phase2_lr.
  ContinuousOptimizer: ContinuousOptimizer#
  ContinuousOptimizer.target_tensor: ContinuousOptimizer#target_tensor.
  DiscreteOptimizer: DiscreteOptimizer#
  DiscreteOptimizer.target_tensor: DiscreteOptimizer#target_tensor.
  get_matrix_multiplication_tensor: get_matrix_multiplication_tensor().
  DiscreteOptimizer.hypers: DiscreteOptimizer#hypers.
---
# Module: [`examples/alphaevolve_math_problems/matmul/initial_program.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py)

## Classes
### `ContinuousOptimizer`
- def: [`examples/alphaevolve_math_problems/matmul/initial_program.py:67`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L67)
- doc: Finds a high-quality approximate continuous solution.
- signature: `class ContinuousOptimizer:`
- members:
  - `_get_constrained_decomposition(self, latent_decomposition: tuple)` — [`L75`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L75) — Applies a scaled tanh to map latent parameters to the desired range.
  - `hypers` — [`L72`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L72)
  - `opt` — [`L73`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L73)
  - `target_tensor` — [`L71`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L71)
- protocol/private: `__init__`[`L70`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L70), `_loss_fn`[`L81`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L81)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (1 test-only callers)

### `DiscreteOptimizer`
- def: [`examples/alphaevolve_math_problems/matmul/initial_program.py:89`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L89)
- doc: Refines a continuous solution into an exact discrete one using an STE.
- signature: `class DiscreteOptimizer:`
- members:
  - `hypers` — [`L94`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L94)
  - `opt` — [`L95`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L95)
  - `target_tensor` — [`L93`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L93)
- protocol/private: `__init__`[`L92`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L92), `_loss_fn`[`L97`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L97)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `Hyperparameters`
- def: [`examples/alphaevolve_math_problems/matmul/initial_program.py:52`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L52)
- signature: `class Hyperparameters:`
- members:
  - `clamp_range` — [`L60`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L60)
  - `init_scale` — [`L58`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L58)
  - `l1_strength` — [`L59`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L59)
  - `num_restarts` — [`L55`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L55)
  - `phase1_lr` — [`L57`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L57)
  - `phase1_steps` — [`L56`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L56)
  - `phase2_lr` — [`L63`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L63)
  - `phase2_steps` — [`L62`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L62)
  - `rank` — [`L53`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L53)
- used by: (7 test-only callers)

## Functions
- `get_matrix_multiplication_tensor(n, m, p)` — [`L113`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L113)
- `l2_loss_real(x: jnp.ndarray, y: jnp.ndarray)` — [`L46`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L46)
- `round_ste_bwd(res, g)` — [`L30`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L30) — Backward pass: Identity function, passes gradient straight through.
- `round_ste_fwd(x)` — [`L25`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L25) — Standard forward pass and identity for backward pass.
- `round_to_half_ste(x)` — [`L20`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L20) — Forward pass: snaps values to the nearest half-integer.
- `run()` — [`L120`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L120)
- `train_step(params, opt_state, optimizer, loss_fn)` — [`L106`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L106)
- `weighted_l2_loss(reconstructed: jnp.ndarray, target: jnp.ndarray)` — [`L40`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L40)

## Module values
- `m` — [`L7`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L7)
- `n` — [`L7`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L7)
- `p` — [`L7`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/matmul/initial_program.py#L7)

