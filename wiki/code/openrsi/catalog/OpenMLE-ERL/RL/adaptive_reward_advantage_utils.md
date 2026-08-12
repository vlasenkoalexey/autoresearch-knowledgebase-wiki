---
title: 'Module: OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.adaptive_reward_advantage_utils`/
symbols:
  compute_adaptive_bound_pair: compute_adaptive_bound_pair().
  SUPPORTED_ADAPTIVE_BOUND_MODES: SUPPORTED_ADAPTIVE_BOUND_MODES.
  _finite: _finite().
  score_to_group_adaptive_reward: score_to_group_adaptive_reward().
  _sanitize_bound_pair: _sanitize_bound_pair().
  BOUND_MODE_THEORETICAL: BOUND_MODE_THEORETICAL.
  compute_ttt_entropic_advantages: compute_ttt_entropic_advantages().
  _solve_entropic_beta.kl_hat: _solve_entropic_beta().kl_hat().
  _solve_entropic_beta: _solve_entropic_beta().
  BOUND_MODE_TOP1_TOP8: BOUND_MODE_TOP1_TOP8.
  BOUND_MODE_TOP1_TOP16: BOUND_MODE_TOP1_TOP16.
  BOUND_MODE_TOP1_ALL_MEAN: BOUND_MODE_TOP1_ALL_MEAN.
  BOUND_MODE_TOP1_ALL_MEDIAN: BOUND_MODE_TOP1_ALL_MEDIAN.
  group_samples_by_group_index: group_samples_by_group_index().
  compute_gspo_group_advantages: compute_gspo_group_advantages().
---
# Module: [`OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py)

## Functions
- `_finite(value)` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L25)
- `_sanitize_bound_pair(best_signed: float | None, worst_signed: float | None, *, metadata: dict, min_span: float = 0.000001)` — [`L32`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L32)
- `_solve_entropic_beta(rewards: np.ndarray, *, target_kl: float, beta_max: float, iters: int)` — [`L182`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L182)
- `compute_adaptive_bound_pair(*, metadata: dict, historical_scores: Iterable[float], current_group_scores: Iterable[float], mode: str, min_span: float = 0.000001, lower_shift_ratio: float = 0)` — [`L60`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L60) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `compute_gspo_group_advantages(rewards: list[float], *, std_normalization: bool = True, eps: float = 0.000001)` — [`L166`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L166)
- `compute_ttt_entropic_advantages(rewards: list[float], *, target_kl: float = math.log(2), beta_max: float = 1000000, iters: int = 60, eps: float = 1e-12)` — [`L220`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L220)
- `group_samples_by_group_index(args, samples)` — [`L248`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L248)
- `kl_hat(beta_value: float)` — [`L197`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L197)
- `score_to_group_adaptive_reward(*, score: float | None, metadata: dict, historical_scores: Iterable[float], current_group_scores: Iterable[float], mode: str, reward_mapping_mode: str, use_score2reward: bool, default_reward: float = 0, min_span: float = 0.000001, lower_shift_ratio: float = 0, single_finite_reward_one: bool = False)` — [`L106`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L106) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)

## Module values
- `BOUND_MODE_THEORETICAL` — [`L14`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L14)
- `BOUND_MODE_TOP1_ALL_MEAN` — [`L12`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L12)
- `BOUND_MODE_TOP1_ALL_MEDIAN` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L13)
- `BOUND_MODE_TOP1_TOP16` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L11)
- `BOUND_MODE_TOP1_TOP8` — [`L10`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L10)
- `SUPPORTED_ADAPTIVE_BOUND_MODES` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/adaptive_reward_advantage_utils.py#L16)

