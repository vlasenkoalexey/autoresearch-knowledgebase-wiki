---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C3.mechanism_sessions.round_2.04_code_attempt_1`/OrthogonalExplorer#
symbols:
  OrthogonalExplorer._generate_orthogonal_samples: _generate_orthogonal_samples().
  OrthogonalExplorer.sample_index: sample_index.
  OrthogonalExplorer.record_visit: record_visit().
  OrthogonalExplorer._initialize_step_sizes: _initialize_step_sizes().
  OrthogonalExplorer.get_exploration_bonus: get_exploration_bonus().
  OrthogonalExplorer.get_orthogonal_sample: get_orthogonal_sample().
  OrthogonalExplorer.param_ranges: param_ranges.
  OrthogonalExplorer.param_visit_counts: param_visit_counts.
  OrthogonalExplorer.param_step_sizes: param_step_sizes.
  OrthogonalExplorer.orthogonal_samples: orthogonal_samples.
  OrthogonalExplorer.get_step_size: get_step_size().
  OrthogonalExplorer.n_samples: n_samples.
  OrthogonalExplorer.exploration_bonus_weight: exploration_bonus_weight.
  OrthogonalExplorer.decay_rate: decay_rate.
  OrthogonalExplorer: ''
  OrthogonalExplorer.__init__: __init__().
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py)

## Classes
### `OrthogonalExplorer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py:8`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L8)
- doc: Manages systematic exploration of hyperparameter space using orthogonal sampling.
- signature: `class OrthogonalExplorer:`
- members:
  - `__init__(self, param_ranges: Dict[str, Tuple[float, float]], n_samples: int = 8, exploration_bonus_weight: float = 0.3, decay_rate: float = 0.85)` — [`L11`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L11) — Args:
  - `_generate_orthogonal_samples(self)` — [`L78`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L78) — Generate Latin hypercube samples for systematic exploration.
  - `_initialize_step_sizes(self)` — [`L71`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L71) — Initialize step sizes based on parameter ranges.
  - `get_exploration_bonus(self, param_name: str)` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L39) — Calculate exploration bonus for a parameter based on visit frequency.
  - `get_orthogonal_sample(self)` — [`L62`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L62) — Get next orthogonal sample, or None if all used.
  - `get_step_size(self, param_name: str)` — [`L52`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L52) — Get exponentially decayed step size for parameter.
  - `record_visit(self, param_name: str)` — [`L56`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L56) — Record that a parameter was modified.
  - `decay_rate` — [`L28`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L28)
  - `exploration_bonus_weight` — [`L27`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L27)
  - `n_samples` — [`L26`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L26)
  - `orthogonal_samples` — [`L33`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L33)
  - `param_ranges` — [`L25`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L25)
  - `param_step_sizes` — [`L32`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L32)
  - `param_visit_counts` — [`L31`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L31)
  - `sample_index` — [`L34`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_2/04_code_attempt_1.py#L34)

