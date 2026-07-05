---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D2.mechanism_sessions.round_2.04_code_attempt_1`/TrustRegionConstraint#
symbols:
  TrustRegionConstraint.update_region: update_region().
  TrustRegionConstraint.constrain_proposal: constrain_proposal().
  TrustRegionConstraint.get_region_status: get_region_status().
  TrustRegionConstraint.radii: radii.
  TrustRegionConstraint.reset_region: reset_region().
  TrustRegionConstraint.history: history.
  TrustRegionConstraint.initial_radii: initial_radii.
  TrustRegionConstraint.logger: logger.
  TrustRegionConstraint.min_radius: min_radius.
  TrustRegionConstraint.max_radius: max_radius.
  TrustRegionConstraint.success_count: success_count.
  TrustRegionConstraint.total_updates: total_updates.
  TrustRegionConstraint.bounded_params: bounded_params.
  TrustRegionConstraint.contraction_factor: contraction_factor.
  TrustRegionConstraint.expansion_factor: expansion_factor.
  TrustRegionConstraint.success_threshold: success_threshold.
  TrustRegionConstraint.log_scale_params: log_scale_params.
  TrustRegionConstraint: ''
  TrustRegionConstraint.__init__: __init__().
  TrustRegionConstraint.window_size: window_size.
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `TrustRegionConstraint`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py:15`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L15)
- doc: Manages trust regions for hyperparameter exploration.
- signature: `class TrustRegionConstraint:`
- members:
  - `__init__(self, initial_radii: Dict[str, float], contraction_factor: float = 0.8, expansion_factor: float = 1.2, min_radius: Optional[Dict[str, float]] = None, max_radius: Optional[Dict[str, float]] = None, success_threshold: float = 0, window_size: int = 3)` — [`L18`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L18) — Args:
  - `constrain_proposal(self, current_params: Dict[str, float], proposed_params: Dict[str, float])` — [`L59`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L59) — Clip proposed parameters to stay within trust region of current best.
  - `get_region_status(self)` — [`L139`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L139) — Return current radii and success statistics for logging.
  - `reset_region(self, param: Optional[str] = None)` — [`L153`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L153) — Reset trust region for specific parameter or all parameters.
  - `update_region(self, current_params: Dict[str, float], new_params: Dict[str, float], improvement: float, iteration: int)` — [`L95`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L95) — Update trust radii based on success/failure of last step.
  - `bounded_params` — [`L54`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L54)
  - `contraction_factor` — [`L41`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L41)
  - `expansion_factor` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L42)
  - `history` — [`L48`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L48)
  - `initial_radii` — [`L40`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L40)
  - `log_scale_params` — [`L53`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L53)
  - `logger` — [`L51`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L51)
  - `max_radius` — [`L44`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L44)
  - `min_radius` — [`L43`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L43)
  - `radii` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L39)
  - `success_count` — [`L49`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L49)
  - `success_threshold` — [`L45`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L45)
  - `total_updates` — [`L50`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L50)
  - `window_size` — [`L46`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/04_code_attempt_1.py#L46)

