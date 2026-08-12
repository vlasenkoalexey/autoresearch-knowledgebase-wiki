---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.seqlen_balancing`/
symbols:
  State.sets: State#sets.
  get_seqlen_balanced_partitions: get_seqlen_balanced_partitions().
  karmarkar_karp.State.merge: karmarkar_karp().State#merge().
  karmarkar_karp.State.__repr__: karmarkar_karp().State#__repr__().
  Set.items: Set#items.
  karmarkar_karp.State.spread: karmarkar_karp().State#spread().
  Set.sum: Set#sum.
  karmarkar_karp.Set.add: karmarkar_karp().Set#add().
  karmarkar_karp.Set.merge: karmarkar_karp().Set#merge().
  karmarkar_karp.Set.__lt__: karmarkar_karp().Set#__lt__().
  karmarkar_karp.State.get_partitions: karmarkar_karp().State#get_partitions().
  karmarkar_karp.State.__lt__: karmarkar_karp().State#__lt__().
  karmarkar_karp: karmarkar_karp().
  State.k: State#k.
  karmarkar_karp.State: karmarkar_karp().State#
  karmarkar_karp.Set: karmarkar_karp().Set#
  get_seqlen_balanced_partitions._check_and_sort_partitions: get_seqlen_balanced_partitions()._check_and_sort_partitions().
  karmarkar_karp.Set.__init__: karmarkar_karp().Set#__init__().
  karmarkar_karp.State.__init__: karmarkar_karp().State#__init__().
  greedy_partition: greedy_partition().
  get_reverse_idx: get_reverse_idx().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py)

## Classes
### `Set`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py:22`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L22)
- signature: `class Set:`
- members:
  - `add(self, idx: int, val: int)` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L28)
  - `merge(self, other)` — [`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L32)
  - `items` — [`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L26)
  - `sum` — [`L25`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L25)
- protocol/private: `__init__`[`L24`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L24), `__lt__`[`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L37)
- used by: [`sets`](seqlen_balancing.md#State.sets), [`__repr__`](seqlen_balancing.md#karmarkar_karp.State.__repr__), [`merge`](seqlen_balancing.md#karmarkar_karp.State.merge), [`spread`](seqlen_balancing.md#karmarkar_karp.State.spread), [`get_partitions`](seqlen_balancing.md#karmarkar_karp.State.get_partitions)

### `State`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py:44`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L44)
- signature: `class State:`
- members:
  - `get_partitions(self)` — [`L55`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L55)
  - `merge(self, other)` — [`L64`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L64)
  - `spread(self)` — [`L70`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L70)
  - `k` — [`L47`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L47)
  - `sets` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L49)
- protocol/private: `__init__`[`L46`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L46), `__lt__`[`L73`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L73), `__repr__`[`L81`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L81)
- uses (calls/refs, reference-scoped): [`items`](seqlen_balancing.md#Set.items), [`add`](seqlen_balancing.md#karmarkar_karp.Set.add), [`merge`](seqlen_balancing.md#karmarkar_karp.Set.merge), [`sum`](seqlen_balancing.md#Set.sum), [`Set`](seqlen_balancing.md#karmarkar_karp.Set)
- used by: [`karmarkar_karp`](seqlen_balancing.md#karmarkar_karp)

## Functions
- `_check_and_sort_partitions(partitions)` — [`L164`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L164)
- `get_reverse_idx(idx_map)` — [`L180`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L180)
- `get_seqlen_balanced_partitions(seqlen_list: list[int], k_partitions: int, equal_size: bool)` — [`L146`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L146) — get order of seq lengths to make partitions balanced, this is
- `greedy_partition(seqlen_list: list[int], k_partitions: int, equal_size: bool)` — [`L126`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L126)
- `karmarkar_karp(seqlen_list: list[int], k_partitions: int, equal_size: bool)` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/seqlen_balancing.py#L20)

