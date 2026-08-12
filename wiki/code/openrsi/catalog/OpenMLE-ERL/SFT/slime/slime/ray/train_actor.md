---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.train_actor`/
symbols:
  TrainRayActor.args: TrainRayActor#args.
  TrainRayActor.master_port: TrainRayActor#master_port.
  TrainRayActor: TrainRayActor#
  TrainRayActor.with_opd_teacher: TrainRayActor#with_opd_teacher.
  TrainRayActor.init: TrainRayActor#init().
  TrainRayActor.rollout_manager: TrainRayActor#rollout_manager.
  logger: logger.
  TrainRayActor.clear_memory: TrainRayActor#clear_memory().
  TrainRayActor.sleep: TrainRayActor#sleep().
  TrainRayActor.wake_up: TrainRayActor#wake_up().
  TrainRayActor.train: TrainRayActor#train().
  TrainRayActor.save_model: TrainRayActor#save_model().
  TrainRayActor.update_weights: TrainRayActor#update_weights().
  TrainRayActor.set_rollout_manager: TrainRayActor#set_rollout_manager().
  TrainRayActor.role: TrainRayActor#role.
  TrainRayActor.__init__: TrainRayActor#__init__().
  TrainRayActor.connect_actor_critic: TrainRayActor#connect_actor_critic().
  TrainRayActor.master_addr: TrainRayActor#master_addr.
  get_local_gpu_id: get_local_gpu_id().
  TrainRayActor._world_size: TrainRayActor#_world_size.
  TrainRayActor._rank: TrainRayActor#_rank.
  TrainRayActor.with_ref: TrainRayActor#with_ref.
  TrainRayActor._get_parallel_config: TrainRayActor#_get_parallel_config().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py)

## Classes
### `TrainRayActor`  ·  implements/extends RayActor
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py:28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L28)
- signature: `class TrainRayActor(RayActor):`
- members:
  - `clear_memory(self)` — [`L99`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L99)
  - `connect_actor_critic(self, critic_group)` — [`L125`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L125)
  - `init(self, args, role, with_ref=False, with_opd_teacher=False)` — [`L50`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L50)
  - `save_model(self, rollout_id, force_sync=False)` — [`L117`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L117)
  - `set_rollout_manager(self, rollout_manager)` — [`L132`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L132)
  - `sleep(self, tags)` — [`L105`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L105)
  - `train(self, rollout_id, rollout_data_ref)` — [`L113`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L113)
  - `update_weights(self)` — [`L121`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L121)
  - `wake_up(self, tags)` — [`L109`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L109)
  - `args` — [`L51`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L51)
  - `master_addr` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L35)
  - `master_port` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L35)
  - `role` — [`L52`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L52)
  - `rollout_manager` — [`L133`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L133)
  - `with_opd_teacher` — [`L54`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L54)
  - `with_ref` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L53)
- protocol/private: `__init__`[`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L29), `_get_parallel_config`[`L129`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L129), `_rank`[`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L33), `_world_size`[`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L32)
- uses (calls/refs, reference-scoped): [`update_weights`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.update_weights), [`print_memory`](../utils/memory_utils.md#print_memory), [`save_model`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.save_model), [`train`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.train), [`train`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train), [`update_weights`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.update_weights), [`sleep`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.sleep), [`init`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.init), [`wake_up`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.wake_up), [`clear_memory`](../utils/memory_utils.md#clear_memory), [`configure_logger`](../utils/logging_utils.md#configure_logger), [`sleep`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.sleep), [`RayActor`](ray_actor.md#RayActor), [`wake_up`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.wake_up), [`init`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.init), [`EvalDatasetConfig`](../utils/eval_config.md#EvalDatasetConfig), [`_get_current_node_ip_and_free_port`](ray_actor.md#RayActor._get_current_node_ip_and_free_port), [`FSDPTrainRayActor`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor), [`connect_actor_critic`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.connect_actor_critic), [`logger`](train_actor.md#logger), [`save_model`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.save_model), [`MegatronTrainRayActor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor), [`init_gloo_group`](../utils/distributed_utils.md#init_gloo_group), [`get_local_gpu_id`](train_actor.md#get_local_gpu_id)
- used by: [`train_actor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_actor), [`_train_step`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._train_step), [`update_weights`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.update_weights), [`_train_core`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._train_core), [`train_critic`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_critic), [`_compute_log_prob`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._compute_log_prob), [`weights_backuper`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.weights_backuper), [`save_model`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.save_model), [`train`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.train), [`weight_updater`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.weight_updater), [`processor`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.processor), [`train`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train), [`update_weights`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.update_weights), [`sleep`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.sleep), [`_active_model_tag`](../backends/megatron_utils/actor.md#MegatronTrainRayActor._active_model_tag), [`init`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.init), [`_create_ref_model`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._create_ref_model), [`wake_up`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.wake_up), [`compute_log_prob`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.compute_log_prob), [`load_other_checkpoint`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.load_other_checkpoint), [`weight_updater`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.weight_updater), [`_log_rollout_data`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._log_rollout_data), [`fill_routing_replay`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.fill_routing_replay), [`rollout_data_postprocess`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.rollout_data_postprocess), [`fsdp_cpu_offload`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.fsdp_cpu_offload), [`sleep`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.sleep), [`RayActor`](ray_actor.md#RayActor), [`_get_rollout_data`](../backends/megatron_utils/actor.md#MegatronTrainRayActor._get_rollout_data), [`_packed_data`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor._packed_data), [`wake_up`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.wake_up), [`init`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.init), [`opt_param_scheduler`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.opt_param_scheduler), [`max_tokens_per_gpu`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.max_tokens_per_gpu), [`tokenizer`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.tokenizer), [`train_parallel_config`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_parallel_config), [`tokenizer`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.tokenizer), [`FSDPTrainRayActor`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor), [`hf_config`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.hf_config), [`pad_func`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.pad_func), [`connect_actor_critic`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.connect_actor_critic)  (+3 more)

## Functions
- `get_local_gpu_id()` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L20)

## Module values
- `logger` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/train_actor.py#L17)

