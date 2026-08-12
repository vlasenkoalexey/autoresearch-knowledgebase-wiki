---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.kernels.fused_experts`/
symbols:
  GateUpProjFunction.backward: GateUpProjFunction#backward().
  DownProjFunction.backward: DownProjFunction#backward().
  GateUpProjFunction: GateUpProjFunction#
  SiluAndMulFunction: SiluAndMulFunction#
  DownProjFunction: DownProjFunction#
  MoeSumReduceFunction: MoeSumReduceFunction#
  GateUpProjFunction.forward: GateUpProjFunction#forward().
  SiluAndMulFunction.forward: SiluAndMulFunction#forward().
  SiluAndMulFunction.backward: SiluAndMulFunction#backward().
  DownProjFunction.forward: DownProjFunction#forward().
  MoeSumReduceFunction.forward: MoeSumReduceFunction#forward().
  MoeSumReduceFunction.backward: MoeSumReduceFunction#backward().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py)

## Classes
### `DownProjFunction`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py:203`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L203)
- signature: `class DownProjFunction(torch.autograd.Function):`
- members:
  - `backward(ctx, grad_output)` — [`L283`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L283) — Backward pass for DownProjFunction using Triton kernels.
  - `forward(ctx, intermediate_cache2: torch.Tensor, w2: torch.Tensor, topk_weights: torch.Tensor, topk_ids: torch.Tensor)` — [`L205`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L205)
- uses (calls/refs, reference-scoped): [`invoke_fused_moe_backward_kernel`](fused_moe_triton_backward_kernels.md#invoke_fused_moe_backward_kernel)
- used by: [`fused_experts_impl`](../models/qwen3_moe.md#fused_experts_impl)

### `GateUpProjFunction`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L15)
- signature: `class GateUpProjFunction(torch.autograd.Function):`
- members:
  - `backward(ctx, grad_output)` — [`L96`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L96) — Backward pass for GateUpProjFunction using Triton kernels.
  - `forward(ctx, hidden_states: torch.Tensor, w1: torch.Tensor, topk_weights: torch.Tensor, topk_ids: torch.Tensor)` — [`L17`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L17)
- uses (calls/refs, reference-scoped): [`invoke_fused_moe_backward_kernel`](fused_moe_triton_backward_kernels.md#invoke_fused_moe_backward_kernel)
- used by: [`fused_experts_impl`](../models/qwen3_moe.md#fused_experts_impl)

### `MoeSumReduceFunction`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py:360`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L360)
- signature: `class MoeSumReduceFunction(torch.autograd.Function):`
- members:
  - `backward(ctx, grad_output)` — [`L379`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L379)
  - `forward(ctx, intermediate_cache3: torch.Tensor, hidden_states_shape)` — [`L362`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L362)
- used by: [`fused_experts_impl`](../models/qwen3_moe.md#fused_experts_impl)

### `SiluAndMulFunction`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py:173`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L173)
- signature: `class SiluAndMulFunction(torch.autograd.Function):`
- members:
  - `backward(ctx, grad_output)` — [`L188`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L188)
  - `forward(ctx, intermediate_cache1: torch.Tensor)` — [`L175`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/kernels/fused_experts.py#L175)
- used by: [`fused_experts_impl`](../models/qwen3_moe.md#fused_experts_impl)

