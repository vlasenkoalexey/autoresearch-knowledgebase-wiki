---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C1.runner_final`/
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
  PhaseDetector.update_and_detect: PhaseDetector#update_and_detect().
  TrainRunner.search_config: TrainRunner#search_config.
  ElitePool._pool: ElitePool#_pool.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  CrashMemory.get_warning_text: CrashMemory#get_warning_text().
  PlateauDetector.check_plateau: PlateauDetector#check_plateau().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  TabuSearchManager.add_tabu_entry: TabuSearchManager#add_tabu_entry().
  TrainResult.status: TrainResult#status.
  TabuSearchManager.tabu_list: TabuSearchManager#tabu_list.
  MomentumTracker.record: MomentumTracker#record().
  ElitePool.generate_crossover: ElitePool#generate_crossover().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  TabuSearchManager.update_distance_thresholds: TabuSearchManager#update_distance_thresholds().
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
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  TabuSearchManager.is_tabu: TabuSearchManager#is_tabu().
  TabuSearchManager.get_suggested_alternatives: TabuSearchManager#get_suggested_alternatives().
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainTrace.results: TrainTrace#results.
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  TabuSearchManager.distance_thresholds: TabuSearchManager#distance_thresholds.
  PhaseDetector.improvement_streak: PhaseDetector#improvement_streak.
  PhaseDetector.plateau_counter: PhaseDetector#plateau_counter.
  TrainRunner.client: TrainRunner#client.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  MomentumTracker.get_momentum_text: MomentumTracker#get_momentum_text().
  StepSizeCalibrator.get_step_size_text: StepSizeCalibrator#get_step_size_text().
  ElitePool.get_elite_text: ElitePool#get_elite_text().
  _is_infrastructure_error: _is_infrastructure_error().
  TrainRunner.original_code: TrainRunner#original_code.
  CrashRecord: CrashRecord#
  MomentumTracker._signals: MomentumTracker#_signals.
  PhaseDetector.non_improvement_streak: PhaseDetector#non_improvement_streak.
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
  TabuSearchManager.max_tabu_size: TabuSearchManager#max_tabu_size.
  PhaseDetector.min_improvement: PhaseDetector#min_improvement.
  PhaseDetector.last_best_bpb: PhaseDetector#last_best_bpb.
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
  TabuSearchManager.tabu_tenure: TabuSearchManager#tabu_tenure.
  TabuSearchManager.enable_adaptive_thresholds: TabuSearchManager#enable_adaptive_thresholds.
  TabuSearchManager.iteration_history: TabuSearchManager#iteration_history.
  TabuSearchManager.logger: TabuSearchManager#logger.
  PhaseDetector.exploration_window: PhaseDetector#exploration_window.
  PhaseDetector.exploitation_window: PhaseDetector#exploitation_window.
  PhaseDetector.stagnation_threshold: PhaseDetector#stagnation_threshold.
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
  TabuSearchManager: TabuSearchManager#
  TabuSearchManager.__init__: TabuSearchManager#__init__().
  PhaseDetector: PhaseDetector#
  PhaseDetector.__init__: PhaseDetector#__init__().
  _build_proposal_prompt: _build_proposal_prompt().
  get_phase_summary: get_phase_summary().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py)

## Classes
### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:152`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L160), `_crashes`[`L161`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](runner_final.md#logger), [`CrashRecord`](runner_final.md#CrashRecord), [`error_hint`](runner_final.md#CrashRecord.error_hint), [`param`](runner_final.md#CrashRecord.param), [`value`](runner_final.md#CrashRecord.value), [`iteration`](runner_final.md#CrashRecord.iteration)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`crash_memory`](runner_final.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:119`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L123)
  - `param` — [`L121`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L121)
  - `value` — [`L122`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L122)
- used by: [`record`](runner_final.md#CrashMemory.record), [`get_warning_text`](runner_final.md#CrashMemory.get_warning_text), [`_crashes`](runner_final.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:529`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L598), `__init__`[`L538`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L538), `_max_size`[`L539`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L539), `_pool`[`L541`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L541)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`run_baseline`](runner_final.md#TrainRunner.run_baseline), [`elite_pool`](runner_final.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:222`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L231), `_signals`[`L235`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](runner_final.md#logger)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`momentum`](runner_final.md#TrainRunner.momentum)

### `PhaseDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:1083`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1083)
- doc: Detects optimization phases based on performance trends.
- signature: `class PhaseDetector:`
- members:
  - `__init__(self, exploration_window: int = 3, exploitation_window: int = 4, stagnation_threshold: int = 3, min_improvement: float = 0.0003)` — [`L1086`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1086) — Args:
  - `update_and_detect(self, iteration: int, current_bpb: float)` — [`L1111`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1111) — Update internal state and return current phase.
  - `exploitation_window` — [`L1101`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1101)
  - `exploration_window` — [`L1100`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1100)
  - `improvement_streak` — [`L1106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1106)
  - `last_best_bpb` — [`L1109`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1109)
  - `min_improvement` — [`L1103`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1103)
  - `non_improvement_streak` — [`L1107`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1107)
  - `plateau_counter` — [`L1108`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1108)
  - `stagnation_threshold` — [`L1102`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1102)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:439`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L452), `_recent`[`L454`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L456), `_window`[`L451`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L451)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`plateau_detector`](runner_final.md#TrainRunner.plateau_detector)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:344`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L351), `_history`[`L353`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L353)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`step_calibrator`](runner_final.md#TrainRunner.step_calibrator)

### `TabuSearchManager`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:853`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L853)
- doc: Manages tabu lists to prevent revisiting recently explored parameter regions.
- signature: `class TabuSearchManager:`
- members:
  - `__init__(self, max_tabu_size: int = 10, tabu_tenure: int = 3, distance_thresholds: Optional[dict[str, float]] = None, enable_adaptive_thresholds: bool = True)` — [`L856`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L856) — Args:
  - `add_tabu_entry(self, config: dict[str, Any], iteration: int, reason: str = "explored")` — [`L917`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L917) — Add a configuration to the tabu list.
  - `get_suggested_alternatives(self, current_config: dict[str, Any], param_ranges: dict[str, tuple[float, float]])` — [`L1010`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1010) — Suggest alternative values for parameters that are currently tabu.
  - `is_tabu(self, config: dict[str, Any], current_iteration: int)` — [`L884`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L884) — Check if a configuration is tabu (forbidden).
  - `update_distance_thresholds(self, elite_configs: list[dict[str, Any]], current_iteration: int)` — [`L946`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L946) — Adaptively update distance thresholds based on elite configurations.
  - `distance_thresholds` — [`L872`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L872)
  - `enable_adaptive_thresholds` — [`L879`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L879)
  - `iteration_history` — [`L881`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L881)
  - `logger` — [`L882`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L882)
  - `max_tabu_size` — [`L870`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L870)
  - `tabu_list` — [`L880`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L880)
  - `tabu_tenure` — [`L871`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L871)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L115)
  - `description` — [`L114`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L109)
  - `status` — [`L112`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L108)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`run_baseline`](runner_final.md#TrainRunner.run_baseline), [`add`](runner_final.md#TrainTrace.add), [`summary`](runner_final.md#TrainTrace.summary), [`results`](runner_final.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:1279`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1279)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1809`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1809) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1947`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1947) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1853`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1853) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1818`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1818) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1961`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1961) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1614`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1614) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1863`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1863) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1578`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1578) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L1344`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1344) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L1283`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1283)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L1284`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1284)
  - `artifacts_dir` — [`L1299`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1299)
  - `client` — [`L1297`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1297)
  - `crash_memory` — [`L1309`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1309)
  - `current_code` — [`L1305`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1305)
  - `elite_pool` — [`L1315`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1315)
  - `momentum` — [`L1312`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1312)
  - `original_code` — [`L1304`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1304)
  - `plateau_detector` — [`L1321`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1321)
  - `search_config` — [`L1298`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1298)
  - `simple_mode` — [`L1300`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1300)
  - `step_calibrator` — [`L1318`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1318)
  - `trace` — [`L1306`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1306)
  - `train_py` — [`L1295`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1295)
  - `work_dir` — [`L1296`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1296)
- protocol/private: `__init__`[`L1286`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1286), `_best_code`[`L1340`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1340), `_crossover_frequency`[`L1324`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1324), `_exploration_frequency`[`L1328`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1328), `_iters_since_improvement`[`L1341`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1341), `_max_acceptable_regression`[`L1331`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1331), `_proposal_count`[`L1325`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1325), `_sa_cooling_rate`[`L1335`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1335), `_sa_initial_temp`[`L1334`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1334), `_sa_iteration_count`[`L1337`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1337), `_sa_temp`[`L1336`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1336), `_stagnation_threshold`[`L1342`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1342)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](runner_final.md#logger), [`record`](runner_final.md#CrashMemory.record), [`add`](runner_final.md#TrainTrace.add), [`summary`](runner_final.md#TrainTrace.summary), [`best_bpb`](runner_final.md#TrainTrace.best_bpb), [`check_plateau`](runner_final.md#PlateauDetector.check_plateau), [`get_warning_text`](runner_final.md#CrashMemory.get_warning_text), [`val_bpb`](runner_final.md#TrainResult.val_bpb), [`TrainResult`](runner_final.md#TrainResult), [`status`](runner_final.md#TrainResult.status), [`generate_crossover`](runner_final.md#ElitePool.generate_crossover), [`record`](runner_final.md#MomentumTracker.record), [`description`](runner_final.md#TrainResult.description), [`iteration`](runner_final.md#TrainResult.iteration), [`add`](runner_final.md#ElitePool.add), [`changes`](runner_final.md#TrainResult.changes), [`num_params_m`](runner_final.md#TrainResult.num_params_m), [`peak_vram_mb`](runner_final.md#TrainResult.peak_vram_mb), [`record`](runner_final.md#PlateauDetector.record), [`record`](runner_final.md#StepSizeCalibrator.record), [`training_seconds`](runner_final.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](runner_final.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](runner_final.md#_is_infrastructure_error), [`get_elite_text`](runner_final.md#ElitePool.get_elite_text), [`get_momentum_text`](runner_final.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](runner_final.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](runner_final.md#PROPOSE_PROMPT), [`depth`](runner_final.md#TrainResult.depth), [`CrashMemory`](runner_final.md#CrashMemory), [`ElitePool`](runner_final.md#ElitePool)  (+6 more)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py:128`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L131)
  - `results` — [`L129`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner_final.md#TrainResult.val_bpb), [`TrainResult`](runner_final.md#TrainResult), [`status`](runner_final.md#TrainResult.status), [`description`](runner_final.md#TrainResult.description), [`iteration`](runner_final.md#TrainResult.iteration)
- used by: [`run_iteration`](runner_final.md#TrainRunner.run_iteration), [`_propose`](runner_final.md#TrainRunner._propose), [`run_baseline`](runner_final.md#TrainRunner.run_baseline), [`trace`](runner_final.md#TrainRunner.trace)

## Functions
- `_build_proposal_prompt(self, current_config: dict[str, any], iteration: int, phase: str)` — [`L1149`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1149) — Build phase-aware prompt for LLM proposals.
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L823) — Check if a crash was caused by infrastructure (not training).
- `get_phase_summary(self)` — [`L1264`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L1264) — Return phase detection state for debugging.

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L678)
- `logger` — [`L99`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C1/runner_final.py#L99)

