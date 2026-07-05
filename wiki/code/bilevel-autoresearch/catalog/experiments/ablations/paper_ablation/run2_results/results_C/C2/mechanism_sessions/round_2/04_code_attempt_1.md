---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C2.mechanism_sessions.round_2.04_code_attempt_1`/PostGenerationAdjuster#
symbols:
  PostGenerationAdjuster.adjust_proposal: adjust_proposal().
  PostGenerationAdjuster.should_adjust_param: should_adjust_param().
  PostGenerationAdjuster._calculate_adjustment_magnitude: _calculate_adjustment_magnitude().
  PostGenerationAdjuster._validate_and_bound: _validate_and_bound().
  PostGenerationAdjuster._get_adjustment_direction: _get_adjustment_direction().
  PostGenerationAdjuster._param_disable_count: _param_disable_count.
  PostGenerationAdjuster.get_adjustment_summary: get_adjustment_summary().
  PostGenerationAdjuster._clamp_to_bounds: _clamp_to_bounds().
  PostGenerationAdjuster.fallback_to_original: fallback_to_original.
  PostGenerationAdjuster.adjustment_history: adjustment_history.
  PostGenerationAdjuster.config: config.
  PostGenerationAdjuster.logger: logger.
  PostGenerationAdjuster.record_adjustment_performance: record_adjustment_performance().
  PostGenerationAdjuster.momentum_tracker: momentum_tracker.
  PostGenerationAdjuster.step_calibrator: step_calibrator.
  PostGenerationAdjuster.elite_pool: elite_pool.
  PostGenerationAdjuster.adjustment_enabled: adjustment_enabled.
  PostGenerationAdjuster.max_relative_adjustment: max_relative_adjustment.
  PostGenerationAdjuster._allowlist: _allowlist.
  PostGenerationAdjuster: ''
  PostGenerationAdjuster.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `PostGenerationAdjuster`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py:10`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L10)
- doc: Adjusts LLM-generated parameter proposals based on momentum, elite pool patterns,
- signature: `class PostGenerationAdjuster:`
- members:
  - `__init__(self, momentum_tracker, step_calibrator, elite_pool, config, adjustment_enabled: bool = True, fallback_to_original: bool = True, max_relative_adjustment: float = 0.2)` — [`L20`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L20) — Args:
  - `_calculate_adjustment_magnitude(self, param_name: str, proposed_value: float, direction: int)` — [`L194`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L194) — Calculate the adjustment magnitude based on step size and constraints.
  - `_clamp_to_bounds(self, param_name: str, value: float)` — [`L250`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L250) — Clamp value to parameter bounds.
  - `_get_adjustment_direction(self, param_name: str, proposed_value: float)` — [`L163`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L163) — Determine adjustment direction (1 for increase, -1 for decrease, 0 for none).
  - `_validate_and_bound(self, param_name: str, proposed_value: float, adjusted_value: float)` — [`L216`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L216) — Validate adjusted value and apply bounds if necessary.
  - `adjust_proposal(self, param_name: str, proposed_value: float, current_value: Optional[float], param_type: str = "continuous", iteration: int = 0)` — [`L57`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L57) — Adjust a single proposed parameter value based on momentum and calibration.
  - `get_adjustment_summary(self)` — [`L275`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L275) — Generate a summary of adjustments for debugging.
  - `record_adjustment_performance(self, param_name: str, original_bpb: float, adjusted_bpb: float)` — [`L266`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L266) — Record performance of adjustment to potentially disable poorly performing parameters.
  - `should_adjust_param(self, param_name: str)` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L129) — Determine if parameter should be adjusted.
  - `adjustment_enabled` — [`L44`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L44)
  - `adjustment_history` — [`L52`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L52)
  - `config` — [`L43`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L43)
  - `elite_pool` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L42)
  - `fallback_to_original` — [`L45`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L45)
  - `logger` — [`L55`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L55)
  - `max_relative_adjustment` — [`L46`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L46)
  - `momentum_tracker` — [`L40`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L40)
  - `step_calibrator` — [`L41`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L41)
- protocol/private: `_allowlist`[`L49`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L49), `_param_disable_count`[`L53`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/04_code_attempt_1.py#L53)

