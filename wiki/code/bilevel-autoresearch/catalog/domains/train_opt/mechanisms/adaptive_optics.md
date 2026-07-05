---
title: 'Module: domains/train_opt/mechanisms/adaptive_optics.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/adaptive_optics.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.adaptive_optics`/
symbols:
  AdaptiveOptics.get_seeing_text: AdaptiveOptics#get_seeing_text().
  AdaptiveOptics._noise_std: AdaptiveOptics#_noise_std.
  AdaptiveOptics._history: AdaptiveOptics#_history.
  AdaptiveOptics.record: AdaptiveOptics#record().
  AdaptiveOptics._update_noise_estimate: AdaptiveOptics#_update_noise_estimate().
  AdaptiveOptics._recent_deltas: AdaptiveOptics#_recent_deltas.
  AdaptiveOptics.compute_snr: AdaptiveOptics#compute_snr().
  AdaptiveOptics: AdaptiveOptics#
  AdaptiveOptics._min_samples: AdaptiveOptics#_min_samples.
  logger: logger.
  AdaptiveOptics.__init__: AdaptiveOptics#__init__().
---
# Module: [`domains/train_opt/mechanisms/adaptive_optics.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py)

## Classes
### `AdaptiveOptics`
- def: [`domains/train_opt/mechanisms/adaptive_optics.py:28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L28)
- doc: Estimates measurement noise and computes signal-to-noise ratios.
- signature: `class AdaptiveOptics:`
- members:
  - `_update_noise_estimate(self)` — [`L74`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L74) — Update the noise floor estimate using robust statistics.
  - `compute_snr(self, delta_bpb: float)` — [`L99`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L99) — Compute signal-to-noise ratio for a bpb improvement.
  - `get_seeing_text(self)` — [`L113`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L113) — Generate adaptive optics report for injection into the proposal prompt.
  - `record(self, val_bpb: float, status: str, changes: dict)` — [`L49`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L49) — Record an observation for noise estimation.
- protocol/private: `__init__`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L40), `_history`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L43), `_min_samples`[`L41`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L41), `_noise_std`[`L45`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L45), `_recent_deltas`[`L47`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L47)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`adaptive_optics`](../runner.md#TrainRunner.adaptive_optics)

## Module values
- `logger` — [`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/adaptive_optics.py#L25)

