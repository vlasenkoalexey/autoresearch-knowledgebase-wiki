---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C1.mechanism_sessions.round_2.04_code_attempt_1`/
symbols:
  PhaseDetector.update_and_detect: PhaseDetector#update_and_detect().
  PhaseDetector.improvement_streak: PhaseDetector#improvement_streak.
  PhaseDetector.plateau_counter: PhaseDetector#plateau_counter.
  PhaseDetector.non_improvement_streak: PhaseDetector#non_improvement_streak.
  PhaseDetector.min_improvement: PhaseDetector#min_improvement.
  PhaseDetector.last_best_bpb: PhaseDetector#last_best_bpb.
  PhaseDetector.exploration_window: PhaseDetector#exploration_window.
  PhaseDetector.exploitation_window: PhaseDetector#exploitation_window.
  PhaseDetector.stagnation_threshold: PhaseDetector#stagnation_threshold.
  PhaseDetector: PhaseDetector#
  PhaseDetector.__init__: PhaseDetector#__init__().
  _build_proposal_prompt: _build_proposal_prompt().
  get_phase_summary: get_phase_summary().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `PhaseDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py:1`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L1)
- doc: Detects optimization phases based on performance trends.
- signature: `class PhaseDetector:`
- members:
  - `__init__(self, exploration_window: int = 3, exploitation_window: int = 4, stagnation_threshold: int = 3, min_improvement: float = 0.0003)` — [`L4`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L4) — Args:
  - `update_and_detect(self, iteration: int, current_bpb: float)` — [`L29`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L29) — Update internal state and return current phase.
  - `exploitation_window` — [`L19`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L19)
  - `exploration_window` — [`L18`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L18)
  - `improvement_streak` — [`L24`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L24)
  - `last_best_bpb` — [`L27`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L27)
  - `min_improvement` — [`L21`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L21)
  - `non_improvement_streak` — [`L25`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L25)
  - `plateau_counter` — [`L26`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L26)
  - `stagnation_threshold` — [`L20`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L20)

## Functions
- `_build_proposal_prompt(self, current_config: dict[str, any], iteration: int, phase: str)` — [`L67`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L67) — Build phase-aware prompt for LLM proposals.
- `get_phase_summary(self)` — [`L182`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/mechanism_sessions/round_2/04_code_attempt_1.py#L182) — Return phase detection state for debugging.

