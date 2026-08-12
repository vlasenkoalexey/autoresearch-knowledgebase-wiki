---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.tensor_backper`/
symbols:
  _TensorBackuperNormal.backup: _TensorBackuperNormal#backup().
  _TensorBackuperNoop.backup: _TensorBackuperNoop#backup().
  _TensorBackuperNoop.restore: _TensorBackuperNoop#restore().
  _TensorBackuperNoop.get: _TensorBackuperNoop#get().
  _TensorBackuperNormal._backups: _TensorBackuperNormal#_backups.
  _TensorBackuperNormal.backup_tags: _TensorBackuperNormal#backup_tags().
  TensorBackuper.create: TensorBackuper#create().
  _TensorBackuperNormal.restore: _TensorBackuperNormal#restore().
  _compute_hash_dict: _compute_hash_dict().
  TensorBackuper._source_getter: TensorBackuper#_source_getter.
  TensorBackuper.backup_tags: TensorBackuper#backup_tags().
  TensorBackuper.get: TensorBackuper#get().
  TensorBackuper.backup: TensorBackuper#backup().
  TensorBackuper.restore: TensorBackuper#restore().
  TensorBackuper.__init__: TensorBackuper#__init__().
  TensorBackuper: TensorBackuper#
  _TensorBackuperNormal.get: _TensorBackuperNormal#get().
  _TensorBackuperNormal.copy: _TensorBackuperNormal#copy().
  _TensorBackuperNormal: _TensorBackuperNormal#
  _TensorBackuperNoop: _TensorBackuperNoop#
  _TensorBackuperNoop._single_tag: _TensorBackuperNoop#_single_tag.
  _TensorBackuperNoop._backup_hash_dict: _TensorBackuperNoop#_backup_hash_dict.
  TensorBackuper.copy: TensorBackuper#copy().
  _TensorBackuperNormal.__init__: _TensorBackuperNormal#__init__().
  _TensorBackuperNoop.__init__: _TensorBackuperNoop#__init__().
  _TensorBackuperNoop.backup_tags: _TensorBackuperNoop#backup_tags().
  _SourceGetter: _SourceGetter.
  _compute_hash_tensor: _compute_hash_tensor().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py)

## Classes
### `TensorBackuper`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py:10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L10)
- signature: `class TensorBackuper(ABC):`
- members:
  - `backup(self, tag: str)` — [`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L31)
  - `backup_tags(self)` — [`L23`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L23)
  - `copy(self, *, src_tag: str, dst_tag: str)` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L34)
  - `create(source_getter, single_tag)` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L12)
  - `get(self, tag: str)` — [`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L27)
  - `restore(self, tag: str)` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L38)
- protocol/private: `__init__`[`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L18), `_source_getter`[`L19`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L19)
- uses (calls/refs, reference-scoped): [`backup`](tensor_backper.md#_TensorBackuperNormal.backup), [`backup`](tensor_backper.md#_TensorBackuperNoop.backup), [`restore`](tensor_backper.md#_TensorBackuperNoop.restore), [`get`](tensor_backper.md#_TensorBackuperNoop.get), [`backup_tags`](tensor_backper.md#_TensorBackuperNormal.backup_tags), [`restore`](tensor_backper.md#_TensorBackuperNormal.restore), [`_TensorBackuperNoop`](tensor_backper.md#_TensorBackuperNoop), [`_TensorBackuperNormal`](tensor_backper.md#_TensorBackuperNormal), [`copy`](tensor_backper.md#_TensorBackuperNormal.copy), [`get`](tensor_backper.md#_TensorBackuperNormal.get), [`backup_tags`](tensor_backper.md#_TensorBackuperNoop.backup_tags), [`_SourceGetter`](tensor_backper.md#_SourceGetter)
- used by: [`weights_backuper`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.weights_backuper), [`backup`](tensor_backper.md#_TensorBackuperNormal.backup), [`backup`](tensor_backper.md#_TensorBackuperNoop.backup), [`restore`](tensor_backper.md#_TensorBackuperNoop.restore), [`get`](tensor_backper.md#_TensorBackuperNoop.get), [`restore`](tensor_backper.md#_TensorBackuperNormal.restore), [`_TensorBackuperNoop`](tensor_backper.md#_TensorBackuperNoop), [`_TensorBackuperNormal`](tensor_backper.md#_TensorBackuperNormal), [`__init__`](tensor_backper.md#_TensorBackuperNoop.__init__), [`__init__`](tensor_backper.md#_TensorBackuperNormal.__init__)

### `_TensorBackuperNoop`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py:77`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L77)
- members:
  - `backup(self, tag: str)` — [`L94`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L94)
  - `backup_tags(self)` — [`L85`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L85)
  - `get(self, tag: str)` — [`L88`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L88)
  - `restore(self, tag: str)` — [`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L99)
- protocol/private: `__init__`[`L78`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L78), `_backup_hash_dict`[`L82`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L82), `_single_tag`[`L80`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L80)
- uses (calls/refs, reference-scoped): [`_compute_hash_dict`](tensor_backper.md#_compute_hash_dict), [`_source_getter`](tensor_backper.md#TensorBackuper._source_getter), [`__init__`](tensor_backper.md#TensorBackuper.__init__), [`TensorBackuper`](tensor_backper.md#TensorBackuper)
- used by: [`create`](tensor_backper.md#TensorBackuper.create), [`backup`](tensor_backper.md#TensorBackuper.backup), [`backup_tags`](tensor_backper.md#TensorBackuper.backup_tags), [`get`](tensor_backper.md#TensorBackuper.get), [`restore`](tensor_backper.md#TensorBackuper.restore)

### `_TensorBackuperNormal`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py:42`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L42)
- members:
  - `backup(self, tag: str)` — [`L55`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L55)
  - `backup_tags(self)` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L48)
  - `copy(self, *, src_tag: str, dst_tag: str)` — [`L64`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L64)
  - `get(self, tag: str)` — [`L51`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L51)
  - `restore(self, tag: str)` — [`L69`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L69)
- protocol/private: `__init__`[`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L43), `_backups`[`L45`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L45)
- uses (calls/refs, reference-scoped): [`_source_getter`](tensor_backper.md#TensorBackuper._source_getter), [`__init__`](tensor_backper.md#TensorBackuper.__init__), [`TensorBackuper`](tensor_backper.md#TensorBackuper)
- used by: [`train_actor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_actor), [`update_weights`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.update_weights), [`weight_updater`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.weight_updater), [`_active_model_tag`](../backends/megatron_utils/actor.md#MegatronTrainRayActor._active_model_tag), [`load_other_checkpoint`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.load_other_checkpoint), [`_switch_model`](../backends/megatron_utils/actor.md#MegatronTrainRayActor._switch_model), [`create`](tensor_backper.md#TensorBackuper.create), [`backup`](tensor_backper.md#TensorBackuper.backup), [`backup_tags`](tensor_backper.md#TensorBackuper.backup_tags), [`get`](tensor_backper.md#TensorBackuper.get), [`restore`](tensor_backper.md#TensorBackuper.restore), [`copy`](tensor_backper.md#TensorBackuper.copy)

## Functions
- `_compute_hash_dict(tensors: dict[str, torch.Tensor])` — [`L105`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L105)
- `_compute_hash_tensor(x: torch.Tensor)` — [`L109`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L109)

## Module values
- `_SourceGetter` — [`L7`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensor_backper.py#L7)

