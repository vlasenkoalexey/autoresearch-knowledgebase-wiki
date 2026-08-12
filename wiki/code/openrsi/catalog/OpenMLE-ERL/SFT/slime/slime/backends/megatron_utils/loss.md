---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.loss`/
symbols:
  policy_loss_function: policy_loss_function().
  compute_advantages_and_returns: compute_advantages_and_returns().
  loss_function: loss_function().
  get_log_probs_and_entropy: get_log_probs_and_entropy().
  get_values: get_values().
  value_loss_function: value_loss_function().
  sft_loss_function: sft_loss_function().
  get_responses: get_responses().
  _allgather_cp_redistribute: _allgather_cp_redistribute().
  apply_opd_kl_to_advantages: apply_opd_kl_to_advantages().
  vanilla_tis_function: vanilla_tis_function().
  icepop_function: icepop_function().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py)

## Functions
- `_allgather_cp_redistribute(res: dict[str, list[torch.Tensor]], *, logits: torch.Tensor, args: Namespace, total_lengths: list[int], response_lengths: list[int], max_seq_lens: list[int] | None = None)` — [`L145`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L145) — Redistribute response tensors from allgather-CP layout to zigzag ring-attn layout.
- `apply_opd_kl_to_advantages(args: Namespace, rollout_data: RolloutBatch, advantages: list[torch.Tensor], student_log_probs: list[torch.Tensor] | None)` — [`L359`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L359) — Apply on-policy distillation KL penalty to advantages.
- `compute_advantages_and_returns(args: Namespace, rollout_data: RolloutBatch)` — [`L400`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L400) — Compute advantages and returns in-place based on `args.advantage_estimator`.
- `get_log_probs_and_entropy(logits: torch.Tensor, *, args: Namespace, unconcat_tokens: list[torch.Tensor], total_lengths: list[int], response_lengths: list[int], with_entropy: bool = False, non_loss_data: bool = True, max_seq_lens: list[int] | None = None)` — [`L225`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L225) — Compute per-token log-probabilities (and optionally entropy) on responses.
- `get_responses(logits: torch.Tensor, *, args: Namespace, unconcat_tokens: list[torch.Tensor], total_lengths: list[int], response_lengths: list[int], max_seq_lens: list[int] | None = None)` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L34) — Yield response-aligned `(logits_chunk, tokens_chunk)` pairs per sample.
- `get_values(logits: torch.Tensor, *, args: Namespace, unconcat_tokens: list[torch.Tensor], total_lengths: list[int], response_lengths: list[int], with_entropy: bool = False, non_loss_data: bool = True, max_seq_lens: list[int] | None = None)` — [`L300`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L300) — Extract per-token value predictions over response tokens.
- `icepop_function(args, *, pg_loss: torch.Tensor, train_log_probs: list[torch.Tensor], rollout_log_probs: list[torch.Tensor], loss_masks: list[torch.Tensor], **kwargs: Any)` — [`L587`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L587)
- `loss_function(args: Namespace, batch: RolloutBatch, num_microbatches: int, logits: torch.Tensor)` — [`L943`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L943) — Dispatch to the configured loss and rescale for Megatron integration.
- `policy_loss_function(args: Namespace, batch: RolloutBatch, logits: torch.Tensor, sum_of_sample_mean: Callable[[torch.Tensor], torch.Tensor])` — [`L613`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L613) — Compute policy loss (PPO/GSPO) and metrics.
- `sft_loss_function(args: Namespace, batch: RolloutBatch, logits: torch.Tensor, sum_of_sample_mean: Callable[[torch.Tensor], torch.Tensor])` — [`L892`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L892) — Compute supervised fine-tuning loss over response tokens.
- `value_loss_function(args: Namespace, batch: RolloutBatch, logits: torch.Tensor, sum_of_sample_mean: Callable[[torch.Tensor], torch.Tensor])` — [`L834`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L834) — Compute clipped value loss and metrics.
- `vanilla_tis_function(args, *, pg_loss: torch.Tensor, train_log_probs: list[torch.Tensor], rollout_log_probs: list[torch.Tensor], loss_masks: list[torch.Tensor], **kwargs: Any)` — [`L563`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/loss.py#L563)

