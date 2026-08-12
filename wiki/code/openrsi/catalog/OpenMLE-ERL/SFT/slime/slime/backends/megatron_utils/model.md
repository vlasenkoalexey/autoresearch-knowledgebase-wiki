---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.model`/
symbols:
  train: train().
  forward_only: forward_only().
  initialize_model_and_optimizer: initialize_model_and_optimizer().
  train_one_step: train_one_step().
  save: save().
  setup_model_and_optimizer: setup_model_and_optimizer().
  train_one_step.forward_step: train_one_step().forward_step().
  save_hf_model: save_hf_model().
  forward_only.forward_step: forward_only().forward_step().
  logger: logger.
  should_disable_forward_pre_hook: should_disable_forward_pre_hook().
  disable_forward_pre_hook: disable_forward_pre_hook().
  enable_forward_pre_hook: enable_forward_pre_hook().
  get_optimizer_param_scheduler: get_optimizer_param_scheduler().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py)

## Functions
- `disable_forward_pre_hook(model_chunks: Sequence[DDP], param_sync: bool = True)` — [`L140`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L140) — Disable forward pre-hooks for provided DDP-wrapped model chunks.
- `enable_forward_pre_hook(model_chunks: Sequence[DDP])` — [`L129`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L129) — Enable forward pre-hooks for provided DDP-wrapped model chunks.
- `forward_only(f: Callable[..., dict[str, list[torch.Tensor]]], args: Namespace, model: Sequence[DDP], data_iterator: Sequence[DataIterator], num_microbatches: Sequence[int], store_prefix: str = "")` — [`L153`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L153) — Run forward passes only and collect non-loss outputs (e.g., logprobs).
- `forward_step(data_iterator: DataIterator, model: GPTModel, return_schedule_plan: bool = False)` — [`L190`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L190) — Forward step used by Megatron's pipeline engine.
- `forward_step(data_iterator: DataIterator, model: GPTModel, return_schedule_plan: bool = False)` — [`L341`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L341) — Forward step used by Megatron's pipeline engine during training.
- `get_optimizer_param_scheduler(args: Namespace, optimizer: MegatronOptimizer)` — [`L36`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L36) — Create and configure the optimizer learning-rate/weight-decay scheduler.
- `initialize_model_and_optimizer(args: Namespace, role: str = "actor")` — [`L755`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L755) — Initialize model(s), optimizer, scheduler, and load from checkpoint.
- `save(iteration: int, model: Sequence[DDP], optimizer: MegatronOptimizer, opt_param_scheduler: OptimizerParamScheduler)` — [`L690`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L690) — Persist a training checkpoint safely with forward hooks disabled.
- `save_hf_model(args, rollout_id: int, model: Sequence[DDP])` — [`L718`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L718) — Save Megatron model in HuggingFace format.
- `setup_model_and_optimizer(args: Namespace, role: str = "actor")` — [`L84`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L84) — Build model(s), wrap with DDP, and construct optimizer and scheduler.
- `should_disable_forward_pre_hook(args: Namespace)` — [`L484`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L484) — Block forward pre-hook for certain configurations.
- `train(rollout_id: int, model: Sequence[DDP], optimizer: MegatronOptimizer, opt_param_scheduler: OptimizerParamScheduler, data_iterator: Sequence[DataIterator], num_microbatches: Sequence[int])` — [`L489`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L489) — Run training over a rollout consisting of multiple steps.
- `train_one_step(args: Namespace, rollout_id: int, step_id: int, data_iterator: Sequence[DataIterator], model: Sequence[DDP], optimizer: MegatronOptimizer, opt_param_scheduler: OptimizerParamScheduler, num_microbatches: int)` — [`L299`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L299) — Execute a single pipeline-parallel training step.

## Module values
- `logger` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/model.py#L33)

