---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C2.mechanism_sessions.round_2.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  CrashMemory.record: CrashMemory#record().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  MultiScaleBanditProposer.select_scale: MultiScaleBanditProposer#select_scale().
  PostGenerationAdjuster.adjust_proposal: PostGenerationAdjuster#adjust_proposal().
  TrainRunner.search_config: TrainRunner#search_config.
  ElitePool._pool: ElitePool#_pool.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  CrashMemory.get_warning_text: CrashMemory#get_warning_text().
  PlateauDetector.check_plateau: PlateauDetector#check_plateau().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  PostGenerationAdjuster.should_adjust_param: PostGenerationAdjuster#should_adjust_param().
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
  MomentumTracker.record: MomentumTracker#record().
  ElitePool.generate_crossover: ElitePool#generate_crossover().
  PostGenerationAdjuster._calculate_adjustment_magnitude: PostGenerationAdjuster#_calculate_adjustment_magnitude().
  PostGenerationAdjuster._validate_and_bound: PostGenerationAdjuster#_validate_and_bound().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  MultiScaleBanditProposer.update_reward: MultiScaleBanditProposer#update_reward().
  MultiScaleBanditProposer.get_stats: MultiScaleBanditProposer#get_stats().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  ElitePool.add: ElitePool#add().
  CrashMemory._crashes: CrashMemory#_crashes.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  StepSizeCalibrator.record: StepSizeCalibrator#record().
  PlateauDetector._window: PlateauDetector#_window.
  PlateauDetector._recent: PlateauDetector#_recent.
  PlateauDetector.record: PlateauDetector#record().
  MultiScaleBanditProposer.visit_counts: MultiScaleBanditProposer#visit_counts.
  PostGenerationAdjuster._get_adjustment_direction: PostGenerationAdjuster#_get_adjustment_direction().
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  MultiScaleBanditProposer.q_values: MultiScaleBanditProposer#q_values.
  PostGenerationAdjuster._param_disable_count: PostGenerationAdjuster#_param_disable_count.
  PostGenerationAdjuster.get_adjustment_summary: PostGenerationAdjuster#get_adjustment_summary().
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainTrace.results: TrainTrace#results.
  PostGenerationAdjuster._clamp_to_bounds: PostGenerationAdjuster#_clamp_to_bounds().
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  PostGenerationAdjuster.fallback_to_original: PostGenerationAdjuster#fallback_to_original.
  PostGenerationAdjuster.adjustment_history: PostGenerationAdjuster#adjustment_history.
  TrainRunner.client: TrainRunner#client.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  MomentumTracker.get_momentum_text: MomentumTracker#get_momentum_text().
  StepSizeCalibrator.get_step_size_text: StepSizeCalibrator#get_step_size_text().
  ElitePool.get_elite_text: ElitePool#get_elite_text().
  _is_infrastructure_error: _is_infrastructure_error().
  MultiScaleBanditProposer.get_scale_parameters: MultiScaleBanditProposer#get_scale_parameters().
  TrainRunner.original_code: TrainRunner#original_code.
  CrashRecord: CrashRecord#
  MomentumTracker._signals: MomentumTracker#_signals.
  MultiScaleBanditProposer.total_visits: MultiScaleBanditProposer#total_visits.
  PostGenerationAdjuster.config: PostGenerationAdjuster#config.
  PostGenerationAdjuster.logger: PostGenerationAdjuster#logger.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  CrashMemory.crash_count: CrashMemory#crash_count().
  ElitePool.best_bpb: ElitePool#best_bpb().
  PostGenerationAdjuster.record_adjustment_performance: PostGenerationAdjuster#record_adjustment_performance().
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
  MultiScaleBanditProposer.scale_levels: MultiScaleBanditProposer#scale_levels.
  PostGenerationAdjuster.momentum_tracker: PostGenerationAdjuster#momentum_tracker.
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
  MultiScaleBanditProposer.initial_exploration_bias: MultiScaleBanditProposer#initial_exploration_bias.
  MultiScaleBanditProposer.exploration_decay: MultiScaleBanditProposer#exploration_decay.
  MultiScaleBanditProposer.min_exploration: MultiScaleBanditProposer#min_exploration.
  MultiScaleBanditProposer.scale_parameters: MultiScaleBanditProposer#scale_parameters.
  PostGenerationAdjuster.step_calibrator: PostGenerationAdjuster#step_calibrator.
  PostGenerationAdjuster.elite_pool: PostGenerationAdjuster#elite_pool.
  PostGenerationAdjuster.adjustment_enabled: PostGenerationAdjuster#adjustment_enabled.
  PostGenerationAdjuster.max_relative_adjustment: PostGenerationAdjuster#max_relative_adjustment.
  PostGenerationAdjuster._allowlist: PostGenerationAdjuster#_allowlist.
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
  MultiScaleBanditProposer: MultiScaleBanditProposer#
  MultiScaleBanditProposer.__init__: MultiScaleBanditProposer#__init__().
  MultiScaleBanditProposer.optimistic_init_value: MultiScaleBanditProposer#optimistic_init_value.
  MultiScaleBanditProposer._calculate_information_gain: MultiScaleBanditProposer#_calculate_information_gain().
  PostGenerationAdjuster: PostGenerationAdjuster#
  PostGenerationAdjuster.__init__: PostGenerationAdjuster#__init__().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py)

