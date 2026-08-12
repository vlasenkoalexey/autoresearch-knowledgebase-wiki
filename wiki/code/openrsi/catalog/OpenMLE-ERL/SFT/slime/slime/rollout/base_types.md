---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.base_types`/
symbols:
  call_rollout_fn: call_rollout_fn().
  RolloutFnTrainOutput: RolloutFnTrainOutput#
  RolloutFnTrainOutput.samples: RolloutFnTrainOutput#samples.
  RolloutFnEvalOutput: RolloutFnEvalOutput#
  RolloutFnEvalOutput.data: RolloutFnEvalOutput#data.
  RolloutFnEvalOutput.metrics: RolloutFnEvalOutput#metrics.
  RolloutFnTrainOutput.metrics: RolloutFnTrainOutput#metrics.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py)

## Classes
### `RolloutFnEvalOutput`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py:14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L14)
- signature: `class RolloutFnEvalOutput:`
- members:
  - `data` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L15)
  - `metrics` — [`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L16)
- used by: [`_get_rollout_data`](../ray/rollout.md#RolloutManager._get_rollout_data), [`eval`](../ray/rollout.md#RolloutManager.eval), [`call_rollout_fn`](base_types.md#call_rollout_fn), [`generate_rollout`](sglang_rollout.md#generate_rollout), [`eval_rollout`](sglang_rollout.md#eval_rollout)

### `RolloutFnTrainOutput`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py:8`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L8)
- signature: `class RolloutFnTrainOutput:`
- members:
  - `metrics` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L10)
  - `samples` — [`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L9)
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample)
- used by: [`generate_rollout_async`](sglang_rollout.md#generate_rollout_async), [`_get_rollout_data`](../ray/rollout.md#RolloutManager._get_rollout_data), [`call_rollout_fn`](base_types.md#call_rollout_fn), [`generate_rollout`](sglang_rollout.md#generate_rollout)

## Functions
- `call_rollout_fn(fn, *args, evaluation: bool, **kwargs)` — [`L19`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/base_types.py#L19)

