---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.kernels.fp8_kernel`/
symbols:
  blockwise_cast_to_fp8_triton: blockwise_cast_to_fp8_triton().
  fp8_max: fp8_max.
  fp8_min: fp8_min.
  ceil_div: ceil_div().
  fp8_dtype: fp8_dtype.
  _blockwise_cast_to_fp8_triton: _blockwise_cast_to_fp8_triton().
  blockwise_cast_to_fp8_triton.grid: blockwise_cast_to_fp8_triton().grid().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py)

## Functions
- `_blockwise_cast_to_fp8_triton(X, Y, S, stride_xm, stride_xn, stride_ym, stride_yn, stride_sm, stride_sn, M, N, eps, fp8_min, fp8_max, BLOCK_M: tl.constexpr = 32, BLOCK_N: tl.constexpr = 128)` — [`L25`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L25)
- `blockwise_cast_to_fp8_triton(x: torch.Tensor, block_size=None)` — [`L61`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L61)
- `ceil_div(x: int, y: int)` — [`L10`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L10) — Perform ceiling division of two integers.
- `grid(meta)` — [`L69`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L69)

## Module values
- `fp8_dtype` — [`L5`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L5)
- `fp8_max` — [`L6`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L6)
- `fp8_min` — [`L7`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/kernels/fp8_kernel.py#L7)

