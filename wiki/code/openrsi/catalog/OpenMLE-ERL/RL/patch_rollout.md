---
title: 'Module: OpenMLE-ERL/RL/patch_rollout.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/patch_rollout.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.patch_rollout`/
symbols:
  patched_log_rollout_data: patched_log_rollout_data().
  _to_finite_float: _to_finite_float().
  _log_quality_proxy_metrics: _log_quality_proxy_metrics().
  _build_mode_bucket: _build_mode_bucket().
  apply_patch: apply_patch().
  _has_static_bounds: _has_static_bounds().
  _log_reward_view_means: _log_reward_view_means().
  REWARD_VIEW_KEYS: REWARD_VIEW_KEYS.
  _mean_or_none: _mean_or_none().
  patched_save_db_snapshot: patched_save_db_snapshot().
  _compute_debug_rewards: _compute_debug_rewards().
  QUALITY_PROXY_KEYS: QUALITY_PROXY_KEYS.
---
# Module: [`OpenMLE-ERL/RL/patch_rollout.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py)

## Functions
- `_build_mode_bucket()` — [`L65`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L65)
- `_compute_debug_rewards(args, samples)` — [`L149`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L149)
- `_has_static_bounds(metadata)` — [`L44`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L44)
- `_log_quality_proxy_metrics(log_dict, prefix, samples)` — [`L90`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L90)
- `_log_reward_view_means(log_dict, prefix, reward_views)` — [`L78`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L78)
- `_mean_or_none(values)` — [`L40`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L40)
- `_to_finite_float(value)` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L28)
- `apply_patch()` — [`L363`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L363) — Apply monkey patch to rollout internals.
- `patched_log_rollout_data(rollout_id, args, samples, rollout_extra_metrics, rollout_time)` — [`L204`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L204)
- `patched_save_db_snapshot(self, rollout_id)` — [`L179`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L179) — Save a snapshot of the program database if enabled.

## Module values
- `QUALITY_PROXY_KEYS` — [`L21`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L21)
- `REWARD_VIEW_KEYS` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_rollout.py#L16)

