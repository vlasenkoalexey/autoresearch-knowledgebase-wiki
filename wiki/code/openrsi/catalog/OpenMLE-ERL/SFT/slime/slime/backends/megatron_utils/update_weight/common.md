---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.update_weight.common`/
symbols:
  named_params_and_buffers: named_params_and_buffers().
  all_gather_params_async: all_gather_params_async().
  _named_params_and_buffers_vanilla._compute_fqn: _named_params_and_buffers_vanilla()._compute_fqn().
  _named_params_and_buffers_vanilla: _named_params_and_buffers_vanilla().
  all_gather_param: all_gather_param().
  _maybe_get_cpu_backup: _maybe_get_cpu_backup().
  _named_params_and_buffers_global: _named_params_and_buffers_global().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py)

## Functions
- `_compute_fqn(name, vp_stage=vp_stage)` — [`L145`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L145)
- `_maybe_get_cpu_backup(x: torch.Tensor)` — [`L133`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L133)
- `_named_params_and_buffers_global(args: Namespace, model: Sequence[torch.nn.Module])` — [`L158`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L158) — Yield (global_name, param/buffer) with consistent names across PP/EP. Adjusts indices for
- `_named_params_and_buffers_vanilla(model: Sequence[torch.nn.Module])` — [`L142`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L142)
- `all_gather_param(name: str, param: torch.nn.Parameter)` — [`L15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L15) — All-gather TP-sharded param to full tensor. expert_bias→param, non-TP/duplicated→param.data.
- `all_gather_params_async(param_infos_and_params: list[tuple[ParamInfo, torch.Tensor]])` — [`L51`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L51) — Parallel TP all-gather for multiple params. Loop 1: for each TP param, allocate buffers +
- `named_params_and_buffers(args: Namespace, model: Sequence[torch.nn.Module], convert_to_global_name: bool = True, translate_gpu_to_cpu: bool = False)` — [`L116`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/update_weight/common.py#L116)

