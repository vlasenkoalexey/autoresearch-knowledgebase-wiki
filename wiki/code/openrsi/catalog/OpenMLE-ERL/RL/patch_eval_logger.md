---
title: 'Module: OpenMLE-ERL/RL/patch_eval_logger.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/patch_eval_logger.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.patch_eval_logger`/
symbols:
  custom_log_eval_rollout_data: custom_log_eval_rollout_data().
  get_medal_for_score.get_score_at_position: get_medal_for_score().get_score_at_position().
  test_medal_statistics_integration: test_medal_statistics_integration().
  get_medal_for_score: get_medal_for_score().
  _to_finite_float: _to_finite_float().
  _log_quality_proxy_metrics: _log_quality_proxy_metrics().
  _build_mode_bucket: _build_mode_bucket().
  load_public_leaderboard: load_public_leaderboard().
  apply_patch: apply_patch().
  test2_passed: test2_passed.
  SCRIPT_DIR: SCRIPT_DIR.
  _has_static_bounds: _has_static_bounds().
  get_medal_for_score.get_thresholds: get_medal_for_score().get_thresholds().
  REWARD_VIEW_KEYS: REWARD_VIEW_KEYS.
  LEADERBOARD_PTH: LEADERBOARD_PTH.
  _log_reward_view_means: _log_reward_view_means().
  is_lower_better: is_lower_better().
  apply_patch.eval_with_log_dict: apply_patch().eval_with_log_dict().
  DEFAULT_LEADERBOARD_ROOTS.DEFAULT_LEADERBOARD_ROOTS: DEFAULT_LEADERBOARD_ROOTS.DEFAULT_LEADERBOARD_ROOTS.
---
# Module: [`OpenMLE-ERL/RL/patch_eval_logger.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py)

## Functions
- `_build_mode_bucket()` — [`L43`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L43)
- `_has_static_bounds(metadata)` — [`L58`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L58)
- `_log_quality_proxy_metrics(log_dict, prefix, samples)` — [`L91`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L91)
- `_log_reward_view_means(log_dict, prefix, reward_views)` — [`L79`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L79)
- `_to_finite_float(value)` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L31)
- `apply_patch()` — [`L635`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L635) — Apply monkey patch to _log_eval_rollout_data
- `custom_log_eval_rollout_data(rollout_id, args, data, extra_metrics=None)` — [`L257`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L257) — Extended eval logger with custom metrics for MLE-Agent.
- `eval_with_log_dict(self, rollout_id)` — [`L645`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L645)
- `get_medal_for_score(score: float | None, leaderboard: pd.DataFrame)` — [`L161`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L161) — Determine the medal level for a score using the leaderboard.
- `get_score_at_position(position: int)` — [`L179`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L179)
- `get_thresholds(num_teams: int)` — [`L184`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L184) — Return the gold, silver, and bronze score thresholds.
- `is_lower_better(leaderboard: pd.DataFrame)` — [`L150`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L150) — Determine from the leaderboard whether lower scores are better.
- `load_public_leaderboard(task_name: str)` — [`L228`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L228)
- `test_medal_statistics_integration()` — [`L673`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L673) — Integration test for medal statistics with simulated samples

## Module values
- `DEFAULT_LEADERBOARD_ROOTS` — [`L23`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L23)
- `LEADERBOARD_PTH` — [`L24`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L24)
- `REWARD_VIEW_KEYS` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L25)
- `SCRIPT_DIR` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L19)
- `test2_passed` — [`L854`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/patch_eval_logger.py#L854)

