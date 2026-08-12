---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.fsdp_utils.actor`/
symbols:
  FSDPTrainRayActor._train_step: FSDPTrainRayActor#_train_step().
  FSDPTrainRayActor._train_core: FSDPTrainRayActor#_train_core().
  FSDPTrainRayActor._compute_log_prob: FSDPTrainRayActor#_compute_log_prob().
  FSDPTrainRayActor.train: FSDPTrainRayActor#train().
  FSDPTrainRayActor.processor: FSDPTrainRayActor#processor.
  FSDPTrainRayActor.update_weights: FSDPTrainRayActor#update_weights().
  FSDPTrainRayActor.sleep: FSDPTrainRayActor#sleep().
  FSDPTrainRayActor.wake_up: FSDPTrainRayActor#wake_up().
  FSDPTrainRayActor._create_ref_model: FSDPTrainRayActor#_create_ref_model().
  FSDPTrainRayActor.weight_updater: FSDPTrainRayActor#weight_updater.
  FSDPTrainRayActor._log_rollout_data: FSDPTrainRayActor#_log_rollout_data().
  FSDPTrainRayActor.fsdp_cpu_offload: FSDPTrainRayActor#fsdp_cpu_offload.
  FSDPTrainRayActor.model: FSDPTrainRayActor#model.
  FSDPTrainRayActor._packed_data: FSDPTrainRayActor#_packed_data().
  FSDPTrainRayActor.ref_model: FSDPTrainRayActor#ref_model.
  FSDPTrainRayActor.init: FSDPTrainRayActor#init().
  FSDPTrainRayActor.dp_mesh: FSDPTrainRayActor#dp_mesh.
  logger: logger.
  FSDPTrainRayActor.dp_size: FSDPTrainRayActor#dp_size.
  FSDPTrainRayActor.max_tokens_per_gpu: FSDPTrainRayActor#max_tokens_per_gpu.
  FSDPTrainRayActor.optimizer: FSDPTrainRayActor#optimizer.
  FSDPTrainRayActor._get_init_weight_context_manager: FSDPTrainRayActor#_get_init_weight_context_manager().
  FSDPTrainRayActor._enable_true_on_policy_optimizations: FSDPTrainRayActor#_enable_true_on_policy_optimizations().
  FSDPTrainRayActor.tokenizer: FSDPTrainRayActor#tokenizer.
  FSDPTrainRayActor.lr_scheduler: FSDPTrainRayActor#lr_scheduler.
  FSDPTrainRayActor.prof: FSDPTrainRayActor#prof.
  gather_log_probs_packed: gather_log_probs_packed().
  sum_of_sample_mean: sum_of_sample_mean().
  FSDPTrainRayActor: FSDPTrainRayActor#
  FSDPTrainRayActor.hf_config: FSDPTrainRayActor#hf_config.
  FSDPTrainRayActor.dp_group: FSDPTrainRayActor#dp_group.
  FSDPTrainRayActor.train_parallel_config: FSDPTrainRayActor#train_parallel_config.
  FSDPTrainRayActor.save_model: FSDPTrainRayActor#save_model().
  FSDPTrainRayActor.get_model_cls: FSDPTrainRayActor#get_model_cls().
  FSDPTrainRayActor.mesh: FSDPTrainRayActor#mesh.
  get_logprob_and_entropy: get_logprob_and_entropy().
  apply_fsdp2: apply_fsdp2().
  selective_log_softmax_compiled: selective_log_softmax_compiled.
  FSDPTrainRayActor.global_step: FSDPTrainRayActor#global_step.
  sum_of_token: sum_of_token().
  FSDPTrainRayActor.micro_step: FSDPTrainRayActor#micro_step.
  FSDPTrainRayActor.cpu_init_weights: FSDPTrainRayActor#cpu_init_weights().
  FSDPTrainRayActor._fsdp2_load_full_state_dict: FSDPTrainRayActor#_fsdp2_load_full_state_dict().
  FSDPTrainRayActor._get_model_inputs_args: FSDPTrainRayActor#_get_model_inputs_args().
  selective_log_softmax_raw: selective_log_softmax_raw().
  move_torch_optimizer: move_torch_optimizer().
  FSDPTrainRayActor._setup_device_mesh: FSDPTrainRayActor#_setup_device_mesh().
  FSDPTrainRayActor.dp_rank: FSDPTrainRayActor#dp_rank.
  FSDPTrainRayActor._has_rollout_log_probs: FSDPTrainRayActor#_has_rollout_log_probs().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py)

## Classes
### `FSDPTrainRayActor`  ·  implements/extends TrainRayActor
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py:34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L34)
- doc: Simplified TrainRayActor for pure HF+FSDP training.
- signature: `class FSDPTrainRayActor(TrainRayActor):`
- members:
  - `_compute_log_prob(self, model_tag: str, packed_batches: list[dict[str, torch.Tensor]], store_prefix: str = "")` — [`L301`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L301) — Compute token log-probabilities for a list of packed batches.
  - `_create_ref_model(self, ref_load_path: str | None)` — [`L755`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L755) — Create and initialize a separate reference model with FSDP2 CPUOffloadPolicy.
  - `_fsdp2_load_full_state_dict(self, model, full_state, device_mesh, cpu_offload)` — [`L229`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L229) — Load full state dict into FSDP2 model with efficient broadcast from rank 0.
  - `_get_init_weight_context_manager(self)` — [`L204`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L204) — Get context manager for model initialization.
  - `_packed_data(self, rollout_data: dict[str, list[torch.Tensor]])` — [`L366`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L366) — Pack variable-length sequences for efficient processing.
  - `_setup_device_mesh(self)` — [`L186`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L186) — Setup device mesh for data parallelism.
  - `cpu_init_weights()` — [`L219`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L219)
  - `get_model_cls(self)` — [`L156`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L156)
  - `init(self, args: Namespace, role: str, with_ref: bool = False, with_opd_teacher: bool = False)` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L48)
  - `save_model(self, rollout_id: int, force_sync: bool = False)` — [`L293`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L293) — Delegate checkpoint saving to the shared checkpoint utilities.
  - `sleep(self)` — [`L269`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L269) — Pause CUDA memory for all tracked tensors.
  - `train(self, rollout_id: int, rollout_data_ref: Box)` — [`L437`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L437) — Run one training update over a rollout batch.
  - `update_weights(self)` — [`L725`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L725) — Synchronize actor weights to rollout engines.
  - `wake_up(self)` — [`L283`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L283) — Resume CUDA memory for all tracked tensors.
  - `dp_group` — [`L199`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L199)
  - `dp_mesh` — [`L200`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L200)
  - `dp_rank` — [`L195`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L195)
  - `dp_size` — [`L194`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L194)
  - `fsdp_cpu_offload` — [`L67`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L67)
  - `global_step` — [`L128`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L128)
  - `hf_config` — [`L83`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L83)
  - `lr_scheduler` — [`L126`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L126)
  - `max_tokens_per_gpu` — [`L147`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L147)
  - `mesh` — [`L198`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L198)
  - `micro_step` — [`L129`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L129)
  - `model` — [`L109`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L109)
  - `optimizer` — [`L115`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L115)
  - `processor` — [`L87`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L87)
  - `prof` — [`L79`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L79)
  - `ref_model` — [`L134`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L134)
  - `tokenizer` — [`L84`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L84)
  - `train_parallel_config` — [`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L60)
  - `weight_updater` — [`L138`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L138)
