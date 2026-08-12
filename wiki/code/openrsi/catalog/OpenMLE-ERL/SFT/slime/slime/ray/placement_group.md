---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.placement_group`/
symbols:
  create_training_models: create_training_models().
  create_placement_groups: create_placement_groups().
  _create_placement_group: _create_placement_group().
  create_rollout_manager: create_rollout_manager().
  allocate_train_group: allocate_train_group().
  logger: logger.
  InfoActor: InfoActor#
  sort_key: sort_key().
  InfoActor.get_ip_and_gpu_id: InfoActor#get_ip_and_gpu_id().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py)

## Classes
### `InfoActor`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py:15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L15)
- signature: `class InfoActor:`
- members:
  - `get_ip_and_gpu_id(self)` — [`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L16)
- used by: [`_create_placement_group`](placement_group.md#_create_placement_group)

## Functions
- `_create_placement_group(num_gpus)` — [`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L41) — Create a placement group with the specified number of GPUs.
- `allocate_train_group(args, num_nodes, num_gpus_per_node, pg)` — [`L122`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L122)
- `create_placement_groups(args)` — [`L79`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L79) — Create placement groups for actor and rollout engines.
- `create_rollout_manager(args, pg)` — [`L174`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L174)
- `create_training_models(args, pgs, rollout_manager)` — [`L132`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L132)
- `sort_key(x)` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L20)

## Module values
- `logger` — [`L11`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/placement_group.py#L11)

