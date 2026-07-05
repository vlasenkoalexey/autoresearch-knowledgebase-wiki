---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_C.C3.runner`/
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
  OrthogonalExplorer._generate_orthogonal_samples: OrthogonalExplorer#_generate_orthogonal_samples().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  OrthogonalExplorer.sample_index: OrthogonalExplorer#sample_index.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  OrthogonalExplorer.record_visit: OrthogonalExplorer#record_visit().
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
  OrthogonalExplorer._initialize_step_sizes: OrthogonalExplorer#_initialize_step_sizes().
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  OrthogonalExplorer.get_exploration_bonus: OrthogonalExplorer#get_exploration_bonus().
  OrthogonalExplorer.get_orthogonal_sample: OrthogonalExplorer#get_orthogonal_sample().
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainTrace.results: TrainTrace#results.
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  OrthogonalExplorer.param_ranges: OrthogonalExplorer#param_ranges.
  OrthogonalExplorer.param_visit_counts: OrthogonalExplorer#param_visit_counts.
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
  OrthogonalExplorer.param_step_sizes: OrthogonalExplorer#param_step_sizes.
  OrthogonalExplorer.orthogonal_samples: OrthogonalExplorer#orthogonal_samples.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  CrashMemory.crash_count: CrashMemory#crash_count().
  ElitePool.best_bpb: ElitePool#best_bpb().
  OrthogonalExplorer.get_step_size: OrthogonalExplorer#get_step_size().
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
  OrthogonalExplorer.n_samples: OrthogonalExplorer#n_samples.
  OrthogonalExplorer.exploration_bonus_weight: OrthogonalExplorer#exploration_bonus_weight.
  OrthogonalExplorer.decay_rate: OrthogonalExplorer#decay_rate.
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
  OrthogonalExplorer: OrthogonalExplorer#
  OrthogonalExplorer.__init__: OrthogonalExplorer#__init__().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py)

## Classes
### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:152`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L160), `_crashes`[`L161`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](runner.md#logger), [`CrashRecord`](runner.md#CrashRecord), [`error_hint`](runner.md#CrashRecord.error_hint), [`param`](runner.md#CrashRecord.param), [`value`](runner.md#CrashRecord.value), [`iteration`](runner.md#CrashRecord.iteration)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`crash_memory`](runner.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:119`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L123)
  - `param` — [`L121`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L121)
  - `value` — [`L122`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L122)
- used by: [`record`](runner.md#CrashMemory.record), [`get_warning_text`](runner.md#CrashMemory.get_warning_text), [`_crashes`](runner.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:529`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L598), `__init__`[`L538`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L538), `_max_size`[`L539`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L539), `_pool`[`L541`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L541)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`elite_pool`](runner.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:222`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L231), `_signals`[`L235`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](runner.md#logger)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`momentum`](runner.md#TrainRunner.momentum)

### `OrthogonalExplorer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:850`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L850)
- doc: Manages systematic exploration of hyperparameter space using orthogonal sampling.
- signature: `class OrthogonalExplorer:`
- members:
  - `__init__(self, param_ranges: Dict[str, Tuple[float, float]], n_samples: int = 8, exploration_bonus_weight: float = 0.3, decay_rate: float = 0.85)` — [`L853`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L853) — Args:
  - `_generate_orthogonal_samples(self)` — [`L920`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L920) — Generate Latin hypercube samples for systematic exploration.
  - `_initialize_step_sizes(self)` — [`L913`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L913) — Initialize step sizes based on parameter ranges.
  - `get_exploration_bonus(self, param_name: str)` — [`L881`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L881) — Calculate exploration bonus for a parameter based on visit frequency.
  - `get_orthogonal_sample(self)` — [`L904`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L904) — Get next orthogonal sample, or None if all used.
  - `get_step_size(self, param_name: str)` — [`L894`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L894) — Get exponentially decayed step size for parameter.
  - `record_visit(self, param_name: str)` — [`L898`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L898) — Record that a parameter was modified.
  - `decay_rate` — [`L870`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L870)
  - `exploration_bonus_weight` — [`L869`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L869)
  - `n_samples` — [`L868`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L868)
  - `orthogonal_samples` — [`L875`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L875)
  - `param_ranges` — [`L867`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L867)
  - `param_step_sizes` — [`L874`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L874)
  - `param_visit_counts` — [`L873`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L873)
  - `sample_index` — [`L876`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L876)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:439`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L452), `_recent`[`L454`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L456), `_window`[`L451`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L451)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`plateau_detector`](runner.md#TrainRunner.plateau_detector)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:344`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L351), `_history`[`L353`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L353)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`step_calibrator`](runner.md#TrainRunner.step_calibrator)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L115)
  - `description` — [`L114`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L109)
  - `status` — [`L112`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L108)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`add`](runner.md#TrainTrace.add), [`summary`](runner.md#TrainTrace.summary), [`results`](runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:937`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L937)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1467`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1467) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1605`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1605) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1511`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1511) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1476`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1476) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1619`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1619) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1272`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1272) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1521`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1521) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1236`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1236) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L1002`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1002) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L941`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L941)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L942`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L942)
  - `artifacts_dir` — [`L957`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L957)
  - `client` — [`L955`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L955)
  - `crash_memory` — [`L967`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L967)
  - `current_code` — [`L963`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L963)
  - `elite_pool` — [`L973`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L973)
  - `momentum` — [`L970`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L970)
  - `original_code` — [`L962`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L962)
  - `plateau_detector` — [`L979`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L979)
  - `search_config` — [`L956`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L956)
  - `simple_mode` — [`L958`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L958)
  - `step_calibrator` — [`L976`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L976)
  - `trace` — [`L964`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L964)
  - `train_py` — [`L953`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L953)
  - `work_dir` — [`L954`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L954)
- protocol/private: `__init__`[`L944`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L944), `_best_code`[`L998`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L998), `_crossover_frequency`[`L982`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L982), `_exploration_frequency`[`L986`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L986), `_iters_since_improvement`[`L999`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L999), `_max_acceptable_regression`[`L989`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L989), `_proposal_count`[`L983`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L983), `_sa_cooling_rate`[`L993`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L993), `_sa_initial_temp`[`L992`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L992), `_sa_iteration_count`[`L995`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L995), `_sa_temp`[`L994`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L994), `_stagnation_threshold`[`L1000`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L1000)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](runner.md#logger), [`record`](runner.md#CrashMemory.record), [`add`](runner.md#TrainTrace.add), [`summary`](runner.md#TrainTrace.summary), [`best_bpb`](runner.md#TrainTrace.best_bpb), [`check_plateau`](runner.md#PlateauDetector.check_plateau), [`get_warning_text`](runner.md#CrashMemory.get_warning_text), [`val_bpb`](runner.md#TrainResult.val_bpb), [`TrainResult`](runner.md#TrainResult), [`status`](runner.md#TrainResult.status), [`generate_crossover`](runner.md#ElitePool.generate_crossover), [`record`](runner.md#MomentumTracker.record), [`description`](runner.md#TrainResult.description), [`iteration`](runner.md#TrainResult.iteration), [`add`](runner.md#ElitePool.add), [`changes`](runner.md#TrainResult.changes), [`num_params_m`](runner.md#TrainResult.num_params_m), [`peak_vram_mb`](runner.md#TrainResult.peak_vram_mb), [`record`](runner.md#PlateauDetector.record), [`record`](runner.md#StepSizeCalibrator.record), [`training_seconds`](runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](runner.md#_is_infrastructure_error), [`get_elite_text`](runner.md#ElitePool.get_elite_text), [`get_momentum_text`](runner.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](runner.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](runner.md#PROPOSE_PROMPT), [`depth`](runner.md#TrainResult.depth), [`CrashMemory`](runner.md#CrashMemory), [`ElitePool`](runner.md#ElitePool)  (+6 more)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py:128`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L131)
  - `results` — [`L129`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner.md#TrainResult.val_bpb), [`TrainResult`](runner.md#TrainResult), [`status`](runner.md#TrainResult.status), [`description`](runner.md#TrainResult.description), [`iteration`](runner.md#TrainResult.iteration)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`trace`](runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L823) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L678)
- `logger` — [`L99`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_C/C3/runner.py#L99)

