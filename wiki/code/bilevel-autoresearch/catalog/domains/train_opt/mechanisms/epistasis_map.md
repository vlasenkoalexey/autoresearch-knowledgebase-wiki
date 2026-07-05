---
title: 'Module: domains/train_opt/mechanisms/epistasis_map.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/epistasis_map.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.epistasis_map`/
symbols:
  EpistasisMap.get_epistasis_text: EpistasisMap#get_epistasis_text().
  EpistasisMap.record: EpistasisMap#record().
  EpistasisMap._solo_effects: EpistasisMap#_solo_effects.
  EpistasisMap: EpistasisMap#
  EpistasisMap._pair_effects: EpistasisMap#_pair_effects.
  EpistasisMap._min_samples_individual: EpistasisMap#_min_samples_individual.
  EpistasisMap._min_samples_pair: EpistasisMap#_min_samples_pair.
  logger: logger.
  EpistasisMap.__init__: EpistasisMap#__init__().
---
# Module: [`domains/train_opt/mechanisms/epistasis_map.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py)

## Classes
### `EpistasisMap`
- def: [`domains/train_opt/mechanisms/epistasis_map.py:19`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L19)
- doc: Tracks pairwise parameter interaction effects (epistasis).
- signature: `class EpistasisMap:`
- members:
  - `get_epistasis_text(self)` — [`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L59) — Generate epistasis analysis for injection into the proposal prompt.
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L40) — Record the outcome of a parameter change (solo or multi-param).
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L32), `_min_samples_individual`[`L33`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L33), `_min_samples_pair`[`L34`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L34), `_pair_effects`[`L38`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L38), `_solo_effects`[`L36`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L36)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`epistasis_map`](../runner.md#TrainRunner.epistasis_map)

## Module values
- `logger` — [`L16`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/epistasis_map.py#L16)

