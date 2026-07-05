---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D3.mechanism_sessions.round_2.04_code_attempt_1`/StepSizeCalibrator#
symbols:
  StepSizeCalibrator.calibrate: calibrate().
  StepSizeCalibrator.step_size: step_size.
  StepSizeCalibrator.recent_results: recent_results.
  StepSizeCalibrator.get_step_size: get_step_size().
  StepSizeCalibrator.min_step: min_step.
  StepSizeCalibrator.max_step: max_step.
  StepSizeCalibrator.adaptation_window: adaptation_window.
  StepSizeCalibrator._calculate_step_magnitude: _calculate_step_magnitude().
  StepSizeCalibrator: ''
  StepSizeCalibrator.__init__: __init__().
  StepSizeCalibrator.last_config: last_config.
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py:1`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L1)
- signature: `class StepSizeCalibrator:`
- members:
  - `__init__(self, initial_step_size: float = 0.1, min_step: float = 0.01, max_step: float = 0.5, adaptation_window: int = 3)` — [`L2`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L2) — Args:
  - `_calculate_step_magnitude(self, old_config: Dict[str, Any], new_config: Dict[str, Any])` — [`L111`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L111) — Calculate the magnitude of change between two configurations.
  - `calibrate(self, current_bpb: float, new_bpb: float, current_config: Dict[str, Any], new_config: Dict[str, Any])` — [`L21`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L21) — Adjust step size based on performance of recent modifications.
  - `get_step_size(self)` — [`L107`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L107) — Return current step size.
  - `adaptation_window` — [`L15`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L15)
  - `last_config` — [`L19`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L19)
  - `max_step` — [`L14`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L14)
  - `min_step` — [`L13`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L13)
  - `recent_results` — [`L18`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L18)
  - `step_size` — [`L12`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_2/04_code_attempt_1.py#L12)

