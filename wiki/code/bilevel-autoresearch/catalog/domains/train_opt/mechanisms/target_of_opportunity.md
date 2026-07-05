---
title: 'Module: domains/train_opt/mechanisms/target_of_opportunity.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/target_of_opportunity.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.target_of_opportunity`/
symbols:
  TargetOfOpportunity.check_surprise: TargetOfOpportunity#check_surprise().
  TargetOfOpportunity._active_too: TargetOfOpportunity#_active_too.
  TargetOfOpportunity.get_too_text: TargetOfOpportunity#get_too_text().
  TargetOfOpportunity.clear_alert: TargetOfOpportunity#clear_alert().
  TargetOfOpportunity: TargetOfOpportunity#
  TargetOfOpportunity._surprise_history: TargetOfOpportunity#_surprise_history.
  TargetOfOpportunity._last_trigger_iter: TargetOfOpportunity#_last_trigger_iter.
  logger: logger.
  TargetOfOpportunity._cooldown: TargetOfOpportunity#_cooldown.
  TargetOfOpportunity._surprise_threshold: TargetOfOpportunity#_surprise_threshold.
  TargetOfOpportunity.__init__: TargetOfOpportunity#__init__().
---
# Module: [`domains/train_opt/mechanisms/target_of_opportunity.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py)

## Classes
### `TargetOfOpportunity`
- def: [`domains/train_opt/mechanisms/target_of_opportunity.py:30`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L30)
- doc: Detects surprising improvements and generates follow-up directives.
- signature: `class TargetOfOpportunity:`
- members:
  - `check_surprise(self, changes: dict, val_bpb: float, best_bpb_before: float, iteration: int, momentum_signals: dict[str, list[tuple[str, float]]])` — [`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L52) — Check if the latest result is a surprising improvement. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
  - `clear_alert(self)` — [`L175`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L175) — Clear the active ToO alert (called after follow-up iterations).
  - `get_too_text(self)` — [`L139`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L139) — Generate a Target of Opportunity alert for injection into the prompt.
- protocol/private: `__init__`[`L42`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L42), `_active_too`[`L46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L46), `_cooldown`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L43), `_last_trigger_iter`[`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L48), `_surprise_history`[`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L50), `_surprise_threshold`[`L44`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L44)
- uses (calls/refs, reference-scoped): [`logger`](target_of_opportunity.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`target_of_opportunity`](../runner.md#TrainRunner.target_of_opportunity)

## Module values
- `logger` — [`L27`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/target_of_opportunity.py#L27)

