---
title: 'Module: domains/train_opt/mechanisms/domestication.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/domestication.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.domestication`/
symbols:
  Domestication.record: Domestication#record().
  Domestication.get_domestication_text: Domestication#get_domestication_text().
  Domestication._detect_comfort_zone: Domestication#_detect_comfort_zone().
  Domestication._comfort_threshold: Domestication#_comfort_threshold.
  Domestication._recent_params: Domestication#_recent_params.
  Domestication._total_proposals: Domestication#_total_proposals.
  Domestication._solo_change_counts: Domestication#_solo_change_counts.
  Domestication: Domestication#
  FOREIGNIZATION_FRAMES: FOREIGNIZATION_FRAMES.
  Domestication._round_number_count: Domestication#_round_number_count.
  Domestication._last_foreignize_iter: Domestication#_last_foreignize_iter.
  Domestication._foreignize_index: Domestication#_foreignize_index.
  logger: logger.
  Domestication._foreignize_cooldown: Domestication#_foreignize_cooldown.
  Domestication._is_round_number: Domestication#_is_round_number().
  Domestication.__init__: Domestication#__init__().
---
# Module: [`domains/train_opt/mechanisms/domestication.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py)

## Classes
### `Domestication`
- def: [`domains/train_opt/mechanisms/domestication.py:88`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L88)
- doc: Tracks LLM comfort-zone patterns and injects foreignization frames.
- signature: `class Domestication:`
- members:
  - `__init__(self, comfort_threshold: int = 3, foreignize_cooldown: int = 4)` — [`L97`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L97) — Args:
  - `_detect_comfort_zone(self)` — [`L163`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L163) — Detect if the LLM is stuck in comfort-zone patterns.
  - `_is_round_number(self, value)` — [`L121`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L121) — Check if a value is suspiciously 'round' (LLM comfort zone).
  - `get_domestication_text(self, iteration: int)` — [`L207`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L207) — Generate domestication/foreignization context for the prompt.
  - `record(self, changes: dict, iteration: int)` — [`L139`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L139) — Record a proposal for comfort-zone analysis.
- protocol/private: `_comfort_threshold`[`L104`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L104), `_foreignize_cooldown`[`L105`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L105), `_foreignize_index`[`L116`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L116), `_last_foreignize_iter`[`L115`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L115), `_recent_params`[`L108`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L108), `_round_number_count`[`L111`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L111), `_solo_change_counts`[`L119`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L119), `_total_proposals`[`L112`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L112)
- uses (calls/refs, reference-scoped): [`FOREIGNIZATION_FRAMES`](domestication.md#FOREIGNIZATION_FRAMES), [`logger`](domestication.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`domestication`](../runner.md#TrainRunner.domestication)

## Module values
- `FOREIGNIZATION_FRAMES` — [`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L25)
- `logger` — [`L21`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/domestication.py#L21)

