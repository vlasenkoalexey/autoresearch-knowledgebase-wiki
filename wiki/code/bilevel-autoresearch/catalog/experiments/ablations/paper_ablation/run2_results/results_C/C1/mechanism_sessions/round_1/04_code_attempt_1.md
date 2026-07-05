---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C1.mechanism_sessions.round_1.04_code_attempt_1`/TabuSearchManager#
symbols:
  TabuSearchManager.add_tabu_entry: add_tabu_entry().
  TabuSearchManager.tabu_list: tabu_list.
  TabuSearchManager.update_distance_thresholds: update_distance_thresholds().
  TabuSearchManager.is_tabu: is_tabu().
  TabuSearchManager.get_suggested_alternatives: get_suggested_alternatives().
  TabuSearchManager.distance_thresholds: distance_thresholds.
  TabuSearchManager.max_tabu_size: max_tabu_size.
  TabuSearchManager.tabu_tenure: tabu_tenure.
  TabuSearchManager.enable_adaptive_thresholds: enable_adaptive_thresholds.
  TabuSearchManager.iteration_history: iteration_history.
  TabuSearchManager.logger: logger.
  TabuSearchManager: ''
  TabuSearchManager.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `TabuSearchManager`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py:11`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L11)
- doc: Manages tabu lists to prevent revisiting recently explored parameter regions.
- signature: `class TabuSearchManager:`
- members:
  - `__init__(self, max_tabu_size: int = 10, tabu_tenure: int = 3, distance_thresholds: Optional[dict[str, float]] = None, enable_adaptive_thresholds: bool = True)` — [`L14`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L14) — Args:
  - `add_tabu_entry(self, config: dict[str, Any], iteration: int, reason: str = "explored")` — [`L75`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L75) — Add a configuration to the tabu list.
  - `get_suggested_alternatives(self, current_config: dict[str, Any], param_ranges: dict[str, tuple[float, float]])` — [`L168`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L168) — Suggest alternative values for parameters that are currently tabu.
  - `is_tabu(self, config: dict[str, Any], current_iteration: int)` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L42) — Check if a configuration is tabu (forbidden).
  - `update_distance_thresholds(self, elite_configs: list[dict[str, Any]], current_iteration: int)` — [`L104`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L104) — Adaptively update distance thresholds based on elite configurations.
  - `distance_thresholds` — [`L30`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L30)
  - `enable_adaptive_thresholds` — [`L37`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L37)
  - `iteration_history` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L39)
  - `logger` — [`L40`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L40)
  - `max_tabu_size` — [`L28`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L28)
  - `tabu_list` — [`L38`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L38)
  - `tabu_tenure` — [`L29`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_1/04_code_attempt_1.py#L29)

