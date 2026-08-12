---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.lr_scheduler`/
symbols:
  FSDPLRScheduler._get_lr_for_group: FSDPLRScheduler#_get_lr_for_group().
  FSDPLRScheduler.lr_decay_style: FSDPLRScheduler#lr_decay_style.
  FSDPLRScheduler.use_checkpoint_lr_scheduler: FSDPLRScheduler#use_checkpoint_lr_scheduler.
  FSDPLRScheduler.min_lr: FSDPLRScheduler#min_lr.
  FSDPLRScheduler.lr_wsd_decay_style: FSDPLRScheduler#lr_wsd_decay_style.
  FSDPLRScheduler.lr_warmup_steps: FSDPLRScheduler#lr_warmup_steps.
  FSDPLRScheduler.lr_decay_steps: FSDPLRScheduler#lr_decay_steps.
  get_lr_scheduler: get_lr_scheduler().
  FSDPLRScheduler.init_lr: FSDPLRScheduler#init_lr.
  FSDPLRScheduler.max_lr: FSDPLRScheduler#max_lr.
  FSDPLRScheduler.wsd_decay_steps: FSDPLRScheduler#wsd_decay_steps.
  FSDPLRScheduler.get_lr: FSDPLRScheduler#get_lr().
  FSDPLRScheduler: FSDPLRScheduler#
  logger: logger.
  FSDPLRScheduler.override_lr_scheduler: FSDPLRScheduler#override_lr_scheduler.
  FSDPLRScheduler.__init__: FSDPLRScheduler#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py)

## Classes
### `FSDPLRScheduler`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py:15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L15)
- doc: Learning rate scheduler for FSDP training.
- signature: `class FSDPLRScheduler(LRScheduler):`
- members:
  - `_get_lr_for_group(self, param_group: dict)` — [`L82`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L82) — Compute learning rate for a specific parameter group.
  - `get_lr(self)` — [`L148`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L148) — Compute the learning rates for each parameter group.
  - `init_lr` — [`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L52)
  - `lr_decay_steps` — [`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L60)
  - `lr_decay_style` — [`L67`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L67)
  - `lr_warmup_steps` — [`L59`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L59)
  - `lr_wsd_decay_style` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L62)
  - `max_lr` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L53)
  - `min_lr` — [`L54`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L54)
  - `override_lr_scheduler` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L71)
  - `use_checkpoint_lr_scheduler` — [`L72`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L72)
  - `wsd_decay_steps` — [`L61`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L61)
- protocol/private: `__init__`[`L36`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L36)
- uses (calls/refs, reference-scoped): [`logger`](lr_scheduler.md#logger)
- used by: [`get_lr_scheduler`](lr_scheduler.md#get_lr_scheduler)

## Functions
- `get_lr_scheduler(args, optimizer: torch.optim.Optimizer)` — [`L157`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L157) — Create and configure the learning-rate scheduler.

## Module values
- `logger` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/lr_scheduler.py#L12)

