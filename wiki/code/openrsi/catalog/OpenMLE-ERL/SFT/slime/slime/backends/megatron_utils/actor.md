---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.backends.megatron_utils.actor`/
symbols:
  MegatronTrainRayActor.train_actor: MegatronTrainRayActor#train_actor().
  MegatronTrainRayActor.update_weights: MegatronTrainRayActor#update_weights().
  MegatronTrainRayActor.train_critic: MegatronTrainRayActor#train_critic().
  MegatronTrainRayActor.weights_backuper: MegatronTrainRayActor#weights_backuper.
  MegatronTrainRayActor.save_model: MegatronTrainRayActor#save_model().
  MegatronTrainRayActor.weight_updater: MegatronTrainRayActor#weight_updater.
  MegatronTrainRayActor.train: MegatronTrainRayActor#train().
  MegatronTrainRayActor._active_model_tag: MegatronTrainRayActor#_active_model_tag.
  MegatronTrainRayActor.init: MegatronTrainRayActor#init().
  MegatronTrainRayActor.compute_log_prob: MegatronTrainRayActor#compute_log_prob().
  MegatronTrainRayActor.load_other_checkpoint: MegatronTrainRayActor#load_other_checkpoint().
  MegatronTrainRayActor.fill_routing_replay: MegatronTrainRayActor#fill_routing_replay().
  MegatronTrainRayActor.rollout_data_postprocess: MegatronTrainRayActor#rollout_data_postprocess.
  MegatronTrainRayActor._switch_model: MegatronTrainRayActor#_switch_model().
  MegatronTrainRayActor.sleep: MegatronTrainRayActor#sleep().
  MegatronTrainRayActor.wake_up: MegatronTrainRayActor#wake_up().
  MegatronTrainRayActor._get_rollout_data: MegatronTrainRayActor#_get_rollout_data().
  MegatronTrainRayActor.model: MegatronTrainRayActor#model.
  MegatronTrainRayActor.opt_param_scheduler: MegatronTrainRayActor#opt_param_scheduler.
  MegatronTrainRayActor.train_parallel_config: MegatronTrainRayActor#train_parallel_config.
  MegatronTrainRayActor.tokenizer: MegatronTrainRayActor#tokenizer.
  MegatronTrainRayActor.pad_func: MegatronTrainRayActor#pad_func().
  MegatronTrainRayActor.connect_actor_critic: MegatronTrainRayActor#connect_actor_critic().
  MegatronTrainRayActor: MegatronTrainRayActor#
  MegatronTrainRayActor.prof: MegatronTrainRayActor#prof.
  logger: logger.
  MegatronTrainRayActor.optimizer: MegatronTrainRayActor#optimizer.
  MegatronTrainRayActor.hf_config: MegatronTrainRayActor#hf_config.
  MegatronTrainRayActor._actor_critic_groups: MegatronTrainRayActor#_actor_critic_groups.
  MegatronTrainRayActor.rollout_engines: MegatronTrainRayActor#rollout_engines.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py)

## Classes
### `MegatronTrainRayActor`  ·  implements/extends TrainRayActor
- def: [`OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py:45`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L45)
- signature: `class MegatronTrainRayActor(TrainRayActor):`
- members:
  - `compute_log_prob(self, data_iterator: list[DataIterator], num_microbatches: list[int], store_prefix: str = "")` — [`L335`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L335)
  - `connect_actor_critic(self, actor_handle: ActorHandle | None = None, master_address: str | None = None, master_port: int | None = None)` — [`L612`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L612)
  - `fill_routing_replay(self, data_iterator, num_microbatches, rollout_data)` — [`L257`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L257)
  - `init(self, args: Namespace, role: str, with_ref: bool = False, with_opd_teacher: bool = False)` — [`L47`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L47)
  - `load_other_checkpoint(self, model_tag: str, path: str)` — [`L582`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L582)
  - `pad_func(experts, pad)` — [`L274`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L274)
  - `save_model(self, rollout_id: int, force_sync: bool = False)` — [`L506`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L506)
  - `sleep(self)` — [`L161`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L161)
  - `train(self, rollout_id: int, rollout_data_ref: Box)` — [`L352`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L352)
  - `train_actor(self, rollout_id: int, rollout_data: RolloutBatch)` — [`L396`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L396)
  - `train_critic(self, rollout_id: int, rollout_data: RolloutBatch)` — [`L368`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L368)
  - `update_weights(self)` — [`L533`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L533)
  - `wake_up(self)` — [`L173`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L173)
  - `hf_config` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L71)
  - `model` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L91)
  - `opt_param_scheduler` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L91)
  - `optimizer` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L91)
  - `prof` — [`L66`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L66)
  - `rollout_data_postprocess` — [`L150`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L150)
  - `rollout_engines` — [`L148`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L148)
  - `tokenizer` — [`L72`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L72)
  - `train_parallel_config` — [`L75`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L75)
  - `weight_updater` — [`L132`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L132)
  - `weights_backuper` — [`L102`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L102)
- protocol/private: `_active_model_tag`[`L111`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L111), `_actor_critic_groups`[`L627`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L627), `_get_rollout_data`[`L183`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L183), `_switch_model`[`L251`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L251)
- uses (calls/refs, reference-scoped): [`args`](../../ray/train_actor.md#TrainRayActor.args), [`load_function`](../../utils/misc.md#load_function), [`print_memory`](../../utils/memory_utils.md#print_memory), [`get_gloo_group`](../../utils/distributed_utils.md#get_gloo_group), [`compute_advantages_and_returns`](loss.md#compute_advantages_and_returns), [`train`](model.md#train), [`timer`](../../utils/timer.md#timer), [`update_weights`](update_weight/update_weight_from_tensor.md#UpdateWeightFromTensor.update_weights), [`RolloutBatch`](../../utils/types.md#RolloutBatch), [`get_data_iterator`](data.md#get_data_iterator), [`log_rollout_data`](data.md#log_rollout_data), [`monkey_patch_torch_dist`](../../utils/reloadable_process_group.md#monkey_patch_torch_dist), [`forward_only`](model.md#forward_only), [`clear_memory`](../../utils/memory_utils.md#clear_memory), [`init_tracking`](../../utils/logging_utils.md#init_tracking), [`Timer`](../../utils/timer.md#Timer), [`named_params_and_buffers`](update_weight/common.md#named_params_and_buffers), [`slice_log_prob_with_cp`](cp_utils.md#slice_log_prob_with_cp), [`init`](initialize.md#init), [`DataIterator`](data.md#DataIterator), [`backup`](../../utils/tensor_backper.md#_TensorBackuperNormal.backup), [`initialize_model_and_optimizer`](model.md#initialize_model_and_optimizer), [`TrainRayActor`](../../ray/train_actor.md#TrainRayActor), [`get_log_probs_and_entropy`](loss.md#get_log_probs_and_entropy), [`inverse_timer`](../../utils/timer.md#inverse_timer), [`load_checkpoint`](checkpoint.md#load_checkpoint), [`RoutingReplay`](../../utils/routing_replay.md#RoutingReplay), [`save`](model.md#save), [`step`](../../utils/profile_utils.md#TrainProfiler.step), [`destroy_process_groups`](../../utils/reloadable_process_group.md#destroy_process_groups), [`reload_process_groups`](../../utils/reloadable_process_group.md#reload_process_groups), [`start`](../../utils/timer.md#Timer.start), [`slice_with_cp`](cp_utils.md#slice_with_cp), [`get_values`](loss.md#get_values), [`Box`](../../utils/misc.md#Box), [`init`](../../ray/train_actor.md#TrainRayActor.init), [`log_perf_data`](data.md#log_perf_data), [`save_hf_model`](model.md#save_hf_model), [`backup_tags`](../../utils/tensor_backper.md#_TensorBackuperNormal.backup_tags), [`process_rollout_data`](../../utils/data.md#process_rollout_data)  (+22 more)
- used by: [`_allocate_gpus_for_actor`](../../ray/actor_group.md#RayTrainGroup._allocate_gpus_for_actor), [`TrainRayActor`](../../ray/train_actor.md#TrainRayActor), [`init`](../../ray/train_actor.md#TrainRayActor.init), [`save_model`](../../ray/train_actor.md#TrainRayActor.save_model), [`sleep`](../../ray/train_actor.md#TrainRayActor.sleep), [`train`](../../ray/train_actor.md#TrainRayActor.train), [`update_weights`](../../ray/train_actor.md#TrainRayActor.update_weights), [`wake_up`](../../ray/train_actor.md#TrainRayActor.wake_up), [`connect_actor_critic`](../../ray/train_actor.md#TrainRayActor.connect_actor_critic)

## Module values
- `logger` — [`L42`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/backends/megatron_utils/actor.py#L42)

