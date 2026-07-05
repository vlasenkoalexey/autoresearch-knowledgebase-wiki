---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D1.mechanism_sessions.round_2.04_code_attempt_1`/FixationDetector#
symbols:
  FixationDetector.proposal_history: proposal_history.
  FixationDetector.check_fixation: check_fixation().
  FixationDetector.add_proposal: add_proposal().
  FixationDetector.get_intervention_suggestion: get_intervention_suggestion().
  FixationDetector.reset: reset().
  FixationDetector._identify_fixated_parameter: _identify_fixated_parameter().
  FixationDetector.fixation_counter: fixation_counter.
  FixationDetector.window_size: window_size.
  FixationDetector.iteration_history: iteration_history.
  FixationDetector._detect_directional_pattern: _detect_directional_pattern().
  FixationDetector.similarity_threshold: similarity_threshold.
  FixationDetector.max_repetitions: max_repetitions.
  FixationDetector._clean_proposal: _clean_proposal().
  FixationDetector._jaccard_similarity: _jaccard_similarity().
  FixationDetector: ''
  FixationDetector.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `FixationDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py:5`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L5)
- doc: Detects when the LLM is stuck proposing similar parameter changes repeatedly.
- signature: `class FixationDetector:`
- members:
  - `__init__(self, window_size: int = 5, similarity_threshold: float = 0.7, max_repetitions: int = 3)` — [`L9`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L9) — window_size: How many recent proposals to track
  - `_clean_proposal(self, proposal_text: str)` — [`L112`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L112) — Clean proposal text and extract parameter changes
  - `_detect_directional_pattern(self)` — [`L193`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L193) — Detect if proposals show a consistent directional pattern
  - `_identify_fixated_parameter(self)` — [`L171`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L171) — Identify the most common parameter in recent proposals
  - `_jaccard_similarity(self, text1: str, text2: str)` — [`L156`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L156) — Compute Jaccard similarity between two texts based on tokens
  - `add_proposal(self, proposal_text: str, iteration: int)` — [`L28`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L28) — Record a new proposal for analysis
  - `check_fixation(self)` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L39) — Returns:
  - `get_intervention_suggestion(self)` — [`L78`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L78) — Returns a concrete suggestion to break the fixation pattern
  - `reset(self)` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L106) — Clear history after successful intervention
  - `fixation_counter` — [`L26`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L26)
  - `iteration_history` — [`L25`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L25)
  - `max_repetitions` — [`L22`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L22)
  - `proposal_history` — [`L24`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L24)
  - `similarity_threshold` — [`L21`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L21)
  - `window_size` — [`L20`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/04_code_attempt_1.py#L20)

