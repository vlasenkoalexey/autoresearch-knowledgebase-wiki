---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.tensorboard_utils`/
symbols:
  _TensorboardAdapter._initialize: _TensorboardAdapter#_initialize().
  _TensorboardAdapter: _TensorboardAdapter#
  _TensorboardAdapter.log: _TensorboardAdapter#log().
  _TensorboardAdapter._writer: _TensorboardAdapter#_writer.
  _TensorboardAdapter.__init__: _TensorboardAdapter#__init__().
  _TensorboardAdapter.finish: _TensorboardAdapter#finish().
  logger: logger.
  _resolve_tensorboard_dir: _resolve_tensorboard_dir().
  __all__: __all__.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py)

## Classes
### `_TensorboardAdapter`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py:40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L40)
- signature: `class _TensorboardAdapter(metaclass=SingletonMeta):`
- members:
  - `_initialize(self, tb_project_name, tb_experiment_name)` — [`L65`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L65) — Actual initialization logic
  - `finish(self)` — [`L82`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L82) — Close the tensorboard writer
  - `log(self, data, step)` — [`L72`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L72) — Log data to tensorboard
- protocol/private: `__init__`[`L54`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L54), `_writer`[`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L41)
- uses (calls/refs, reference-scoped): [`SingletonMeta`](misc.md#SingletonMeta), [`_resolve_tensorboard_dir`](tensorboard_utils.md#_resolve_tensorboard_dir), [`logger`](tensorboard_utils.md#logger)
- used by: [`log_perf_data_raw`](train_metric_utils.md#log_perf_data_raw), [`log`](logging_utils.md#log)

## Functions
- `_resolve_tensorboard_dir(tb_project_name, tb_experiment_name)` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L18) — Choose a writer directory whose basename matches the W&B run name when available.

## Module values
- `__all__` — [`L13`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L13)
- `logger` — [`L15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/tensorboard_utils.py#L15)

