---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.cp_utils`/
symbols:
  all_gather_with_cp: all_gather_with_cp().
  slice_log_prob_with_cp: slice_log_prob_with_cp().
  get_sum_of_sample_mean: get_sum_of_sample_mean().
  slice_with_cp: slice_with_cp().
  all_gather_with_cp.zero: all_gather_with_cp().zero().
  get_logits_and_tokens_offset_with_cp: get_logits_and_tokens_offset_with_cp().
  get_sum_of_sample_mean.sum_of_sample_mean: get_sum_of_sample_mean().sum_of_sample_mean().
  get_sum_of_sample_mean.sum_of_token: get_sum_of_sample_mean().sum_of_token().
  slice_with_cp.pad_tokens: slice_with_cp().pad_tokens().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py)

## Functions
- `all_gather_with_cp(tensor: torch.Tensor, total_length: int, response_length: int)` — [`L123`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L123) — Gather tensors across all ranks in the context parallel group.
- `get_logits_and_tokens_offset_with_cp(total_length: int, response_length: int, qkv_format: str = "thd", max_seq_len: int | None = None)` — [`L9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L9) — All offsets start from the begining of the prompt.
- `get_sum_of_sample_mean(total_lengths: list[int], response_lengths: list[int], loss_masks: list[torch.Tensor], calculate_per_token_loss: bool = False, qkv_format: str = "thd", max_seq_lens: list[int] | None = None)` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L53) — Calculate correct sample mean for CP
- `pad_tokens(tokens, pad)` — [`L187`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L187)
- `slice_log_prob_with_cp(log_prob: list[float] | torch.Tensor, total_length: int, response_length: int, qkv_format: str = "thd", max_token_len: int | None = None)` — [`L219`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L219)
- `slice_with_cp(tokens: torch.Tensor, pad_value: tuple[int, float, Callable], qkv_format: str = "thd", max_seq_len: int | None = None)` — [`L175`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L175)
- `sum_of_sample_mean(x: torch.Tensor)` — [`L67`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L67)
- `sum_of_token(x: torch.Tensor)` — [`L75`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L75)
- `zero(len: int)` — [`L142`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/cp_utils.py#L142)

