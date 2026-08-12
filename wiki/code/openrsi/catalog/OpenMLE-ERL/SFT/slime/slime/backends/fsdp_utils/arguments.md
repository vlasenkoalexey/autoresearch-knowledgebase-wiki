---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.arguments`/
symbols:
  fsdp_parse_args: fsdp_parse_args().
  _parse_fsdp_cli: _parse_fsdp_cli().
  FSDPArgs: FSDPArgs#
  FSDPArgs.optimizer: FSDPArgs#optimizer.
  FSDPArgs.lr: FSDPArgs#lr.
  FSDPArgs.lr_warmup_init: FSDPArgs#lr_warmup_init.
  FSDPArgs.min_lr: FSDPArgs#min_lr.
  FSDPArgs.lr_decay_style: FSDPArgs#lr_decay_style.
  FSDPArgs.lr_decay_iters: FSDPArgs#lr_decay_iters.
  FSDPArgs.lr_warmup_iters: FSDPArgs#lr_warmup_iters.
  FSDPArgs.lr_warmup_fraction: FSDPArgs#lr_warmup_fraction.
  FSDPArgs.lr_wsd_decay_iters: FSDPArgs#lr_wsd_decay_iters.
  FSDPArgs.lr_wsd_decay_style: FSDPArgs#lr_wsd_decay_style.
  FSDPArgs.use_checkpoint_lr_scheduler: FSDPArgs#use_checkpoint_lr_scheduler.
  FSDPArgs.override_lr_scheduler: FSDPArgs#override_lr_scheduler.
  FSDPArgs.weight_decay: FSDPArgs#weight_decay.
  FSDPArgs.adam_beta1: FSDPArgs#adam_beta1.
  FSDPArgs.adam_beta2: FSDPArgs#adam_beta2.
  FSDPArgs.adam_eps: FSDPArgs#adam_eps.
  FSDPArgs.warmup_ratio: FSDPArgs#warmup_ratio.
  FSDPArgs.attn_implementation: FSDPArgs#attn_implementation.
  FSDPArgs.wandb_project: FSDPArgs#wandb_project.
  FSDPArgs.wandb_run_name: FSDPArgs#wandb_run_name.
  FSDPArgs.gradient_checkpointing: FSDPArgs#gradient_checkpointing.
  FSDPArgs.fp16: FSDPArgs#fp16.
  FSDPArgs.fsdp_state_dict_cpu_offload: FSDPArgs#fsdp_state_dict_cpu_offload.
  FSDPArgs.fsdp_cpu_offload: FSDPArgs#fsdp_cpu_offload.
  FSDPArgs.fsdp_cpu_backend: FSDPArgs#fsdp_cpu_backend.
  FSDPArgs.deterministic_mode: FSDPArgs#deterministic_mode.
  FSDPArgs.record_memory_history: FSDPArgs#record_memory_history.
  FSDPArgs.memory_snapshot_path: FSDPArgs#memory_snapshot_path.
  FSDPArgs.use_pytorch_profiler: FSDPArgs#use_pytorch_profiler.
  FSDPArgs.profile_step_start: FSDPArgs#profile_step_start.
  FSDPArgs.profile_step_end: FSDPArgs#profile_step_end.
  FSDPArgs.tensorboard_dir: FSDPArgs#tensorboard_dir.
  FSDPArgs.config: FSDPArgs#config.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py)

## Classes
### `FSDPArgs`
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py:9`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L9)
- signature: `class FSDPArgs:`
- members:
  - `adam_beta1` — [`L24`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L24)
  - `adam_beta2` — [`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L25)
  - `adam_eps` — [`L26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L26)
  - `attn_implementation` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L29)
  - `config` — [`L59`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L59)
  - `deterministic_mode` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L48)
  - `fp16` — [`L37`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L37)
  - `fsdp_cpu_backend` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L44)
  - `fsdp_cpu_offload` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L41)
  - `fsdp_state_dict_cpu_offload` — [`L40`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L40)
  - `gradient_checkpointing` — [`L36`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L36)
  - `lr` — [`L12`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L12)
  - `lr_decay_iters` — [`L16`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L16)
  - `lr_decay_style` — [`L15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L15)
  - `lr_warmup_fraction` — [`L18`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L18)
  - `lr_warmup_init` — [`L13`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L13)
  - `lr_warmup_iters` — [`L17`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L17)
  - `lr_wsd_decay_iters` — [`L19`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L19)
  - `lr_wsd_decay_style` — [`L20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L20)
  - `memory_snapshot_path` — [`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L52)
  - `min_lr` — [`L14`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L14)
  - `optimizer` — [`L11`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L11)
  - `override_lr_scheduler` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L22)
  - `profile_step_end` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L55)
  - `profile_step_start` — [`L54`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L54)
  - `record_memory_history` — [`L51`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L51)
  - `tensorboard_dir` — [`L56`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L56)
  - `use_checkpoint_lr_scheduler` — [`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L21)
  - `use_pytorch_profiler` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L53)
  - `wandb_project` — [`L32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L32)
  - `wandb_run_name` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L33)
  - `warmup_ratio` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L27)
  - `weight_decay` — [`L23`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L23)
- used by: [`_parse_fsdp_cli`](arguments.md#_parse_fsdp_cli)

## Functions
- `_parse_fsdp_cli(extra_args_provider=None, ignore_unknown_args=False)` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L62)
- `fsdp_parse_args(extra_args_provider=None, ignore_unknown_args=False)` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/arguments.py#L91)

