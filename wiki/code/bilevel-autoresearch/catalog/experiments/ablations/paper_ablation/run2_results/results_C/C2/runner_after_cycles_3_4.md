---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C2.runner_after_cycles_3_4`/
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
  TrainRunner.search_config: TrainRunner#search_config.
  ElitePool._pool: ElitePool#_pool.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  CrashMemory.get_warning_text: CrashMemory#get_warning_text().
  PlateauDetector.check_plateau: PlateauDetector#check_plateau().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
  MomentumTracker.record: MomentumTracker#record().
  ElitePool.generate_crossover: ElitePool#generate_crossover().
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
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  MultiScaleBanditProposer.q_values: MultiScaleBanditProposer#q_values.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainTrace.results: TrainTrace#results.
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
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
  MultiScaleBanditProposer.scale_levels: MultiScaleBanditProposer#scale_levels.
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
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py)

## Classes
### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:152`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L160), `_crashes`[`L161`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](runner_after_cycles_3_4.md#logger), [`CrashRecord`](runner_after_cycles_3_4.md#CrashRecord), [`error_hint`](runner_after_cycles_3_4.md#CrashRecord.error_hint), [`param`](runner_after_cycles_3_4.md#CrashRecord.param), [`value`](runner_after_cycles_3_4.md#CrashRecord.value), [`iteration`](runner_after_cycles_3_4.md#CrashRecord.iteration)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`crash_memory`](runner_after_cycles_3_4.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:119`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L123)
  - `param` — [`L121`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L121)
  - `value` — [`L122`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L122)
- used by: [`record`](runner_after_cycles_3_4.md#CrashMemory.record), [`get_warning_text`](runner_after_cycles_3_4.md#CrashMemory.get_warning_text), [`_crashes`](runner_after_cycles_3_4.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:529`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L598), `__init__`[`L538`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L538), `_max_size`[`L539`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L539), `_pool`[`L541`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L541)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`run_baseline`](runner_after_cycles_3_4.md#TrainRunner.run_baseline), [`elite_pool`](runner_after_cycles_3_4.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:222`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L231), `_signals`[`L235`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](runner_after_cycles_3_4.md#logger)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`momentum`](runner_after_cycles_3_4.md#TrainRunner.momentum)

### `MultiScaleBanditProposer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:856`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L856)
- doc: Bandit system for selecting proposal scales based on information gain.
- signature: `class MultiScaleBanditProposer:`
- members:
  - `__init__(self, scale_levels: list[str] = None, initial_exploration_bias: float = 0.7, exploration_decay: float = 0.95, min_exploration: float = 0.1, optimistic_init_value: float = 2)` — [`L859`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L859) — Args:
  - `_calculate_information_gain(self, scale_level: str, was_accepted: bool, performance_change: float = None)` — [`L975`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L975) — Calculate information gain metric (0-1).
  - `get_scale_parameters(self, scale_level: str)` — [`L968`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L968) — Get mutation parameters for a given scale level.
  - `get_stats(self)` — [`L998`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L998) — Return current bandit statistics for debugging.
  - `select_scale(self, current_config: dict, iteration: int, recent_performance: list[float] = None)` — [`L895`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L895) — Select a scale level for the next proposal.
  - `update_reward(self, scale_level: str, was_accepted: bool, information_gain: float, performance_change: float = None)` — [`L930`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L930) — Update bandit Q-values based on outcome.
  - `exploration_decay` — [`L879`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L879)
  - `initial_exploration_bias` — [`L878`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L878)
  - `min_exploration` — [`L880`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L880)
  - `optimistic_init_value` — [`L881`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L881)
  - `q_values` — [`L883`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L883)
  - `scale_levels` — [`L877`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L877)
  - `scale_parameters` — [`L887`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L887)
  - `total_visits` — [`L885`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L885)
  - `visit_counts` — [`L884`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L884)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:439`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L452), `_recent`[`L454`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L456), `_window`[`L451`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L451)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`plateau_detector`](runner_after_cycles_3_4.md#TrainRunner.plateau_detector)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:344`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L351), `_history`[`L353`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L353)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`step_calibrator`](runner_after_cycles_3_4.md#TrainRunner.step_calibrator)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L115)
  - `description` — [`L114`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L109)
  - `status` — [`L112`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L108)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`run_baseline`](runner_after_cycles_3_4.md#TrainRunner.run_baseline), [`add`](runner_after_cycles_3_4.md#TrainTrace.add), [`summary`](runner_after_cycles_3_4.md#TrainTrace.summary), [`results`](runner_after_cycles_3_4.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:1008`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1008)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1538`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1538) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1676`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1676) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1582`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1582) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1547`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1547) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1690`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1690) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1343`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1343) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1592`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1592) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1307`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1307) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L1073`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1073) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L1012`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1012)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L1013`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1013)
  - `artifacts_dir` — [`L1028`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1028)
  - `client` — [`L1026`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1026)
  - `crash_memory` — [`L1038`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1038)
  - `current_code` — [`L1034`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1034)
  - `elite_pool` — [`L1044`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1044)
  - `momentum` — [`L1041`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1041)
  - `original_code` — [`L1033`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1033)
  - `plateau_detector` — [`L1050`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1050)
  - `search_config` — [`L1027`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1027)
  - `simple_mode` — [`L1029`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1029)
  - `step_calibrator` — [`L1047`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1047)
  - `trace` — [`L1035`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1035)
  - `train_py` — [`L1024`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1024)
  - `work_dir` — [`L1025`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1025)
- protocol/private: `__init__`[`L1015`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1015), `_best_code`[`L1069`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1069), `_crossover_frequency`[`L1053`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1053), `_exploration_frequency`[`L1057`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1057), `_iters_since_improvement`[`L1070`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1070), `_max_acceptable_regression`[`L1060`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1060), `_proposal_count`[`L1054`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1054), `_sa_cooling_rate`[`L1064`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1064), `_sa_initial_temp`[`L1063`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1063), `_sa_iteration_count`[`L1066`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1066), `_sa_temp`[`L1065`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1065), `_stagnation_threshold`[`L1071`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L1071)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](runner_after_cycles_3_4.md#logger), [`record`](runner_after_cycles_3_4.md#CrashMemory.record), [`add`](runner_after_cycles_3_4.md#TrainTrace.add), [`summary`](runner_after_cycles_3_4.md#TrainTrace.summary), [`best_bpb`](runner_after_cycles_3_4.md#TrainTrace.best_bpb), [`check_plateau`](runner_after_cycles_3_4.md#PlateauDetector.check_plateau), [`get_warning_text`](runner_after_cycles_3_4.md#CrashMemory.get_warning_text), [`val_bpb`](runner_after_cycles_3_4.md#TrainResult.val_bpb), [`TrainResult`](runner_after_cycles_3_4.md#TrainResult), [`status`](runner_after_cycles_3_4.md#TrainResult.status), [`generate_crossover`](runner_after_cycles_3_4.md#ElitePool.generate_crossover), [`record`](runner_after_cycles_3_4.md#MomentumTracker.record), [`description`](runner_after_cycles_3_4.md#TrainResult.description), [`iteration`](runner_after_cycles_3_4.md#TrainResult.iteration), [`add`](runner_after_cycles_3_4.md#ElitePool.add), [`changes`](runner_after_cycles_3_4.md#TrainResult.changes), [`num_params_m`](runner_after_cycles_3_4.md#TrainResult.num_params_m), [`peak_vram_mb`](runner_after_cycles_3_4.md#TrainResult.peak_vram_mb), [`record`](runner_after_cycles_3_4.md#PlateauDetector.record), [`record`](runner_after_cycles_3_4.md#StepSizeCalibrator.record), [`training_seconds`](runner_after_cycles_3_4.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](runner_after_cycles_3_4.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](runner_after_cycles_3_4.md#_is_infrastructure_error), [`get_elite_text`](runner_after_cycles_3_4.md#ElitePool.get_elite_text), [`get_momentum_text`](runner_after_cycles_3_4.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](runner_after_cycles_3_4.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](runner_after_cycles_3_4.md#PROPOSE_PROMPT), [`depth`](runner_after_cycles_3_4.md#TrainResult.depth), [`CrashMemory`](runner_after_cycles_3_4.md#CrashMemory), [`ElitePool`](runner_after_cycles_3_4.md#ElitePool)  (+6 more)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py:128`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L131)
  - `results` — [`L129`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner_after_cycles_3_4.md#TrainResult.val_bpb), [`TrainResult`](runner_after_cycles_3_4.md#TrainResult), [`status`](runner_after_cycles_3_4.md#TrainResult.status), [`description`](runner_after_cycles_3_4.md#TrainResult.description), [`iteration`](runner_after_cycles_3_4.md#TrainResult.iteration)
- used by: [`run_iteration`](runner_after_cycles_3_4.md#TrainRunner.run_iteration), [`_propose`](runner_after_cycles_3_4.md#TrainRunner._propose), [`run_baseline`](runner_after_cycles_3_4.md#TrainRunner.run_baseline), [`trace`](runner_after_cycles_3_4.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L823) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L678)
- `logger` — [`L99`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C2/runner_after_cycles_3_4.py#L99)

