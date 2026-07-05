---
title: 'Module: domains/train_opt/mechanisms/context_stratigraphy.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/context_stratigraphy.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.context_stratigraphy`/
symbols:
  ContextStratigraphy.get_context_text: ContextStratigraphy#get_context_text().
  ContextStratigraphy.record: ContextStratigraphy#record().
  ContextStratigraphy.find_context_patterns: ContextStratigraphy#find_context_patterns().
  ContextStratigraphy: ContextStratigraphy#
  ContextStratigraphy._context_records: ContextStratigraphy#_context_records.
  ContextStratigraphy._min_observations: ContextStratigraphy#_min_observations.
  ContextStratigraphy._detect_direction: ContextStratigraphy#_detect_direction().
  logger: logger.
  ContextStratigraphy.__init__: ContextStratigraphy#__init__().
---
# Module: [`domains/train_opt/mechanisms/context_stratigraphy.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py)

## Classes
### `ContextStratigraphy`
- def: [`domains/train_opt/mechanisms/context_stratigraphy.py:34`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L34)
- doc: Tracks the full parameter context surrounding each successful change.
- signature: `class ContextStratigraphy:`
- members:
  - `_detect_direction(self, old_val, new_val)` — [`L83`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L83) — Detect change direction.
  - `find_context_patterns(self)` — [`L96`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L96) — Identify context-dependent patterns for each parameter.
  - `get_context_text(self)` — [`L177`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L177) — Generate context analysis text for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L52) — Record a change with its full parameter context.
- protocol/private: `__init__`[`L46`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L46), `_context_records`[`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L50), `_min_observations`[`L47`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L47)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`context_stratigraphy`](../runner.md#TrainRunner.context_stratigraphy)

## Module values
- `logger` — [`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/context_stratigraphy.py#L31)

