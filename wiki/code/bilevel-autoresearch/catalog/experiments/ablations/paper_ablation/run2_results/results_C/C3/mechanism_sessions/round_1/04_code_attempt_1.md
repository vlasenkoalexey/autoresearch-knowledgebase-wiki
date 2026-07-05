---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C3.mechanism_sessions.round_1.04_code_attempt_1`/BayesianOptimizer#
symbols:
  BayesianOptimizer.propose_next: propose_next().
  BayesianOptimizer._random_sample: _random_sample().
  BayesianOptimizer._params_to_features: _params_to_features().
  BayesianOptimizer.param_bounds: param_bounds.
  BayesianOptimizer.register_result: register_result().
  BayesianOptimizer._is_too_similar: _is_too_similar().
  BayesianOptimizer.consecutive_failures: consecutive_failures.
  BayesianOptimizer._features_to_params: _features_to_params().
  BayesianOptimizer.discrete_mapping: discrete_mapping.
  BayesianOptimizer.discrete_params: discrete_params.
  BayesianOptimizer.exploration_weight: exploration_weight.
  BayesianOptimizer.recent_attempts: recent_attempts.
  BayesianOptimizer.gp: gp.
  BayesianOptimizer._apply_llm_constraints: _apply_llm_constraints().
  BayesianOptimizer.X_scaler: X_scaler.
  BayesianOptimizer.y_scaler: y_scaler.
  BayesianOptimizer.init_samples: init_samples.
  BayesianOptimizer.max_consecutive_failures: max_consecutive_failures.
  BayesianOptimizer: ''
  BayesianOptimizer.__init__: __init__().
  BayesianOptimizer.history: history.
  BayesianOptimizer.param_names: param_names.
  BayesianOptimizer.llm_constraints: llm_constraints.
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py)

## Classes
### `BayesianOptimizer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py:19`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L19)
- doc: Bayesian optimization with constrained action space for hyperparameter tuning.
- signature: `class BayesianOptimizer:`
- members:
  - `__init__(self, param_bounds: Dict[str, Tuple[float, float]], discrete_params: Dict[str, List[float]], init_samples: int = 5, exploration_weight: float = 0.1, max_consecutive_failures: int = 3)` — [`L22`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L22) — Args:
  - `_apply_llm_constraints(self, params: Dict[str, Any], llm_insights: Optional[str])` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L129) — Apply penalty based on LLM insights.
  - `_features_to_params(self, features: np.ndarray)` — [`L89`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L89) — Convert feature vector back to params dict.
  - `_is_too_similar(self, params1: Dict[str, Any], params2: Dict[str, Any], threshold: float = 0.1)` — [`L162`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L162) — Check if two parameter sets are too similar.
  - `_params_to_features(self, params: Dict[str, Any])` — [`L63`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L63) — Convert params dict to feature vector.
  - `_random_sample(self)` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L115) — Generate random sample within bounds.
  - `propose_next(self, history: List[Dict[str, Any]], current_best: float, llm_insights: Optional[str] = None)` — [`L191`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L191) — Propose next hyperparameter configuration.
  - `register_result(self, params: Dict[str, Any], score: float, success: bool)` — [`L314`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L314) — Register the outcome of a proposed configuration.
  - `X_scaler` — [`L57`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L57)
  - `consecutive_failures` — [`L45`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L45)
  - `discrete_mapping` — [`L51`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L51)
  - `discrete_params` — [`L39`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L39)
  - `exploration_weight` — [`L41`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L41)
  - `gp` — [`L56`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L56)
  - `history` — [`L47`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L47)
  - `init_samples` — [`L40`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L40)
  - `llm_constraints` — [`L61`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L61)
  - `max_consecutive_failures` — [`L42`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L42)
  - `param_bounds` — [`L38`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L38)
  - `param_names` — [`L48`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L48)
  - `recent_attempts` — [`L46`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L46)
  - `y_scaler` — [`L58`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/04_code_attempt_1.py#L58)

