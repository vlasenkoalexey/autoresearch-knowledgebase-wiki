---
title: 'Module: domains/train_opt/mechanisms/knockout_screen.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/knockout_screen.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.knockout_screen`/
symbols:
  KnockoutScreen.record_knockout: KnockoutScreen#record_knockout().
  KnockoutScreen.suggest_knockout: KnockoutScreen#suggest_knockout().
  KnockoutScreen.get_importance_text: KnockoutScreen#get_importance_text().
  KnockoutScreen._defaults: KnockoutScreen#_defaults.
  KnockoutScreen._knockout_results: KnockoutScreen#_knockout_results.
  KnockoutScreen.set_current_config: KnockoutScreen#set_current_config().
  KnockoutScreen.set_defaults: KnockoutScreen#set_defaults().
  KnockoutScreen.is_knockout_proposal: KnockoutScreen#is_knockout_proposal().
  KnockoutScreen: KnockoutScreen#
  KnockoutScreen._knocked_out: KnockoutScreen#_knocked_out.
  KnockoutScreen._current_config: KnockoutScreen#_current_config.
  logger: logger.
  KnockoutScreen.__init__: KnockoutScreen#__init__().
---
# Module: [`domains/train_opt/mechanisms/knockout_screen.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py)

## Classes
### `KnockoutScreen`
- def: [`domains/train_opt/mechanisms/knockout_screen.py:24`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L24)
- doc: Systematically tests parameter importance by resetting to defaults.
- signature: `class KnockoutScreen:`
- members:
  - `get_importance_text(self)` — [`L117`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L117) — Generate parameter importance rankings from knockout results.
  - `is_knockout_proposal(self, changes: dict)` — [`L158`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L158) — Check if a proposal is actually a knockout (param reset to default).
  - `record_knockout(self, param: str, delta_bpb: float)` — [`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L54) — Record the result of a knockout experiment.
  - `set_current_config(self, config: dict)` — [`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L50) — Update the current best config for comparison.
  - `set_defaults(self, default_config: dict)` — [`L46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L46) — Set the default (baseline) parameter values from original train.py.
  - `suggest_knockout(self, active_params: list[str])` — [`L72`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L72) — Suggest a knockout experiment candidate.
- protocol/private: `__init__`[`L34`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L34), `_current_config`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L44), `_defaults`[`L36`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L36), `_knocked_out`[`L42`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L42), `_knockout_results`[`L40`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L40)
- uses (calls/refs, reference-scoped): [`logger`](knockout_screen.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`run_baseline`](../runner.md#TrainRunner.run_baseline), [`knockout_screen`](../runner.md#TrainRunner.knockout_screen)

## Module values
- `logger` — [`L21`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/knockout_screen.py#L21)

