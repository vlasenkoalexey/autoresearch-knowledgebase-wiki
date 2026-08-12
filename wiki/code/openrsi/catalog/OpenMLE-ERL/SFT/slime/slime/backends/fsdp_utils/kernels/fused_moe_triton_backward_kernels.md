---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.kernels.fused_moe_triton_backward_kernels`/
symbols:
  invoke_fused_moe_backward_kernel: invoke_fused_moe_backward_kernel().
  fused_moe_backward_input_kernel: fused_moe_backward_input_kernel().
  fused_moe_backward_weight_kernel: fused_moe_backward_weight_kernel().
  fused_moe_backward_topk_weights_kernel: fused_moe_backward_topk_weights_kernel().
  invoke_fused_moe_backward_kernel.grid_input: invoke_fused_moe_backward_kernel().grid_input().
  invoke_fused_moe_backward_kernel.grid_weight: invoke_fused_moe_backward_kernel().grid_weight().
  invoke_fused_moe_backward_kernel.grid_topk: invoke_fused_moe_backward_kernel().grid_topk().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py)

## Functions
- `fused_moe_backward_input_kernel(grad_output_ptr, weight_ptr, grad_input_ptr, grad_topk_weights_ptr, topk_weights_ptr, sorted_token_ids_ptr, expert_ids_ptr, num_tokens_post_padded_ptr, N, K, EM, num_valid_tokens, stride_gom, stride_gon, stride_we, stride_wn, stride_wk, stride_gim, stride_gik, BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr, GROUP_SIZE_M: tl.constexpr, MUL_ROUTED_WEIGHT: tl.constexpr, top_k: tl.constexpr, compute_type: tl.constexpr)` — [`L11`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L11) — Backward kernel for computing grad_input.
- `fused_moe_backward_topk_weights_kernel(grad_output_ptr, input_ptr, weight_ptr, grad_topk_weights_ptr, sorted_token_ids_ptr, expert_ids_ptr, num_tokens_post_padded_ptr, N, K, EM, num_valid_tokens, stride_gom, stride_gon, stride_im, stride_ik, stride_we, stride_wn, stride_wk, BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr, top_k: tl.constexpr, compute_type: tl.constexpr)` — [`L273`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L273) — Backward kernel for computing grad_topk_weights.
- `fused_moe_backward_weight_kernel(grad_output_ptr, input_ptr, grad_weight_ptr, topk_weights_ptr, sorted_token_ids_ptr, expert_ids_ptr, num_tokens_post_padded_ptr, N, K, EM, num_valid_tokens, stride_gom, stride_gon, stride_im, stride_ik, stride_gwe, stride_gwn, stride_gwk, BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr, GROUP_SIZE_M: tl.constexpr, MUL_ROUTED_WEIGHT: tl.constexpr, top_k: tl.constexpr, compute_type: tl.constexpr)` — [`L132`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L132) — Backward kernel for computing grad_weight.
- `grid_input(META)` — [`L448`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L448)
- `grid_topk(META)` — [`L513`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L513)
- `grid_weight(META)` — [`L482`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L482)
- `invoke_fused_moe_backward_kernel(grad_output: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, grad_input: torch.Tensor, grad_weight: torch.Tensor, grad_topk_weights: torch.Tensor | None, topk_weights: torch.Tensor, topk_ids: torch.Tensor, sorted_token_ids: torch.Tensor, expert_ids: torch.Tensor, num_tokens_post_padded: torch.Tensor, mul_routed_weight: bool, top_k: int, config: dict[str, Any], compute_type: tl.dtype)` — [`L399`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_moe_triton_backward_kernels.py#L399) — Invoke the fused MOE backward kernels to compute gradients.