- protocol/private: `_enable_true_on_policy_optimizations`[`L167`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L167), `_get_model_inputs_args`[`L796`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L796), `_has_rollout_log_probs`[`L611`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L611), `_log_rollout_data`[`L464`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L464), `_train_core`[`L500`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L500), `_train_step`[`L551`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L551)
- uses (calls/refs, reference-scoped): [`args`](../../ray/train_actor.md#TrainRayActor.args), [`print_memory`](../../utils/memory_utils.md#print_memory), [`get_gloo_group`](../../utils/distributed_utils.md#get_gloo_group), [`timer`](../../utils/timer.md#timer), [`log_perf_data_raw`](../../utils/train_metric_utils.md#log_perf_data_raw), [`clear_memory`](../../utils/memory_utils.md#clear_memory), [`init_tracking`](../../utils/logging_utils.md#init_tracking), [`Timer`](../../utils/timer.md#Timer), [`load`](checkpoint.md#load), [`log`](../../utils/logging_utils.md#log), [`save`](checkpoint.md#save), [`TrainRayActor`](../../ray/train_actor.md#TrainRayActor), [`inverse_timer`](../../utils/timer.md#inverse_timer), [`load_processor`](../../utils/processing_utils.md#load_processor), [`update_weights`](update_weight_utils.md#UpdateWeight.update_weights), [`logger`](actor.md#logger), [`step`](../../utils/profile_utils.md#TrainProfiler.step), [`load_tokenizer`](../../utils/processing_utils.md#load_tokenizer), [`start`](../../utils/timer.md#Timer.start), [`Box`](../../utils/misc.md#Box), [`compute_rollout_step`](../../utils/metric_utils.md#compute_rollout_step), [`init`](../../ray/train_actor.md#TrainRayActor.init), [`process_rollout_data`](../../utils/data.md#process_rollout_data), [`with_defer`](../../utils/timer.md#with_defer), [`iterate_train_actor`](../../utils/profile_utils.md#TrainProfiler.iterate_train_actor), [`iterate_train_log_probs`](../../utils/profile_utils.md#TrainProfiler.iterate_train_log_probs), [`rollout_manager`](../../ray/train_actor.md#TrainRayActor.rollout_manager), [`sum_of_sample_mean`](actor.md#sum_of_sample_mean), [`compute_approx_kl`](../../utils/ppo_utils.md#compute_approx_kl), [`UpdateWeightFromDistributed`](update_weight_utils.md#UpdateWeightFromDistributed), [`UpdateWeightFromTensor`](update_weight_utils.md#UpdateWeightFromTensor), [`apply_fsdp2`](actor.md#apply_fsdp2), [`apply_fsdp_moe_patch`](models/qwen3_moe_hf.md#apply_fsdp_moe_patch), [`apply_true_on_policy_patch_for_qwen3_moe`](models/qwen3_moe.md#apply_true_on_policy_patch_for_qwen3_moe), [`get_logprob_and_entropy`](actor.md#get_logprob_and_entropy), [`get_lr_scheduler`](lr_scheduler.md#get_lr_scheduler), [`on_init_end`](../../utils/profile_utils.md#TrainProfiler.on_init_end), [`pack_sequences`](data_packing.md#pack_sequences), [`save_debug_train_data`](../../utils/train_dump_utils.md#save_debug_train_data), [`TrainProfiler`](../../utils/profile_utils.md#TrainProfiler)  (+10 more)
- used by: [`_allocate_gpus_for_actor`](../../ray/actor_group.md#RayTrainGroup._allocate_gpus_for_actor), [`TrainRayActor`](../../ray/train_actor.md#TrainRayActor), [`init`](../../ray/train_actor.md#TrainRayActor.init), [`save_model`](../../ray/train_actor.md#TrainRayActor.save_model), [`sleep`](../../ray/train_actor.md#TrainRayActor.sleep), [`train`](../../ray/train_actor.md#TrainRayActor.train), [`update_weights`](../../ray/train_actor.md#TrainRayActor.update_weights), [`wake_up`](../../ray/train_actor.md#TrainRayActor.wake_up)

## Functions
- `apply_fsdp2(model, mesh=None, cpu_offload=False, args=None)` — [`L928`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L928) — Apply FSDP v2 to the model.
- `gather_log_probs_packed(shifted_logits: torch.Tensor, input_ids: torch.Tensor, allow_compile: bool, cu_seqlens: torch.Tensor | float | None = None, temperature: torch.Tensor | None = None)` — [`L830`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L830) — Gather next-token log probabilities for packed sequences.
- `get_logprob_and_entropy(logits: torch.Tensor, target_tokens: torch.Tensor, allow_compile: bool, temperature: float | None = None)` — [`L864`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L864) — Compute log probabilities and entropy.
- `move_torch_optimizer(optimizer, device)` — [`L913`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L913) — ref: https://github.com/volcengine/verl/blob/main/verl/utils/fsdp_utils.py
- `selective_log_softmax_raw(logits: torch.Tensor, input_ids: torch.Tensor)` — [`L810`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L810) — Fused version of the common `log_softmax -> gather` operation.
- `sum_of_sample_mean(x: torch.Tensor, response_lengths: list[int], loss_masks: list[torch.Tensor])` — [`L892`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L892) — Compute sum of per-sample means across variable-length responses.
- `sum_of_token(x: torch.Tensor, response_lengths: list[int], loss_masks: list[torch.Tensor])` — [`L982`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L982)

## Module values
- `logger` — [`L31`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L31)
- `selective_log_softmax_compiled` — [`L827`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/fsdp_utils/actor.py#L827)

