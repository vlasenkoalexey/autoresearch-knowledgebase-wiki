---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.rocm_checkpoint_writer`/ROCmFileSystemWriterAsync#
symbols:
  ROCmFileSystemWriterAsync: ''
  ROCmFileSystemWriterAsync.preload_tensors: preload_tensors().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py)

## Classes
### `ROCmFileSystemWriterAsync`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py:5`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py#L5)
- doc: FileSystemWriterAsync wrapper for ROCm compatibility.
- signature: `class ROCmFileSystemWriterAsync(FileSystemWriterAsync):`
- members:
  - `preload_tensors(*args, **kwargs)` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/rocm_checkpoint_writer.py#L14)
- used by: [`main`](../../tools/convert_hf_to_torch_dist.md#main), [`initialize_model_and_optimizer`](../backends/megatron_utils/model.md#initialize_model_and_optimizer)

