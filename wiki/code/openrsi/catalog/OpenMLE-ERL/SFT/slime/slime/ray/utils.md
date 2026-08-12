---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/ray/utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/ray/utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.ray.utils`/
symbols:
  NOSET_VISIBLE_DEVICES_ENV_VARS_LIST: NOSET_VISIBLE_DEVICES_ENV_VARS_LIST.
  Lock: Lock#
  Lock._locked: Lock#_locked.
  ray_noset_visible_devices: ray_noset_visible_devices().
  Lock.acquire: Lock#acquire().
  Lock.release: Lock#release().
  get_physical_gpu_id: get_physical_gpu_id().
  Lock.__init__: Lock#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/ray/utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py)

## Classes
### `Lock`  ·  implements/extends RayActor
- def: [`OpenMLE-ERL/SFT/slime/slime/ray/utils.py:39`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L39)
- signature: `class Lock(RayActor):`
- members:
  - `acquire(self)` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L43) — Try to acquire the lock. Returns True if acquired, False otherwise.
  - `release(self)` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L53) — Release the lock, allowing others to acquire.
- protocol/private: `__init__`[`L40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L40), `_locked`[`L41`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L41)
- uses (calls/refs, reference-scoped): [`RayActor`](ray_actor.md#RayActor)
- used by: [`RayActor`](ray_actor.md#RayActor), [`rollout_engine_lock`](rollout.md#RolloutManager.rollout_engine_lock)

## Functions
- `get_physical_gpu_id()` — [`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L32)
- `ray_noset_visible_devices(env_vars=os.environ)` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L28)

## Module values
- `NOSET_VISIBLE_DEVICES_ENV_VARS_LIST` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/ray/utils.py#L17)

