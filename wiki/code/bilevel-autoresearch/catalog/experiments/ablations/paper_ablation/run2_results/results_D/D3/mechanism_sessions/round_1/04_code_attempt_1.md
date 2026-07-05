---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D3.mechanism_sessions.round_1.04_code_attempt_1`/StaleProposalDetector#
symbols:
  StaleProposalDetector.record_outcome: record_outcome().
  StaleProposalDetector.reset: reset().
  StaleProposalDetector.record_proposal: record_proposal().
  StaleProposalDetector._last_proposed_params: _last_proposed_params.
  StaleProposalDetector._is_stale: _is_stale.
  StaleProposalDetector._discard_count: _discard_count.
  StaleProposalDetector.is_stale: is_stale().
  StaleProposalDetector.consecutive_discards_threshold: consecutive_discards_threshold.
  StaleProposalDetector.reset_on_any_accept: reset_on_any_accept.
  StaleProposalDetector.reset_on_parameter_change: reset_on_parameter_change.
  StaleProposalDetector: ''
  StaleProposalDetector.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `StaleProposalDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py:1`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L1)
- doc: Detects when the proposal stream is stuck in a discard loop.
- signature: `class StaleProposalDetector:`
- members:
  - `__init__(self, consecutive_discards_threshold: int = 3, reset_on_any_accept: bool = True, reset_on_parameter_change: bool = True)` — [`L10`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L10) — Args:
  - `is_stale(self)` — [`L71`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L71) — Returns True if the detector believes the proposal stream is stale
  - `record_outcome(self, accepted: bool)` — [`L54`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L54) — Update state based on whether the proposal was accepted or discarded.
  - `record_proposal(self, proposed_params: dict[str, float])` — [`L33`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L33) — Store the hyperparameters of the newly generated proposal.
  - `reset(self)` — [`L78`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L78) — Manually reset the detector (e.g., after a forced exploration move).
  - `consecutive_discards_threshold` — [`L25`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L25)
  - `reset_on_any_accept` — [`L26`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L26)
  - `reset_on_parameter_change` — [`L27`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L27)
- protocol/private: `_discard_count`[`L29`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L29), `_is_stale`[`L31`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L31), `_last_proposed_params`[`L30`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/04_code_attempt_1.py#L30)

