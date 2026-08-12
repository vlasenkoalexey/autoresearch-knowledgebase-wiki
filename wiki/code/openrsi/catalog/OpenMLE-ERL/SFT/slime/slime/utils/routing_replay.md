---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.routing_replay`/
symbols:
  RoutingReplay: RoutingReplay#
  RoutingReplay.top_indices_list: RoutingReplay#top_indices_list.
  RoutingReplay.clear: RoutingReplay#clear().
  RoutingReplay.clear_all: RoutingReplay#clear_all().
  RoutingReplay.clear_all_forward: RoutingReplay#clear_all_forward().
  ROUTING_REPLAY: ROUTING_REPLAY.
  RoutingReplay.all_routing_replays: RoutingReplay#all_routing_replays.
  RoutingReplay.pop_forward: RoutingReplay#pop_forward().
  RoutingReplay.pop_backward: RoutingReplay#pop_backward().
  register_routing_replay: register_routing_replay().
  RoutingReplay.forward_index: RoutingReplay#forward_index.
  set_routing_replay: set_routing_replay().
  get_routing_replay_compute_topk.compute_topk: get_routing_replay_compute_topk().compute_topk().
  register_routing_replay.pre_forward_hook: register_routing_replay().pre_forward_hook().
  RoutingReplay.backward_index: RoutingReplay#backward_index.
  RoutingReplay.record: RoutingReplay#record().
  RoutingReplay.clear_forward: RoutingReplay#clear_forward().
  get_routing_replay_compute_topk: get_routing_replay_compute_topk().
  RoutingReplay.__init__: RoutingReplay#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py)

## Classes
### `RoutingReplay`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py:13`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L13)
- signature: `class RoutingReplay:`
- members:
  - `clear(self)` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L38)
  - `clear_all()` — [`L47`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L47)
  - `clear_all_forward()` — [`L52`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L52)
  - `clear_forward(self)` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L43)
  - `pop_backward(self)` — [`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L33)
  - `pop_forward(self)` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L28)
  - `record(self, top_indices)` — [`L22`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L22)
  - `all_routing_replays` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L14)
  - `backward_index` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L18)
  - `forward_index` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L17)
  - `top_indices_list` — [`L19`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L19)
- protocol/private: `__init__`[`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L16)
- used by: [`train_actor`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.train_actor), [`fill_routing_replay`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.fill_routing_replay), [`register_routing_replay`](routing_replay.md#register_routing_replay)

## Functions
- `compute_topk(scores, topk, num_groups=None, group_topk=None)` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L58)
- `get_routing_replay_compute_topk(old_compute_topk)` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L57)
- `pre_forward_hook(*args, **kwargs)` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L89)
- `register_routing_replay(module)` — [`L85`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L85)
- `set_routing_replay(replay)` — [`L8`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L8)

## Module values
- `ROUTING_REPLAY` — [`L5`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/routing_replay.py#L5)