## Classes
### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:152`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L160), `_crashes`[`L161`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](05_patched_runner.md#logger), [`CrashRecord`](05_patched_runner.md#CrashRecord), [`error_hint`](05_patched_runner.md#CrashRecord.error_hint), [`param`](05_patched_runner.md#CrashRecord.param), [`value`](05_patched_runner.md#CrashRecord.value), [`iteration`](05_patched_runner.md#CrashRecord.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`crash_memory`](05_patched_runner.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L123)
  - `param` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L121)
  - `value` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L122)
- used by: [`record`](05_patched_runner.md#CrashMemory.record), [`get_warning_text`](05_patched_runner.md#CrashMemory.get_warning_text), [`_crashes`](05_patched_runner.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:529`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L598), `__init__`[`L538`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L538), `_max_size`[`L539`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L539), `_pool`[`L541`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L541)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`elite_pool`](05_patched_runner.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:222`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L231), `_signals`[`L235`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](05_patched_runner.md#logger)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`momentum`](05_patched_runner.md#TrainRunner.momentum)

### `MultiScaleBanditProposer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:856`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L856)
- doc: Bandit system for selecting proposal scales based on information gain.
- signature: `class MultiScaleBanditProposer:`
- members:
  - `__init__(self, scale_levels: list[str] = None, initial_exploration_bias: float = 0.7, exploration_decay: float = 0.95, min_exploration: float = 0.1, optimistic_init_value: float = 2)` — [`L859`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L859) — Args:
  - `_calculate_information_gain(self, scale_level: str, was_accepted: bool, performance_change: float = None)` — [`L975`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L975) — Calculate information gain metric (0-1).
  - `get_scale_parameters(self, scale_level: str)` — [`L968`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L968) — Get mutation parameters for a given scale level.
  - `get_stats(self)` — [`L998`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L998) — Return current bandit statistics for debugging.
  - `select_scale(self, current_config: dict, iteration: int, recent_performance: list[float] = None)` — [`L895`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L895) — Select a scale level for the next proposal.
  - `update_reward(self, scale_level: str, was_accepted: bool, information_gain: float, performance_change: float = None)` — [`L930`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L930) — Update bandit Q-values based on outcome.
  - `exploration_decay` — [`L879`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L879)
  - `initial_exploration_bias` — [`L878`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L878)
  - `min_exploration` — [`L880`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L880)
  - `optimistic_init_value` — [`L881`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L881)
  - `q_values` — [`L883`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L883)
  - `scale_levels` — [`L877`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L877)
  - `scale_parameters` — [`L887`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L887)
  - `total_visits` — [`L885`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L885)
  - `visit_counts` — [`L884`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L884)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:439`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L452), `_recent`[`L454`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L456), `_window`[`L451`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L451)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`plateau_detector`](05_patched_runner.md#TrainRunner.plateau_detector)

### `PostGenerationAdjuster`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:1020`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1020)
- doc: Adjusts LLM-generated parameter proposals based on momentum, elite pool patterns,
- signature: `class PostGenerationAdjuster:`
- members:
  - `__init__(self, momentum_tracker, step_calibrator, elite_pool, config, adjustment_enabled: bool = True, fallback_to_original: bool = True, max_relative_adjustment: float = 0.2)` — [`L1030`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1030) — Args:
  - `_calculate_adjustment_magnitude(self, param_name: str, proposed_value: float, direction: int)` — [`L1204`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1204) — Calculate the adjustment magnitude based on step size and constraints.
  - `_clamp_to_bounds(self, param_name: str, value: float)` — [`L1260`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1260) — Clamp value to parameter bounds.
  - `_get_adjustment_direction(self, param_name: str, proposed_value: float)` — [`L1173`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1173) — Determine adjustment direction (1 for increase, -1 for decrease, 0 for none).
  - `_validate_and_bound(self, param_name: str, proposed_value: float, adjusted_value: float)` — [`L1226`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1226) — Validate adjusted value and apply bounds if necessary.
  - `adjust_proposal(self, param_name: str, proposed_value: float, current_value: Optional[float], param_type: str = "continuous", iteration: int = 0)` — [`L1067`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1067) — Adjust a single proposed parameter value based on momentum and calibration.
  - `get_adjustment_summary(self)` — [`L1285`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1285) — Generate a summary of adjustments for debugging.
  - `record_adjustment_performance(self, param_name: str, original_bpb: float, adjusted_bpb: float)` — [`L1276`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1276) — Record performance of adjustment to potentially disable poorly performing parameters.
  - `should_adjust_param(self, param_name: str)` — [`L1139`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1139) — Determine if parameter should be adjusted.
  - `adjustment_enabled` — [`L1054`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1054)
  - `adjustment_history` — [`L1062`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1062)
  - `config` — [`L1053`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1053)
  - `elite_pool` — [`L1052`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1052)
  - `fallback_to_original` — [`L1055`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1055)
  - `logger` — [`L1065`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1065)
  - `max_relative_adjustment` — [`L1056`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1056)
  - `momentum_tracker` — [`L1050`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1050)
  - `step_calibrator` — [`L1051`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1051)
