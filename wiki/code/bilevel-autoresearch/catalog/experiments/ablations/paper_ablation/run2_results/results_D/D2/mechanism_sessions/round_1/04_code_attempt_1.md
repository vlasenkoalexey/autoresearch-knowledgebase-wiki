---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D2.mechanism_sessions.round_1.04_code_attempt_1`/GeneratedMechanism_20260324_142015#
symbols:
  GeneratedMechanism_20260324_142015._detect_phase_transition: _detect_phase_transition().
  GeneratedMechanism_20260324_142015.update: update().
  GeneratedMechanism_20260324_142015.get_specialized_instructions: get_specialized_instructions().
  GeneratedMechanism_20260324_142015.discard_patterns: discard_patterns.
  GeneratedMechanism_20260324_142015.history: history.
  GeneratedMechanism_20260324_142015.phase: phase.
  GeneratedMechanism_20260324_142015._update_discard_patterns: _update_discard_patterns().
  GeneratedMechanism_20260324_142015._is_significant_improvement: _is_significant_improvement().
  GeneratedMechanism_20260324_142015._get_recent_discard_summary: _get_recent_discard_summary().
  GeneratedMechanism_20260324_142015.iterations_in_current_phase: iterations_in_current_phase.
  GeneratedMechanism_20260324_142015.improvements_in_phase: improvements_in_phase.
  GeneratedMechanism_20260324_142015.stagnation_window: stagnation_window.
  GeneratedMechanism_20260324_142015._get_stagnation_instructions: _get_stagnation_instructions().
  GeneratedMechanism_20260324_142015._get_pattern_warnings: _get_pattern_warnings().
  GeneratedMechanism_20260324_142015.last_phase_change: last_phase_change.
  GeneratedMechanism_20260324_142015.get_phase: get_phase().
  GeneratedMechanism_20260324_142015.min_improvement: min_improvement.
  GeneratedMechanism_20260324_142015._param_categories: _param_categories.
  GeneratedMechanism_20260324_142015._get_exploration_instructions: _get_exploration_instructions().
  GeneratedMechanism_20260324_142015._get_exploitation_instructions: _get_exploitation_instructions().
  GeneratedMechanism_20260324_142015: ''
  GeneratedMechanism_20260324_142015.__init__: __init__().
  GeneratedMechanism_20260324_142015.exploration_window: exploration_window.
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `GeneratedMechanism_20260324_142015`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py:9`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L9)
- doc: Adaptive Prompt Specializer: Dynamically adjusts LLM instructions based on
- signature: `class GeneratedMechanism_20260324_142015:`
- members:
  - `__init__(self, stagnation_window: int = 4, exploration_window: int = 3, min_improvement_threshold: float = 0.0003)` — [`L15`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L15) — Args:
  - `_detect_phase_transition(self, current_iteration: int)` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L118) — Determine current optimization phase based on recent history.
  - `_get_pattern_warnings(self)` — [`L231`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L231) — Generate warnings about repeated failure patterns.
  - `_get_recent_discard_summary(self)` — [`L217`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L217) — Get summary of recently failed parameters.
  - `_is_significant_improvement(self, recent_best: float)` — [`L159`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L159) — Check if recent improvement is significant compared to history.
  - `_update_discard_patterns(self, iteration: int, config: dict, discard_reason: str)` — [`L85`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L85) — Track patterns in failed parameter changes.
  - `get_phase(self)` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L256) — Return current phase: 'exploration', 'exploitation', or 'stagnation'.
  - `get_specialized_instructions(self)` — [`L175`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L175) — Return specialized prompt instructions based on current phase.
  - `update(self, iteration: int, result: Any, current_config: dict)` — [`L59`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L59) — Update internal state with latest iteration results.
  - `discard_patterns` — [`L37`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L37)
  - `exploration_window` — [`L28`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L28)
  - `history` — [`L32`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L32)
  - `improvements_in_phase` — [`L44`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L44)
  - `iterations_in_current_phase` — [`L43`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L43)
  - `last_phase_change` — [`L34`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L34)
  - `min_improvement` — [`L29`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L29)
  - `phase` — [`L33`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L33)
  - `stagnation_window` — [`L27`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L27)
- protocol/private: `_get_exploitation_instructions`[`L201`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L201), `_get_exploration_instructions`[`L194`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L194), `_get_stagnation_instructions`[`L208`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L208), `_param_categories`[`L47`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/04_code_attempt_1.py#L47)

