---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C3.mechanism_sessions.round_1.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  BayesianOptimizer.propose_next: BayesianOptimizer#propose_next().
  CrashMemory.record: CrashMemory#record().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  TrainRunner.search_config: TrainRunner#search_config.
  ElitePool._pool: ElitePool#_pool.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  CrashMemory.get_warning_text: CrashMemory#get_warning_text().
  PlateauDetector.check_plateau: PlateauDetector#check_plateau().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  BayesianOptimizer._random_sample: BayesianOptimizer#_random_sample().
  BayesianOptimizer._params_to_features: BayesianOptimizer#_params_to_features().
  TrainResult.status: TrainResult#status.
  MomentumTracker.record: MomentumTracker#record().
  ElitePool.generate_crossover: ElitePool#generate_crossover().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  BayesianOptimizer.param_bounds: BayesianOptimizer#param_bounds.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  BayesianOptimizer.register_result: BayesianOptimizer#register_result().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  ElitePool.add: ElitePool#add().
  BayesianOptimizer._is_too_similar: BayesianOptimizer#_is_too_similar().
  CrashMemory._crashes: CrashMemory#_crashes.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  StepSizeCalibrator.record: StepSizeCalibrator#record().
  PlateauDetector._window: PlateauDetector#_window.
  PlateauDetector._recent: PlateauDetector#_recent.
  PlateauDetector.record: PlateauDetector#record().
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  BayesianOptimizer.consecutive_failures: BayesianOptimizer#consecutive_failures.
  BayesianOptimizer._features_to_params: BayesianOptimizer#_features_to_params().
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainTrace.results: TrainTrace#results.
  BayesianOptimizer.discrete_mapping: BayesianOptimizer#discrete_mapping.
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  BayesianOptimizer.discrete_params: BayesianOptimizer#discrete_params.
  BayesianOptimizer.exploration_weight: BayesianOptimizer#exploration_weight.
  BayesianOptimizer.recent_attempts: BayesianOptimizer#recent_attempts.
  BayesianOptimizer.gp: BayesianOptimizer#gp.
  TrainRunner.client: TrainRunner#client.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  MomentumTracker.get_momentum_text: MomentumTracker#get_momentum_text().
  StepSizeCalibrator.get_step_size_text: StepSizeCalibrator#get_step_size_text().
  ElitePool.get_elite_text: ElitePool#get_elite_text().
  _is_infrastructure_error: _is_infrastructure_error().
  BayesianOptimizer._apply_llm_constraints: BayesianOptimizer#_apply_llm_constraints().
  TrainRunner.original_code: TrainRunner#original_code.
  CrashRecord: CrashRecord#
  MomentumTracker._signals: MomentumTracker#_signals.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  CrashMemory.crash_count: CrashMemory#crash_count().
  ElitePool.best_bpb: ElitePool#best_bpb().
  TrainResult.depth: TrainResult#depth.
  CrashRecord.param: CrashRecord#param.
  CrashRecord.value: CrashRecord#value.
  CrashRecord.error_hint: CrashRecord#error_hint.
  TrainTrace.best_iteration: TrainTrace#best_iteration.
  CrashMemory._param_crash_counts: CrashMemory#_param_crash_counts.
  StepSizeCalibrator._compute_relative_change: StepSizeCalibrator#_compute_relative_change().
  PlateauDetector._diversification_active: PlateauDetector#_diversification_active.
  ElitePool._max_size: ElitePool#_max_size.
  PROPOSE_PROMPT: PROPOSE_PROMPT.
  BayesianOptimizer.X_scaler: BayesianOptimizer#X_scaler.
  BayesianOptimizer.y_scaler: BayesianOptimizer#y_scaler.
  TrainRunner.QUICK_TEST_BUDGET: TrainRunner#QUICK_TEST_BUDGET.
  TrainRunner.QUICK_TEST_LOSS_THRESHOLD: TrainRunner#QUICK_TEST_LOSS_THRESHOLD.
  TrainRunner._crossover_frequency: TrainRunner#_crossover_frequency.
  TrainRunner._max_acceptable_regression: TrainRunner#_max_acceptable_regression.
  TrainRunner._sa_iteration_count: TrainRunner#_sa_iteration_count.
  TrainRunner._apply_changes: TrainRunner#_apply_changes().
  CrashRecord.iteration: CrashRecord#iteration.
  TrainTrace: TrainTrace#
  CrashMemory: CrashMemory#
  MomentumTracker: MomentumTracker#
  MomentumTracker._detect_direction: MomentumTracker#_detect_direction().
  StepSizeCalibrator: StepSizeCalibrator#
  PlateauDetector: PlateauDetector#
  PlateauDetector._min_improvement_threshold: PlateauDetector#_min_improvement_threshold.
  PlateauDetector._recently_plateaued_params: PlateauDetector#_recently_plateaued_params.
  ElitePool: ElitePool#
  ElitePool._EXPRESSION_PARAMS: ElitePool#_EXPRESSION_PARAMS.
  ElitePool._INTEGER_PARAMS: ElitePool#_INTEGER_PARAMS.
  MULTI_CANDIDATE_PROMPT: MULTI_CANDIDATE_PROMPT.
  PICK_CANDIDATE_PROMPT: PICK_CANDIDATE_PROMPT.
  INFRA_ERROR_PATTERNS: INFRA_ERROR_PATTERNS.
  BayesianOptimizer.init_samples: BayesianOptimizer#init_samples.
  BayesianOptimizer.max_consecutive_failures: BayesianOptimizer#max_consecutive_failures.
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  CrashMemory.__init__: CrashMemory#__init__().
  MomentumTracker.__init__: MomentumTracker#__init__().
  StepSizeCalibrator.__init__: StepSizeCalibrator#__init__().
  PlateauDetector.__init__: PlateauDetector#__init__().
  ElitePool.__init__: ElitePool#__init__().
  BayesianOptimizer: BayesianOptimizer#
  BayesianOptimizer.__init__: BayesianOptimizer#__init__().
  BayesianOptimizer.history: BayesianOptimizer#history.
  BayesianOptimizer.param_names: BayesianOptimizer#param_names.
  BayesianOptimizer.llm_constraints: BayesianOptimizer#llm_constraints.
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py)