- protocol/private: `_allowlist`[`L1059`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1059), `_param_disable_count`[`L1063`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1063)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:344`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L351), `_history`[`L353`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L353)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`step_calibrator`](05_patched_runner.md#TrainRunner.step_calibrator)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L115)
  - `description` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L109)
  - `status` — [`L112`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L108)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:1310`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1310)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1840`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1840) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1978`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1978) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1884`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1884) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1849`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1849) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1992`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1992) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1645`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1645) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1894`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1894) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1609`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1609) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L1375`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1375) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L1314`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1314)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L1315`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1315)
  - `artifacts_dir` — [`L1330`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1330)
  - `client` — [`L1328`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1328)
  - `crash_memory` — [`L1340`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1340)
  - `current_code` — [`L1336`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1336)
  - `elite_pool` — [`L1346`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1346)
  - `momentum` — [`L1343`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1343)
  - `original_code` — [`L1335`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1335)
  - `plateau_detector` — [`L1352`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1352)
  - `search_config` — [`L1329`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1329)
  - `simple_mode` — [`L1331`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1331)
  - `step_calibrator` — [`L1349`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1349)
  - `trace` — [`L1337`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1337)
  - `train_py` — [`L1326`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1326)
  - `work_dir` — [`L1327`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1327)
- protocol/private: `__init__`[`L1317`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1317), `_best_code`[`L1371`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1371), `_crossover_frequency`[`L1355`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1355), `_exploration_frequency`[`L1359`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1359), `_iters_since_improvement`[`L1372`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1372), `_max_acceptable_regression`[`L1362`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1362), `_proposal_count`[`L1356`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1356), `_sa_cooling_rate`[`L1366`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1366), `_sa_initial_temp`[`L1365`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1365), `_sa_iteration_count`[`L1368`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1368), `_sa_temp`[`L1367`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1367), `_stagnation_threshold`[`L1373`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L1373)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`record`](05_patched_runner.md#CrashMemory.record), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`check_plateau`](05_patched_runner.md#PlateauDetector.check_plateau), [`get_warning_text`](05_patched_runner.md#CrashMemory.get_warning_text), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`generate_crossover`](05_patched_runner.md#ElitePool.generate_crossover), [`record`](05_patched_runner.md#MomentumTracker.record), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`add`](05_patched_runner.md#ElitePool.add), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`record`](05_patched_runner.md#PlateauDetector.record), [`record`](05_patched_runner.md#StepSizeCalibrator.record), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`get_elite_text`](05_patched_runner.md#ElitePool.get_elite_text), [`get_momentum_text`](05_patched_runner.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](05_patched_runner.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`CrashMemory`](05_patched_runner.md#CrashMemory), [`ElitePool`](05_patched_runner.md#ElitePool)  (+6 more)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py:128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L131)
  - `results` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L823) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L678)
- `logger` — [`L99`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/mechanism_sessions/round_2/05_patched_runner.py#L99)

