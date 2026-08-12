---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.initialize`/
symbols:
  init: init().
  logger: logger.
  is_megatron_main_rank: is_megatron_main_rank().
  _set_random_seed: _set_random_seed().
  _initialize_distributed: _initialize_distributed().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py)

## Functions
- `_initialize_distributed(args, get_embedding_ranks=None, get_position_embedding_ranks=None)` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py#L33) — Initialize torch.distributed and core model parallel.
- `_set_random_seed(seed_: int, data_parallel_random_init: bool = False, te_rng_tracker: bool = False, inference_rng_tracker: bool = False, use_cudagraphable_rng: bool = False)` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py#L14) — Set random seed for reproducability.
- `init(args)` — [`L56`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py#L56)
- `is_megatron_main_rank()` — [`L108`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py#L108)

## Module values
- `logger` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/initialize.py#L11)

