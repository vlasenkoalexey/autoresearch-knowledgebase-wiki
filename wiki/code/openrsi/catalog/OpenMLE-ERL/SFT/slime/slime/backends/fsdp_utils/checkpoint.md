---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.checkpoint`/
symbols:
  load: load().
  save: save().
  logger: logger.
  OptimizerState.state_dict: OptimizerState#state_dict().
  OptimizerState.load_state_dict: OptimizerState#load_state_dict().
  _read_checkpoint_metadata: _read_checkpoint_metadata().
  ModelState.state_dict: ModelState#state_dict().
  ModelState.load_state_dict: ModelState#load_state_dict().
  LRSchedulerState.state_dict: LRSchedulerState#state_dict().
  LRSchedulerState.load_state_dict: LRSchedulerState#load_state_dict().
  ModelState: ModelState#
  ModelState.model: ModelState#model.
  OptimizerState: OptimizerState#
  OptimizerState.model: OptimizerState#model.
  OptimizerState.optimizer: OptimizerState#optimizer.
  LRSchedulerState: LRSchedulerState#
  LRSchedulerState.lr_scheduler: LRSchedulerState#lr_scheduler.
  _write_checkpoint_metadata: _write_checkpoint_metadata().
  finalize_load: finalize_load().
  ModelState.__init__: ModelState#__init__().
  OptimizerState.__init__: OptimizerState#__init__().
  LRSchedulerState.__init__: LRSchedulerState#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py)

## Classes
### `LRSchedulerState`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py:49`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L49)
- doc: Wrapper for LR scheduler state only.
- signature: `class LRSchedulerState(Stateful):`
- members:
  - `load_state_dict(self, state_dict)` — [`L58`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L58)
  - `state_dict(self)` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L55)
  - `lr_scheduler` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L53)
- protocol/private: `__init__`[`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L52)
- used by: [`load`](checkpoint.md#load), [`save`](checkpoint.md#save)

### `ModelState`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py:18`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L18)
- doc: Wrapper for model state only.
- signature: `class ModelState(Stateful):`
- members:
  - `load_state_dict(self, state_dict)` — [`L28`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L28)
  - `state_dict(self)` — [`L24`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L24)
  - `model` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L22)
- protocol/private: `__init__`[`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L21)
- used by: [`load`](checkpoint.md#load), [`save`](checkpoint.md#save)

### `OptimizerState`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py:32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L32)
- doc: Wrapper for optimizer state only.
- signature: `class OptimizerState(Stateful):`
- members:
  - `load_state_dict(self, state_dict)` — [`L43`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L43)
  - `state_dict(self)` — [`L39`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L39)
  - `model` — [`L36`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L36)
  - `optimizer` — [`L37`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L37)
- protocol/private: `__init__`[`L35`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L35)
- used by: [`load`](checkpoint.md#load), [`save`](checkpoint.md#save)

## Functions
- `_read_checkpoint_metadata(path: Path)` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L62)
- `_write_checkpoint_metadata(path: Path, metadata: dict[str, Any])` — [`L72`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L72)
- `finalize_load(actor: Any, checkpoint_payload: dict[str, Any] | None)` — [`L162`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L162)
- `load(actor: Any)` — [`L78`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L78) — Load checkpoint from disk.
- `save(actor: Any, iteration: int)` — [`L190`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L190) — Save checkpoint to disk.

## Module values
- `logger` — [`L15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/checkpoint.py#L15)

