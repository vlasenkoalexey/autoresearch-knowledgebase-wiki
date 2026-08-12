---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.data`/
symbols:
  get_data_iterator: get_data_iterator().
  log_rollout_data: log_rollout_data().
  get_batch: get_batch().
  DataIterator: DataIterator#
  DataIterator.get_next: DataIterator#get_next().
  gather_log_data: gather_log_data().
  log_passrate: log_passrate().
  DataIterator.offset: DataIterator#offset.
  DataIterator.reset: DataIterator#reset().
  log_perf_data: log_perf_data().
  log_multi_turn_data: log_multi_turn_data().
  sync_actor_critic_data: sync_actor_critic_data().
  get_data_iterator._generate_data_iterator: get_data_iterator()._generate_data_iterator().
  DataIterator.micro_batch_size: DataIterator#micro_batch_size.
  DataIterator.micro_batch_indices: DataIterator#micro_batch_indices.
  DataIterator.rollout_data: DataIterator#rollout_data.
  DataIterator.__init__: DataIterator#__init__().
  logger: logger.
  log_rollout_data.quantile: log_rollout_data().quantile().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py)

## Classes
### `DataIterator`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py:229`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L229)
- members:
  - `__init__(self, rollout_data: RolloutBatch, micro_batch_size: int | None = None, micro_batch_indices: list[list[int]] | None = None)` — [`L236`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L236) — Initialize an iterator over `rollout_data`.
  - `get_next(self, keys: Sequence[str])` — [`L256`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L256) — Return the next micro-batch for the requested keys.
  - `reset(self)` — [`L287`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L287) — Reset internal offset to the start and return self.
  - `micro_batch_indices` — [`L252`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L252)
  - `micro_batch_size` — [`L251`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L251)
  - `offset` — [`L254`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L254)
  - `rollout_data` — [`L250`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L250)
- uses (calls/refs, reference-scoped): [`RolloutBatch`](../../utils/types.md#RolloutBatch)
- used by: [`train`](model.md#train), [`compute_log_prob`](actor.md#MegatronTrainRayActor.compute_log_prob), [`get_data_iterator`](data.md#get_data_iterator), [`forward_only`](model.md#forward_only), [`get_batch`](data.md#get_batch), [`train_one_step`](model.md#train_one_step), [`forward_step`](model.md#train_one_step.forward_step), [`forward_step`](model.md#forward_only.forward_step), [`_generate_data_iterator`](data.md#get_data_iterator._generate_data_iterator)

## Functions
- `_generate_data_iterator(rollout_data, micro_batch_size, micro_batch_indices=None)` — [`L335`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L335)
- `gather_log_data(metric_name: str, args: Namespace, rollout_id: int, log_dict: dict[str, float])` — [`L182`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L182) — Gather per-rank metrics, reduce by mean on the DP source rank, and log.
- `get_batch(data_iterator: DataIterator, keys: Sequence[str], pad_multiplier: int = 128, qkv_format: str = "thd", allgather_cp: bool = False)` — [`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L25) — Generate a CP-ready micro-batch with packed sequence parameters.
- `get_data_iterator(args: Namespace, model: torch.nn.Module | Sequence[torch.nn.Module], rollout_data: RolloutBatch)` — [`L293`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L293) — Create iterators and a micro-batch schedule for a rollout step.
- `log_multi_turn_data(rollout_id: int, args: Namespace, rollout_data: RolloutBatch)` — [`L538`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L538) — Log multi-turn auxiliary metrics such as raw/observed response lengths and rounds.
- `log_passrate(rollout_id: int, args: Namespace, rollout_data: RolloutBatch)` — [`L577`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L577) — Compute pass@k metrics from `raw_reward` groups and log the results.
- `log_perf_data(rollout_id: int, args: Namespace)` — [`L599`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L599)
- `log_rollout_data(rollout_id: int, args: Namespace, rollout_data: RolloutBatch)` — [`L391`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L391) — Summarize rollout fields and log reduced metrics on PP last stage, TP rank 0.
- `quantile(total_value, n_quantiles, data)` — [`L487`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L487)
- `sync_actor_critic_data(args: Namespace, rollout_data: RolloutBatch | None = None, group: dist.ProcessGroup | None = None)` — [`L614`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L614) — Broadcast `values` (from critic) and optionally `log_probs`/`ref_log_probs`

## Module values
- `logger` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/data.py#L22)

