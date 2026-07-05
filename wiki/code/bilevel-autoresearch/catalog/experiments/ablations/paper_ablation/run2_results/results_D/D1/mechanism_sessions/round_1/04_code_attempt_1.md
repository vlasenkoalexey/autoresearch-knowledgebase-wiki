---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D1.mechanism_sessions.round_1.04_code_attempt_1`/DiversityEnforcer#
symbols:
  DiversityEnforcer.enforce_diversity: enforce_diversity().
  DiversityEnforcer._normalize_config: _normalize_config().
  DiversityEnforcer.min_distance_threshold: min_distance_threshold.
  DiversityEnforcer.PARAM_BOUNDS: PARAM_BOUNDS.
  DiversityEnforcer._compute_distance: _compute_distance().
  DiversityEnforcer.CATEGORICAL_OPTIONS: CATEGORICAL_OPTIONS.
  DiversityEnforcer.history_window: history_window.
  DiversityEnforcer.max_retries: max_retries.
  DiversityEnforcer.logger: logger.
  DiversityEnforcer._perturb_parameter: _perturb_parameter().
  DiversityEnforcer: ''
  DiversityEnforcer.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `DiversityEnforcer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py:8`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L8)
- doc: Enforces diversity in hyperparameter proposals to avoid repetitive configurations.
- signature: `class DiversityEnforcer:`
- members:
  - `__init__(self, history_window: int = 5, min_distance_threshold: float = 0.3, max_retries: int = 3)` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L42) — Args:
  - `_compute_distance(self, norm_vec1: Dict[str, float], norm_vec2: Dict[str, float])` — [`L272`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L272) — Compute Euclidean distance between two normalized vectors.
  - `_normalize_config(self, config: Dict[str, Any])` — [`L204`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L204) — Normalize a configuration to [0,1] range.
  - `_perturb_parameter(self, param_name: str, original_value: Any, param_type: str, bounds: Optional[Tuple[float, float]], options: Optional[List[str]], norm_value: float, norm_closest: Optional[float])` — [`L288`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L288) — Apply targeted perturbation to a parameter.
  - `enforce_diversity(self, proposed_config: Dict[str, Any], recent_configs: List[Dict[str, Any]], iteration: int)` — [`L59`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L59) — Check if proposed config is sufficiently diverse from recent history.
  - `CATEGORICAL_OPTIONS` — [`L35`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L35)
  - `PARAM_BOUNDS` — [`L14`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L14)
  - `history_window` — [`L54`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L54)
  - `logger` — [`L57`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L57)
  - `max_retries` — [`L56`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L56)
  - `min_distance_threshold` — [`L55`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/04_code_attempt_1.py#L55)

