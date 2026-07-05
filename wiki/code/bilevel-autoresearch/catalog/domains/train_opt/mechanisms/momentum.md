---
title: 'Module: domains/train_opt/mechanisms/momentum.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/momentum.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.momentum`/
symbols:
  MomentumTracker.record: MomentumTracker#record().
  MomentumTracker._signals: MomentumTracker#_signals.
  MomentumTracker.get_momentum_text: MomentumTracker#get_momentum_text().
  MomentumTracker: MomentumTracker#
  logger: logger.
  MomentumTracker._detect_direction: MomentumTracker#_detect_direction().
  MomentumTracker.__init__: MomentumTracker#__init__().
---
# Module: [`domains/train_opt/mechanisms/momentum.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py)

## Classes
### `MomentumTracker`
- def: [`domains/train_opt/mechanisms/momentum.py:11`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L11)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L48) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L61`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L61) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L26`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L26) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L20), `_signals`[`L24`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L24)
- uses (calls/refs, reference-scoped): [`logger`](momentum.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`momentum`](../runner.md#TrainRunner.momentum)

## Module values
- `logger` — [`L8`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/momentum.py#L8)

