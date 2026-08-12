---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.filter_hub.base_types`/
symbols:
  call_dynamic_filter: call_dynamic_filter().
  DynamicFilterOutput: DynamicFilterOutput#
  DynamicFilterOutput.keep: DynamicFilterOutput#keep.
  MetricGatherer.on_dynamic_filter_drop: MetricGatherer#on_dynamic_filter_drop().
  MetricGatherer.collect: MetricGatherer#collect().
  DynamicFilterOutput.reason: DynamicFilterOutput#reason.
  MetricGatherer: MetricGatherer#
  MetricGatherer._dynamic_filter_drop_reason_count: MetricGatherer#_dynamic_filter_drop_reason_count.
  MetricGatherer.__init__: MetricGatherer#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py)

## Classes
### `DynamicFilterOutput`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py:6`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L6)
- signature: `class DynamicFilterOutput:`
- members:
  - `keep` — [`L7`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L7)
  - `reason` — [`L8`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L8)
- used by: [`generate_rollout_async`](../sglang_rollout.md#generate_rollout_async), [`check_reward_nonzero_std`](dynamic_sampling_filters.md#check_reward_nonzero_std), [`call_dynamic_filter`](base_types.md#call_dynamic_filter)

### `MetricGatherer`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py:24`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L24)
- signature: `class MetricGatherer:`
- members:
  - `collect(self)` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L33)
  - `on_dynamic_filter_drop(self, reason: str | None)` — [`L28`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L28)
- protocol/private: `__init__`[`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L25), `_dynamic_filter_drop_reason_count`[`L26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L26)
- used by: [`generate_rollout_async`](../sglang_rollout.md#generate_rollout_async)

## Functions
- `call_dynamic_filter(fn, *args, **kwargs)` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/filter_hub/base_types.py#L11)

