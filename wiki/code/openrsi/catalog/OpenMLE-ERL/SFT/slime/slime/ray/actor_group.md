---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.actor_group`/RayTrainGroup#
symbols:
  RayTrainGroup._allocate_gpus_for_actor: _allocate_gpus_for_actor().
  RayTrainGroup._actor_handlers: _actor_handlers.
  RayTrainGroup.async_train: async_train().
  RayTrainGroup.async_init: async_init().
  RayTrainGroup.save_model: save_model().
  RayTrainGroup.update_weights: update_weights().
  RayTrainGroup.args: args.
  RayTrainGroup.offload: offload().
  RayTrainGroup.role: role.
  RayTrainGroup.clear_memory: clear_memory().
  RayTrainGroup.connect: connect().
  RayTrainGroup.set_rollout_manager: set_rollout_manager().
  RayTrainGroup.onload: onload().
  RayTrainGroup: ''
  RayTrainGroup._num_nodes: _num_nodes.
  RayTrainGroup._num_gpus_per_node: _num_gpus_per_node.
  RayTrainGroup.__init__: __init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py)

## Classes
### `RayTrainGroup`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py:10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L10)
- doc: A group of ray actors
- signature: `class RayTrainGroup:`
- members:
  - `async_init(self, args, role, with_ref=False, with_opd_teacher=False)` — [`L108`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L108) — Allocate GPU resourced and initialize model, optimzier, local ckpt, etc.
  - `async_train(self, rollout_id, rollout_data_ref)` — [`L118`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L118) — Do one rollout training
  - `clear_memory(self)` — [`L136`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L136)
  - `connect(self, critic_group)` — [`L139`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L139)
  - `offload(self)` — [`L133`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L133)
  - `onload(self)` — [`L130`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L130)
  - `save_model(self, rollout_id, force_sync=False)` — [`L122`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L122) — Save actor model
  - `set_rollout_manager(self, rollout_manager)` — [`L147`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L147)
  - `update_weights(self)` — [`L126`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L126) — Broadcast weights from rank 0 to all other ranks.
  - `args` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L38)
  - `role` — [`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L41)
- protocol/private: `__init__`[`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L29), `_actor_handlers`[`L93`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L93), `_allocate_gpus_for_actor`[`L46`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L46), `_num_gpus_per_node`[`L40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L40), `_num_nodes`[`L39`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/actor_group.py#L39)
- uses (calls/refs, reference-scoped): [`FSDPTrainRayActor`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor), [`NOSET_VISIBLE_DEVICES_ENV_VARS_LIST`](utils.md#NOSET_VISIBLE_DEVICES_ENV_VARS_LIST), [`MegatronTrainRayActor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor)
- used by: [`train`](../../train.md#train), [`train`](../../train_async.md#train), [`create_training_models`](placement_group.md#create_training_models), [`offload_train`](../../train.md#train.offload_train), [`allocate_train_group`](placement_group.md#allocate_train_group), [`save`](../../train.md#train.save)

