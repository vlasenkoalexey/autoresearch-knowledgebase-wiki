---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.ci_utils`/
symbols:
  check_mtp_only_grad: check_mtp_only_grad().
  logger: logger.
  check_mtp_loss: check_mtp_loss().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py)

## Functions
- `check_mtp_loss(mtp_loss: float, max_mtp_loss: float = 1)` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py#L71) — Check that MTP loss is within expected bounds.
- `check_mtp_only_grad(model: Sequence[DDP], step_id: int)` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py#L11) — Check that only MTP parameters have non-zero gradients.

## Module values
- `logger` — [`L8`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/ci_utils.py#L8)

