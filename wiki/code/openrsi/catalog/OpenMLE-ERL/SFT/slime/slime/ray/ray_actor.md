---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.ray_actor`/RayActor#
symbols:
  RayActor: ''
  RayActor._get_current_node_ip_and_free_port: _get_current_node_ip_and_free_port().
  RayActor.get_master_addr_and_port: get_master_addr_and_port().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py)

## Classes
### `RayActor`
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py:4`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py#L4)
- signature: `class RayActor:`
- members:
  - `get_master_addr_and_port(self)` — [`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py#L9)
- protocol/private: `_get_current_node_ip_and_free_port`[`L6`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/ray_actor.py#L6)
- uses (calls/refs, reference-scoped): [`TrainRayActor`](train_actor.md#TrainRayActor), [`Lock`](utils.md#Lock), [`SGLangEngine`](../backends/sglang_utils/sglang_engine.md#SGLangEngine), [`get_free_port`](../utils/misc.md#get_free_port), [`get_current_node_ip`](../utils/misc.md#get_current_node_ip)
- used by: [`master_port`](train_actor.md#TrainRayActor.master_port), [`TrainRayActor`](train_actor.md#TrainRayActor), [`Lock`](utils.md#Lock), [`SGLangEngine`](../backends/sglang_utils/sglang_engine.md#SGLangEngine)

