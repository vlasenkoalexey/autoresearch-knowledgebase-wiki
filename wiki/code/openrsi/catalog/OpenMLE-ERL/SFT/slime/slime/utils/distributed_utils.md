---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.distributed_utils`/
symbols:
  get_gloo_group: get_gloo_group().
  GLOO_GROUP: GLOO_GROUP.
  init_process_group: init_process_group().
  init_gloo_group: init_gloo_group().
  distributed_masked_whiten: distributed_masked_whiten().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py)

## Functions
- `distributed_masked_whiten(values: torch.Tensor, mask: torch.Tensor, process_group: dist.ProcessGroup | None = None, shift_mean: bool = True, epsilon: float = 1e-8)` — [`L94`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py#L94) — Performs whitening on a tensor using global statistics from all participating GPUs.
- `get_gloo_group()` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py#L28) — Get the Gloo group for distributed communication.
- `init_gloo_group()` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py#L20) — Initialize Gloo group for distributed communication.
- `init_process_group(backend: str | Backend = None, init_method: str | None = None, timeout: timedelta | None = None, world_size: int = -1, rank: int = -1, store: Store | None = None, group_name: str = None, pg_options: Any | None = None)` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py#L38)

## Module values
- `GLOO_GROUP` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/distributed_utils.py#L17)

