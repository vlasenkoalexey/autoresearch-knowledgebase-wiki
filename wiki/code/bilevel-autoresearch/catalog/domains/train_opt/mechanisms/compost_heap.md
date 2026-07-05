---
title: 'Module: domains/train_opt/mechanisms/compost_heap.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/compost_heap.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.compost_heap`/
symbols:
  CompostHeap.record: CompostHeap#record().
  CompostHeap.get_compost_text: CompostHeap#get_compost_text().
  CompostHeap._rebuild_barren_zones: CompostHeap#_rebuild_barren_zones().
  CompostHeap._barren_zones: CompostHeap#_barren_zones.
  CompostHeap._failure_records: CompostHeap#_failure_records.
  CompostHeap: CompostHeap#
  CompostHeap._min_failures_for_zone: CompostHeap#_min_failures_for_zone.
  CompostHeap._total_composted: CompostHeap#_total_composted.
  CompostHeap._multi_param_failures: CompostHeap#_multi_param_failures.
  logger: logger.
  CompostHeap.__init__: CompostHeap#__init__().
---
# Module: [`domains/train_opt/mechanisms/compost_heap.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py)

## Classes
### `CompostHeap`
- def: [`domains/train_opt/mechanisms/compost_heap.py:33`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L33)
- doc: Transforms failed experiments into structured guidance for future proposals.
- signature: `class CompostHeap:`
- members:
  - `_rebuild_barren_zones(self)` — [`L102`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L102) — Distill failure records into barren zones per parameter.
  - `get_compost_text(self)` — [`L136`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L136) — Generate compost-derived guidance for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L59) — Compost a failed experiment — extract nutrients from failure.
- protocol/private: `__init__`[`L42`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L42), `_barren_zones`[`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L54), `_failure_records`[`L47`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L47), `_min_failures_for_zone`[`L43`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L43), `_multi_param_failures`[`L51`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L51), `_total_composted`[`L57`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L57)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`compost_heap`](../runner.md#TrainRunner.compost_heap)

## Module values
- `logger` — [`L30`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/compost_heap.py#L30)

