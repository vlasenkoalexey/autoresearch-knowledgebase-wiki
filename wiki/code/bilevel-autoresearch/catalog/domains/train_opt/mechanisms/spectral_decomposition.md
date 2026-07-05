---
title: 'Module: domains/train_opt/mechanisms/spectral_decomposition.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/spectral_decomposition.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.spectral_decomposition`/
symbols:
  SpectralDecomposition.decompose: SpectralDecomposition#decompose().
  SpectralDecomposition._solo_effects: SpectralDecomposition#_solo_effects.
  SpectralDecomposition._decompositions: SpectralDecomposition#_decompositions.
  SpectralDecomposition.get_attribution_text: SpectralDecomposition#get_attribution_text().
  SpectralDecomposition.record_solo: SpectralDecomposition#record_solo().
  SpectralDecomposition.record_from_changes: SpectralDecomposition#record_from_changes().
  SpectralDecomposition: SpectralDecomposition#
  SpectralDecomposition._min_solo_samples: SpectralDecomposition#_min_solo_samples.
  logger: logger.
  SpectralDecomposition.__init__: SpectralDecomposition#__init__().
---
# Module: [`domains/train_opt/mechanisms/spectral_decomposition.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py)

## Classes
### `SpectralDecomposition`
- def: [`domains/train_opt/mechanisms/spectral_decomposition.py:32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L32)
- doc: Decomposes multi-parameter bpb deltas into per-parameter attributions.
- signature: `class SpectralDecomposition:`
- members:
  - `decompose(self, changes: dict, total_delta: float)` — [`L74`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L74) — Decompose a multi-parameter delta into per-parameter attributions.
  - `get_attribution_text(self)` — [`L136`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L136) — Generate a spectral decomposition report for the proposal prompt.
  - `record_from_changes(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L55`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L55) — Record an experiment, routing to solo or multi as appropriate.
  - `record_solo(self, param: str, delta_bpb: float)` — [`L46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L46) — Record a single-parameter experiment result.
- protocol/private: `__init__`[`L39`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L39), `_decompositions`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L44), `_min_solo_samples`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L40), `_solo_effects`[`L42`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L42)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`spectral_decomposition`](../runner.md#TrainRunner.spectral_decomposition)

## Module values
- `logger` — [`L29`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/spectral_decomposition.py#L29)

