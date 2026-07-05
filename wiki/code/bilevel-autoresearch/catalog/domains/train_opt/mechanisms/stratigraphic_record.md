---
title: 'Module: domains/train_opt/mechanisms/stratigraphic_record.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/stratigraphic_record.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.stratigraphic_record`/
symbols:
  StratigraphicRecord._strata: StratigraphicRecord#_strata.
  StratigraphicRecord.get_stratigraphy_text: StratigraphicRecord#get_stratigraphy_text().
  StratigraphicRecord.record: StratigraphicRecord#record().
  StratigraphicRecord.get_param_ages: StratigraphicRecord#get_param_ages().
  StratigraphicRecord.get_foundation_params: StratigraphicRecord#get_foundation_params().
  StratigraphicRecord.get_recent_params: StratigraphicRecord#get_recent_params().
  StratigraphicRecord: StratigraphicRecord#
  StratigraphicRecord._current_iteration: StratigraphicRecord#_current_iteration.
  logger: logger.
  StratigraphicRecord.__init__: StratigraphicRecord#__init__().
---
# Module: [`domains/train_opt/mechanisms/stratigraphic_record.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py)

## Classes
### `StratigraphicRecord`
- def: [`domains/train_opt/mechanisms/stratigraphic_record.py:30`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L30)
- doc: Reconstructs the layer-by-layer provenance of the current config.
- signature: `class StratigraphicRecord:`
- members:
  - `get_foundation_params(self, min_age: int = 5)` — [`L99`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L99) — Identify 'foundation' parameters -- changed early and never modified since.
  - `get_param_ages(self)` — [`L85`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L85) — For each parameter, determine which stratum last changed it.
  - `get_recent_params(self, max_age: int = 2)` — [`L112`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L112) — Identify 'recent' parameters -- changed in the last few iterations.
  - `get_stratigraphy_text(self)` — [`L121`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L121) — Generate a stratigraphic summary for the proposal prompt.
  - `record(self, iteration: int, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L54) — Record an iteration result. Only 'keep' results form new strata.
- protocol/private: `__init__`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L44), `_current_iteration`[`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L52), `_strata`[`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L50)
- uses (calls/refs, reference-scoped): [`logger`](stratigraphic_record.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`stratigraphy`](../runner.md#TrainRunner.stratigraphy)

## Module values
- `logger` — [`L27`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/stratigraphic_record.py#L27)

