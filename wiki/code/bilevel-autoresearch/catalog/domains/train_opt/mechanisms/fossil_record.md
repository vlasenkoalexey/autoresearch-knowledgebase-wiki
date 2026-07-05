---
title: 'Module: domains/train_opt/mechanisms/fossil_record.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/fossil_record.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.fossil_record`/
symbols:
  FossilRecord._fossils: FossilRecord#_fossils.
  FossilRecord.find_lazarus_candidates: FossilRecord#find_lazarus_candidates().
  FossilRecord.record: FossilRecord#record().
  FossilRecord.suggest_revival: FossilRecord#suggest_revival().
  FossilRecord.get_fossil_text: FossilRecord#get_fossil_text().
  FossilRecord: FossilRecord#
  FossilRecord._max_fossils: FossilRecord#_max_fossils.
  FossilRecord._revival_suggested: FossilRecord#_revival_suggested.
  logger: logger.
  FossilRecord.__init__: FossilRecord#__init__().
---
# Module: [`domains/train_opt/mechanisms/fossil_record.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py)

## Classes
### `FossilRecord`
- def: [`domains/train_opt/mechanisms/fossil_record.py:32`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L32)
- doc: Preserves extinct configs and suggests Lazarus revivals.
- signature: `class FossilRecord:`
- members:
  - `find_lazarus_candidates(self, current_best_bpb: float, active_params: list[str], n_candidates: int = 3)` — [`L82`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L82) — Find the most promising fossils for revival.
  - `get_fossil_text(self)` — [`L216`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L216) — Generate a fossil record summary for the proposal prompt.
  - `record(self, iteration: int, changes: dict, val_bpb: float, best_bpb_before: float, status: str, config_snapshot: dict | None = None)` — [`L56`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L56) — Record every evaluated config in the fossil record.
  - `suggest_revival(self, current_config: dict, current_best_bpb: float, active_params: list[str])` — [`L144`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L144) — Suggest a Lazarus revival -- re-apply the direction of a promising fossil.
- protocol/private: `__init__`[`L48`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L48), `_fossils`[`L52`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L52), `_max_fossils`[`L49`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L49), `_revival_suggested`[`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L54)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`fossil_record`](../runner.md#TrainRunner.fossil_record)

## Module values
- `logger` — [`L29`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/fossil_record.py#L29)

