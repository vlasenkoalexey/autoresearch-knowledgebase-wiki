---
title: 'Module: domains/train_opt/mechanisms/elite_pool.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/elite_pool.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.elite_pool`/ElitePool#
symbols:
  ElitePool._pool: _pool.
  ElitePool.generate_crossover: generate_crossover().
  ElitePool.add: add().
  ElitePool.get_elite_text: get_elite_text().
  ElitePool: ''
  ElitePool.best_bpb: best_bpb().
  ElitePool._max_size: _max_size.
  ElitePool._EXPRESSION_PARAMS: _EXPRESSION_PARAMS.
  ElitePool._INTEGER_PARAMS: _INTEGER_PARAMS.
  ElitePool.__init__: __init__().
---
# Module: [`domains/train_opt/mechanisms/elite_pool.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py)

## Classes
### `ElitePool`
- def: [`domains/train_opt/mechanisms/elite_pool.py:8`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L8)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L22) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L32)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L79`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L79) — Generate a crossover candidate by interpolating between top-2 elite configs. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
  - `get_elite_text(self)` — [`L37`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L37) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L75`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L75), `_INTEGER_PARAMS`[`L77`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L77), `__init__`[`L17`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L17), `_max_size`[`L18`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L18), `_pool`[`L20`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/elite_pool.py#L20)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`run_baseline`](../runner.md#TrainRunner.run_baseline), [`elite_pool`](../runner.md#TrainRunner.elite_pool)

