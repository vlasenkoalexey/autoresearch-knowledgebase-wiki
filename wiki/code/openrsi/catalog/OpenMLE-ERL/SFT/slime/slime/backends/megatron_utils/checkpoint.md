---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.checkpoint`/
symbols:
  load_checkpoint: load_checkpoint().
  _load_checkpoint_hf: _load_checkpoint_hf().
  __post_init__: __post_init__().
  _init_from_local_shards_and_global_metadata: _init_from_local_shards_and_global_metadata().
  logger: logger.
  _is_megatron_checkpoint: _is_megatron_checkpoint().
  _is_dir_nonempty: _is_dir_nonempty().
  __all__: __all__.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py)

## Functions
- `__post_init__(self)` — [`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L25)
- `_init_from_local_shards_and_global_metadata(cls, local_shards: list[Shard], sharded_tensor_metadata: ShardedTensorMetadata, process_group=None, init_rrefs=False, sharding_spec=None)` — [`L31`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L31) — Initialize a ShardedTensor with local shards and a global
- `_is_dir_nonempty(path)` — [`L153`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L153)
- `_is_megatron_checkpoint(path: str | Path)` — [`L123`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L123)
- `_load_checkpoint_hf(ddp_model, optimizer, args, load_path: str)` — [`L129`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L129)
- `load_checkpoint(ddp_model, optimizer, opt_param_scheduler, checkpointing_context, skip_load_to_model_and_opt)` — [`L97`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L97)

## Module values
- `__all__` — [`L94`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L94)
- `logger` — [`L92`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/checkpoint.py#L92)

