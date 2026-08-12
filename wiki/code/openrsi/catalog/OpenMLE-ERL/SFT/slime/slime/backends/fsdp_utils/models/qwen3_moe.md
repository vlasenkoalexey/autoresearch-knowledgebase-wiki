---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.models.qwen3_moe`/
symbols:
  Qwen3MoeSparseMoeBlock.forward: Qwen3MoeSparseMoeBlock#forward().
  StandardDispatcher.local_expert_mapping: StandardDispatcher#local_expert_mapping.
  Qwen3MoeSparseMoeBlock.experts: Qwen3MoeSparseMoeBlock#experts.
  fused_experts_impl: fused_experts_impl().
  apply_true_on_policy_patch_for_qwen3_moe: apply_true_on_policy_patch_for_qwen3_moe().
  Qwen3MoeSparseMoeBlock: Qwen3MoeSparseMoeBlock#
  StandardDispatcher.dispatch: StandardDispatcher#dispatch().
  StandardDispatcher.num_local_experts: StandardDispatcher#num_local_experts.
  Qwen3MoeSparseMoeBlock.dispatcher: Qwen3MoeSparseMoeBlock#dispatcher.
  StandardDispatcher.moe_ep_rank: StandardDispatcher#moe_ep_rank.
  StandardDispatcher: StandardDispatcher#
  StandardDispatcher.moe_ep_size: StandardDispatcher#moe_ep_size.
  StandardDispatcher.num_experts: StandardDispatcher#num_experts.
  Qwen3MoeSparseMoeBlock.num_experts: Qwen3MoeSparseMoeBlock#num_experts.
  Qwen3MoeSparseMoeBlock.top_k: Qwen3MoeSparseMoeBlock#top_k.
  Qwen3MoeSparseMoeBlock.norm_topk_prob: Qwen3MoeSparseMoeBlock#norm_topk_prob.
  Qwen3MoeSparseMoeBlock.gate: Qwen3MoeSparseMoeBlock#gate.
  StandardDispatcher.__init__: StandardDispatcher#__init__().
  Qwen3MoeSparseMoeBlock.runner: Qwen3MoeSparseMoeBlock#runner.
  Qwen3MoeSparseMoeBlock.__init__: Qwen3MoeSparseMoeBlock#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py)

## Classes
### `Qwen3MoeSparseMoeBlock`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py:68`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L68)
- signature: `class Qwen3MoeSparseMoeBlock(nn.Module):`
- members:
  - `forward(self, hidden_states: torch.Tensor)` — [`L90`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L90)
  - `dispatcher` — [`L69`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L69)
  - `experts` — [`L81`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L81)
  - `gate` — [`L79`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L79)
  - `norm_topk_prob` — [`L76`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L76)
  - `num_experts` — [`L74`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L74)
  - `runner` — [`L70`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L70)
  - `top_k` — [`L75`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L75)
- protocol/private: `__init__`[`L72`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L72)
- uses (calls/refs, reference-scoped): [`fused_experts_impl`](qwen3_moe.md#fused_experts_impl), [`dispatch`](qwen3_moe.md#StandardDispatcher.dispatch), [`StandardDispatcher`](qwen3_moe.md#StandardDispatcher)
- used by: [`apply_true_on_policy_patch_for_qwen3_moe`](qwen3_moe.md#apply_true_on_policy_patch_for_qwen3_moe)

### `StandardDispatcher`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py:48`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L48)
- signature: `class StandardDispatcher:`
- members:
  - `dispatch(self, topk_ids)` — [`L62`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L62)
  - `local_expert_mapping` — [`L54`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L54)
  - `moe_ep_rank` — [`L53`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L53)
  - `moe_ep_size` — [`L50`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L50)
  - `num_experts` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L51)
  - `num_local_experts` — [`L52`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L52)
- protocol/private: `__init__`[`L49`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L49)
- used by: [`forward`](qwen3_moe.md#Qwen3MoeSparseMoeBlock.forward), [`experts`](qwen3_moe.md#Qwen3MoeSparseMoeBlock.experts)

## Functions
- `apply_true_on_policy_patch_for_qwen3_moe()` — [`L122`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L122)
- `fused_experts_impl(hidden_states: torch.Tensor, w1: torch.Tensor, w2: torch.Tensor, topk_weights: torch.Tensor, topk_ids: torch.Tensor)` — [`L14`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/models/qwen3_moe.py#L14)