## Classes
### `BayesianOptimizer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:861`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L861)
- doc: Bayesian optimization with constrained action space for hyperparameter tuning.
- signature: `class BayesianOptimizer:`
- members:
  - `__init__(self, param_bounds: Dict[str, Tuple[float, float]], discrete_params: Dict[str, List[float]], init_samples: int = 5, exploration_weight: float = 0.1, max_consecutive_failures: int = 3)` — [`L864`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L864) — Args:
  - `_apply_llm_constraints(self, params: Dict[str, Any], llm_insights: Optional[str])` — [`L971`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L971) — Apply penalty based on LLM insights.
  - `_features_to_params(self, features: np.ndarray)` — [`L931`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L931) — Convert feature vector back to params dict.
  - `_is_too_similar(self, params1: Dict[str, Any], params2: Dict[str, Any], threshold: float = 0.1)` — [`L1004`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1004) — Check if two parameter sets are too similar.
  - `_params_to_features(self, params: Dict[str, Any])` — [`L905`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L905) — Convert params dict to feature vector.
  - `_random_sample(self)` — [`L957`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L957) — Generate random sample within bounds.
  - `propose_next(self, history: List[Dict[str, Any]], current_best: float, llm_insights: Optional[str] = None)` — [`L1033`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1033) — Propose next hyperparameter configuration.
  - `register_result(self, params: Dict[str, Any], score: float, success: bool)` — [`L1156`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1156) — Register the outcome of a proposed configuration.
  - `X_scaler` — [`L899`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L899)
  - `consecutive_failures` — [`L887`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L887)
  - `discrete_mapping` — [`L893`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L893)
  - `discrete_params` — [`L881`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L881)
  - `exploration_weight` — [`L883`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L883)
  - `gp` — [`L898`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L898)
  - `history` — [`L889`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L889)
  - `init_samples` — [`L882`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L882)
  - `llm_constraints` — [`L903`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L903)
  - `max_consecutive_failures` — [`L884`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L884)
  - `param_bounds` — [`L880`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L880)
  - `param_names` — [`L890`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L890)
  - `recent_attempts` — [`L888`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L888)
  - `y_scaler` — [`L900`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L900)

### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:152`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L160), `_crashes`[`L161`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](05_patched_runner.md#logger), [`CrashRecord`](05_patched_runner.md#CrashRecord), [`error_hint`](05_patched_runner.md#CrashRecord.error_hint), [`param`](05_patched_runner.md#CrashRecord.param), [`value`](05_patched_runner.md#CrashRecord.value), [`iteration`](05_patched_runner.md#CrashRecord.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`crash_memory`](05_patched_runner.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L123)
  - `param` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L121)
  - `value` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L122)
- used by: [`record`](05_patched_runner.md#CrashMemory.record), [`get_warning_text`](05_patched_runner.md#CrashMemory.get_warning_text), [`_crashes`](05_patched_runner.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:529`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L598), `__init__`[`L538`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L538), `_max_size`[`L539`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L539), `_pool`[`L541`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L541)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`elite_pool`](05_patched_runner.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:222`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L231), `_signals`[`L235`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](05_patched_runner.md#logger)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`momentum`](05_patched_runner.md#TrainRunner.momentum)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:439`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L452), `_recent`[`L454`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L456), `_window`[`L451`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L451)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`plateau_detector`](05_patched_runner.md#TrainRunner.plateau_detector)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:344`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L351), `_history`[`L353`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L353)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`step_calibrator`](05_patched_runner.md#TrainRunner.step_calibrator)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L115)
  - `description` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L109)
  - `status` — [`L112`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L108)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:1181`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1181)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1711`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1711) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1849`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1849) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1755`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1755) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1720`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1720) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1863`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1863) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1516`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1516) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1765`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1765) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1480`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1480) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L1246`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1246) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L1185`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1185)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L1186`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1186)
  - `artifacts_dir` — [`L1201`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1201)
  - `client` — [`L1199`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1199)
  - `crash_memory` — [`L1211`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1211)
  - `current_code` — [`L1207`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1207)
  - `elite_pool` — [`L1217`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1217)
  - `momentum` — [`L1214`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1214)
  - `original_code` — [`L1206`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1206)
  - `plateau_detector` — [`L1223`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1223)
  - `search_config` — [`L1200`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1200)
  - `simple_mode` — [`L1202`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1202)
  - `step_calibrator` — [`L1220`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1220)
  - `trace` — [`L1208`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1208)
  - `train_py` — [`L1197`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1197)
  - `work_dir` — [`L1198`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1198)
- protocol/private: `__init__`[`L1188`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1188), `_best_code`[`L1242`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1242), `_crossover_frequency`[`L1226`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1226), `_exploration_frequency`[`L1230`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1230), `_iters_since_improvement`[`L1243`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1243), `_max_acceptable_regression`[`L1233`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1233), `_proposal_count`[`L1227`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1227), `_sa_cooling_rate`[`L1237`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1237), `_sa_initial_temp`[`L1236`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1236), `_sa_iteration_count`[`L1239`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1239), `_sa_temp`[`L1238`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1238), `_stagnation_threshold`[`L1244`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L1244)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`record`](05_patched_runner.md#CrashMemory.record), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`check_plateau`](05_patched_runner.md#PlateauDetector.check_plateau), [`get_warning_text`](05_patched_runner.md#CrashMemory.get_warning_text), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`generate_crossover`](05_patched_runner.md#ElitePool.generate_crossover), [`record`](05_patched_runner.md#MomentumTracker.record), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`add`](05_patched_runner.md#ElitePool.add), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`record`](05_patched_runner.md#PlateauDetector.record), [`record`](05_patched_runner.md#StepSizeCalibrator.record), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`get_elite_text`](05_patched_runner.md#ElitePool.get_elite_text), [`get_momentum_text`](05_patched_runner.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](05_patched_runner.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`CrashMemory`](05_patched_runner.md#CrashMemory), [`ElitePool`](05_patched_runner.md#ElitePool)  (+6 more)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py:128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L131)
  - `results` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L823) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L678)
- `logger` — [`L99`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/mechanism_sessions/round_1/05_patched_runner.py#L99)

