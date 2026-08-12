---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.ppo_utils`/
symbols:
  get_advantages_and_returns_batch: get_advantages_and_returns_batch().
  get_reinforce_plus_plus_returns: get_reinforce_plus_plus_returns().
  calculate_log_probs_and_entropy: calculate_log_probs_and_entropy().
  compute_approx_kl: compute_approx_kl().
  get_advantages_and_returns: get_advantages_and_returns().
  compute_entropy_from_logits: compute_entropy_from_logits().
  compute_opsm_mask: compute_opsm_mask().
  compute_gspo_kl: compute_gspo_kl().
  compute_policy_loss: compute_policy_loss().
  _VocabParallelEntropy.forward: _VocabParallelEntropy#forward().
  compute_log_probs: compute_log_probs().
  get_grpo_returns: get_grpo_returns().
  get_reinforce_plus_plus_baseline_advantages: get_reinforce_plus_plus_baseline_advantages().
  _VocabParallelEntropy: _VocabParallelEntropy#
  _VocabParallelEntropy.mul_reduce: _VocabParallelEntropy#mul_reduce().
  vanilla_gae: vanilla_gae().
  chunked_gae: chunked_gae().
  _VocabParallelEntropy.backward: _VocabParallelEntropy#backward().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py)

## Classes
### `_VocabParallelEntropy`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py:162`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L162)
- signature: `class _VocabParallelEntropy(torch.autograd.Function):`
- members:
  - `backward(ctx, grad_output: torch.Tensor)` — [`L185`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L185)
  - `forward(ctx, vocab_parallel_logits: torch.Tensor, process_group: dist.ProcessGroup)` — [`L165`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L165)
  - `mul_reduce(a, b)` — [`L168`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L168)
- used by: [`compute_entropy_from_logits`](ppo_utils.md#compute_entropy_from_logits)

## Functions
- `calculate_log_probs_and_entropy(logits, tokens, tp_group, with_entropy: bool = False, chunk_size: int = -1)` — [`L649`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L649)
- `chunked_gae(rewards: torch.Tensor, values: torch.Tensor, gamma: float, lambd: float, chunk_size: int = 128)` — [`L506`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L506) — Compute Generalized Advantage Estimation (GAE) using a FlashLinearAttention-
- `compute_approx_kl(log_probs: torch.Tensor, log_probs_base: torch.Tensor, kl_loss_type: str, importance_ratio: torch.Tensor | None = None)` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L12) — Compute the approximate KL divergence between two distributions.
- `compute_entropy_from_logits(logits: torch.Tensor, process_group)` — [`L197`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L197)
- `compute_gspo_kl(full_log_probs: list[torch.Tensor], full_old_log_probs: list[torch.Tensor], local_log_probs: list[torch.Tensor], loss_masks: list[torch.Tensor])` — [`L95`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L95) — Compute GSPO-style per-sequence KL divergence.
- `compute_log_probs(logits: torch.Tensor, tokens: torch.Tensor, process_group: dist.ProcessGroup | None)` — [`L151`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L151)
- `compute_opsm_mask(args: Namespace, full_log_probs: list[torch.Tensor], full_old_log_probs: list[torch.Tensor], advantages: list[torch.Tensor], loss_masks: list[torch.Tensor])` — [`L54`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L54) — Compute Off-Policy Sequence Masking (OPSM) mask.
- `compute_policy_loss(ppo_kl: torch.Tensor, advantages: torch.Tensor, eps_clip: float, eps_clip_high: float, eps_clip_c: float | None = None)` — [`L125`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L125)
- `get_advantages_and_returns(total_len: int, response_len: int, values: torch.Tensor, rewards: torch.Tensor, gamma: float, lambd: float)` — [`L311`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L311) — Function that computes advantages and returns from rewards and values.
- `get_advantages_and_returns_batch(total_lengths, response_lengths, values_list, rewards_list, gamma, lambd, chunked: bool = True)` — [`L374`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L374) — Batched GAE with CP support.
- `get_grpo_returns(rewards: torch.Tensor, kl: list[torch.Tensor])` — [`L201`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L201)
- `get_reinforce_plus_plus_baseline_advantages(rewards: torch.Tensor, kl: list[torch.Tensor], loss_masks: list[torch.Tensor], kl_coef: float)` — [`L281`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L281) — Calculates the unwhitened advantages for the REINFORCE++-baseline algorithm.
- `get_reinforce_plus_plus_returns(rewards: torch.Tensor, kl: list[torch.Tensor], loss_masks: list[torch.Tensor], response_lengths: list[int], total_lengths: list[int], kl_coef: float, gamma: float)` — [`L211`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L211) — Calculates discounted returns for REINFORCE++ (https://arxiv.org/pdf/2501.03262)
- `vanilla_gae(rewards: torch.Tensor, values: torch.Tensor, gamma: float, lambd: float)` — [`L482`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/ppo_utils.py#L482)

