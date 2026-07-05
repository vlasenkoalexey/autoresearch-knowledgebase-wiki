---
title: 'Module: domains/train_opt/mechanisms/excavation_grid.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/excavation_grid.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.excavation_grid`/
symbols:
  ExcavationGrid.record: ExcavationGrid#record().
  ExcavationGrid.get_excavation_text: ExcavationGrid#get_excavation_text().
  PARAM_RANGES: PARAM_RANGES.
  ExcavationGrid.get_underexplored: ExcavationGrid#get_underexplored().
  ExcavationGrid._grid: ExcavationGrid#_grid.
  ExcavationGrid._get_bin_range: ExcavationGrid#_get_bin_range().
  ExcavationGrid._get_bin: ExcavationGrid#_get_bin().
  ExcavationGrid.suggest_excavation: ExcavationGrid#suggest_excavation().
  ExcavationGrid: ExcavationGrid#
  ExcavationGrid._bin_best: ExcavationGrid#_bin_best.
  ExcavationGrid._bin_results: ExcavationGrid#_bin_results.
  logger: logger.
  ExcavationGrid.__init__: ExcavationGrid#__init__().
---
# Module: [`domains/train_opt/mechanisms/excavation_grid.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py)

## Classes
### `ExcavationGrid`
- def: [`domains/train_opt/mechanisms/excavation_grid.py:47`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L47)
- doc: Systematic coverage tracker for parameter space exploration.
- signature: `class ExcavationGrid:`
- members:
  - `_get_bin(self, param: str, value)` — [`L73`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L73) — Map a parameter value to its grid bin index.
  - `_get_bin_range(self, param: str, bin_idx: int)` — [`L90`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L90) — Get the value range for a given bin.
  - `get_excavation_text(self)` — [`L184`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L184) — Generate coverage map text for the proposal prompt.
  - `get_underexplored(self, active_params: list[str], n: int = 3)` — [`L110`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L110) — Find the most under-explored parameter-bin combinations.
  - `record(self, config: dict, val_bpb: float)` — [`L100`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L100) — Record a configuration's position in the grid.
  - `suggest_excavation(self, current_config: dict, active_params: list[str])` — [`L145`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L145) — Suggest a systematic excavation of an under-explored grid cell.
- protocol/private: `__init__`[`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L59), `_bin_best`[`L65`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L65), `_bin_results`[`L69`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L69), `_grid`[`L61`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L61)
- uses (calls/refs, reference-scoped): [`PARAM_RANGES`](excavation_grid.md#PARAM_RANGES)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`run_baseline`](../runner.md#TrainRunner.run_baseline), [`excavation_grid`](../runner.md#TrainRunner.excavation_grid)

## Module values
- `PARAM_RANGES` — [`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L32)
- `logger` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/excavation_grid.py#L28)

