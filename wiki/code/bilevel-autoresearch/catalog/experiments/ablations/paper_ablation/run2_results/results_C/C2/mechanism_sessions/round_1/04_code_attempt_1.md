---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C2.mechanism_sessions.round_1.04_code_attempt_1`/MultiScaleBanditProposer#
symbols:
  MultiScaleBanditProposer.select_scale: select_scale().
  MultiScaleBanditProposer.update_reward: update_reward().
  MultiScaleBanditProposer.get_stats: get_stats().
  MultiScaleBanditProposer.visit_counts: visit_counts.
  MultiScaleBanditProposer.q_values: q_values.
  MultiScaleBanditProposer.get_scale_parameters: get_scale_parameters().
  MultiScaleBanditProposer.total_visits: total_visits.
  MultiScaleBanditProposer.scale_levels: scale_levels.
  MultiScaleBanditProposer.initial_exploration_bias: initial_exploration_bias.
  MultiScaleBanditProposer.exploration_decay: exploration_decay.
  MultiScaleBanditProposer.min_exploration: min_exploration.
  MultiScaleBanditProposer.scale_parameters: scale_parameters.
  MultiScaleBanditProposer: ''
  MultiScaleBanditProposer.__init__: __init__().
  MultiScaleBanditProposer.optimistic_init_value: optimistic_init_value.
  MultiScaleBanditProposer._calculate_information_gain: _calculate_information_gain().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `MultiScaleBanditProposer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py:14`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L14)
- doc: Bandit system for selecting proposal scales based on information gain.
- signature: `class MultiScaleBanditProposer:`
- members:
  - `__init__(self, scale_levels: list[str] = None, initial_exploration_bias: float = 0.7, exploration_decay: float = 0.95, min_exploration: float = 0.1, optimistic_init_value: float = 2)` — [`L17`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L17) — Args:
  - `_calculate_information_gain(self, scale_level: str, was_accepted: bool, performance_change: float = None)` — [`L133`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L133) — Calculate information gain metric (0-1).
  - `get_scale_parameters(self, scale_level: str)` — [`L126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L126) — Get mutation parameters for a given scale level.
  - `get_stats(self)` — [`L156`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L156) — Return current bandit statistics for debugging.
  - `select_scale(self, current_config: dict, iteration: int, recent_performance: list[float] = None)` — [`L53`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L53) — Select a scale level for the next proposal.
  - `update_reward(self, scale_level: str, was_accepted: bool, information_gain: float, performance_change: float = None)` — [`L88`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L88) — Update bandit Q-values based on outcome.
  - `exploration_decay` — [`L37`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L37)
  - `initial_exploration_bias` — [`L36`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L36)
  - `min_exploration` — [`L38`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L38)
  - `optimistic_init_value` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L39)
  - `q_values` — [`L41`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L41)
  - `scale_levels` — [`L35`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L35)
  - `scale_parameters` — [`L45`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L45)
  - `total_visits` — [`L43`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L43)
  - `visit_counts` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_1/04_code_attempt_1.py#L42)

