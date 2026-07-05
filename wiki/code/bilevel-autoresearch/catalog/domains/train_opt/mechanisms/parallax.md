---
title: 'Module: domains/train_opt/mechanisms/parallax.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/parallax.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.parallax`/
symbols:
  ParallaxEstimator._update_roughness: ParallaxEstimator#_update_roughness().
  ParallaxEstimator.record: ParallaxEstimator#record().
  ParallaxEstimator.get_roughness_text: ParallaxEstimator#get_roughness_text().
  ParallaxEstimator._roughness: ParallaxEstimator#_roughness.
  ParallaxEstimator: ParallaxEstimator#
  ParallaxEstimator._observations: ParallaxEstimator#_observations.
  ParallaxEstimator.get_recommended_step: ParallaxEstimator#get_recommended_step().
  ParallaxEstimator._min_observations: ParallaxEstimator#_min_observations.
  logger: logger.
  ParallaxEstimator.__init__: ParallaxEstimator#__init__().
---
# Module: [`domains/train_opt/mechanisms/parallax.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py)

## Classes
### `ParallaxEstimator`
- def: [`domains/train_opt/mechanisms/parallax.py:35`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L35)
- doc: Estimates landscape roughness per parameter from nearby observations.
- signature: `class ParallaxEstimator:`
- members:
  - `_update_roughness(self, param: str)` — [`L89`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L89) — Update roughness estimate for a parameter.
  - `get_recommended_step(self, param: str)` — [`L163`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L163) — Get a recommended relative step size for a parameter.
  - `get_roughness_text(self)` — [`L124`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L124) — Generate a landscape roughness report for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, status: str)` — [`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L50) — Record an observation for landscape roughness estimation.
- protocol/private: `__init__`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L43), `_min_observations`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L44), `_observations`[`L46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L46), `_roughness`[`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L48)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`parallax_estimator`](../runner.md#TrainRunner.parallax_estimator)

## Module values
- `logger` — [`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/parallax.py#L32)

