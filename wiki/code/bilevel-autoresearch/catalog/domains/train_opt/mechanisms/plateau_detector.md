---
title: 'Module: domains/train_opt/mechanisms/plateau_detector.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/plateau_detector.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.plateau_detector`/
symbols:
  PlateauDetector.check_plateau: PlateauDetector#check_plateau().
  PlateauDetector._window: PlateauDetector#_window.
  PlateauDetector._recent: PlateauDetector#_recent.
  PlateauDetector.record: PlateauDetector#record().
  PlateauDetector: PlateauDetector#
  PlateauDetector._diversification_active: PlateauDetector#_diversification_active.
  PlateauDetector._min_improvement_threshold: PlateauDetector#_min_improvement_threshold.
  PlateauDetector._recently_plateaued_params: PlateauDetector#_recently_plateaued_params.
  logger: logger.
  PlateauDetector.__init__: PlateauDetector#__init__().
---
# Module: [`domains/train_opt/mechanisms/plateau_detector.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py)

## Classes
### `PlateauDetector`
- def: [`domains/train_opt/mechanisms/plateau_detector.py:9`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L9)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L39`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L39) — Check if we're on a plateau. Returns (is_plateau, directive_text). — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L28) — Record a proposal outcome.
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L20), `_diversification_active`[`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L25), `_min_improvement_threshold`[`L22`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L22), `_recent`[`L24`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L24), `_recently_plateaued_params`[`L26`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L26), `_window`[`L21`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L21)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`plateau_detector`](../runner.md#TrainRunner.plateau_detector)

## Module values
- `logger` — [`L6`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/plateau_detector.py#L6)

