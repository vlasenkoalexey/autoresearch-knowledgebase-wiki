---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_B.B3.runner`/
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
  ElitePool._pool: ElitePool#_pool.
  TrainRunner.search_config: TrainRunner#search_config.
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
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  StepSizeCalibrator._history: StepSizeCalibrator#_history.
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
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
  TrainRunner.original_code: TrainRunner#original_code.
  CrashRecord: CrashRecord#
  MomentumTracker._signals: MomentumTracker#_signals.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  CrashMemory.crash_count: CrashMemory#crash_count().
  ElitePool.best_bpb: ElitePool#best_bpb().
  TrainRunner.__init__: TrainRunner#__init__().
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
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py)

## Classes
### `CrashMemory`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:152`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L152)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L179`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L179)
  - `get_warning_text(self)` — [`L182`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L182) — Generate a warning block to inject into the proposal prompt.
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L165`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L165) — Record a crash caused by the given parameter changes.
- protocol/private: `__init__`[`L160`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L160), `_crashes`[`L161`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L161), `_param_crash_counts`[`L163`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L163)
- uses (calls/refs, reference-scoped): [`logger`](runner.md#logger), [`CrashRecord`](runner.md#CrashRecord), [`error_hint`](runner.md#CrashRecord.error_hint), [`param`](runner.md#CrashRecord.param), [`value`](runner.md#CrashRecord.value), [`iteration`](runner.md#CrashRecord.iteration)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`crash_memory`](runner.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:119`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L119)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L124`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L124)
  - `iteration` — [`L123`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L123)
  - `param` — [`L121`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L121)
  - `value` — [`L122`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L122)
- used by: [`record`](runner.md#CrashMemory.record), [`get_warning_text`](runner.md#CrashMemory.get_warning_text), [`_crashes`](runner.md#CrashMemory._crashes)

### `ElitePool`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:529`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L529)
- doc: Maintains a pool of the top-K configs seen during search.
- signature: `class ElitePool:`
- members:
  - `add(self, val_bpb: float, config: dict, iteration: int, description: str)` — [`L543`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L543) — Add a config to the pool if it qualifies.
  - `best_bpb(self)` — [`L553`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L553)
  - `generate_crossover(self, current_config: dict, active_params: list[str])` — [`L600`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L600) — Generate a crossover candidate by interpolating between top-2 elite configs.
  - `get_elite_text(self)` — [`L558`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L558) — Generate a summary of elite configs for the proposal prompt.
- protocol/private: `_EXPRESSION_PARAMS`[`L596`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L596), `_INTEGER_PARAMS`[`L598`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L598), `__init__`[`L538`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L538), `_max_size`[`L539`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L539), `_pool`[`L541`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L541)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`elite_pool`](runner.md#TrainRunner.elite_pool)

### `MomentumTracker`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:222`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L222)
- doc: Tracks which parameter change directions have led to improvements.
- signature: `class MomentumTracker:`
- members:
  - `_detect_direction(self, param: str, old_val: str, new_val)` — [`L259`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L259) — Detect whether a parameter was increased or decreased.
  - `get_momentum_text(self)` — [`L272`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L272) — Generate a momentum summary to inject into the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L237`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L237) — Record the outcome of a parameter change.
- protocol/private: `__init__`[`L231`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L231), `_signals`[`L235`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L235)
- uses (calls/refs, reference-scoped): [`logger`](runner.md#logger)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`momentum`](runner.md#TrainRunner.momentum)

### `PlateauDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:439`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L439)
- doc: Detects when the search is stuck on the same parameter set with diminishing returns.
- signature: `class PlateauDetector:`
- members:
  - `check_plateau(self)` — [`L467`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L467) — Check if we're on a plateau. Returns (is_plateau, directive_text).
  - `record(self, changes: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L458`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L458) — Record a proposal outcome.
- protocol/private: `__init__`[`L450`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L450), `_diversification_active`[`L455`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L455), `_min_improvement_threshold`[`L452`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L452), `_recent`[`L454`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L454), `_recently_plateaued_params`[`L456`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L456), `_window`[`L451`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L451)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`plateau_detector`](runner.md#TrainRunner.plateau_detector)

### `StepSizeCalibrator`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:344`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L344)
- doc: Tracks successful vs failed change magnitudes per parameter.
- signature: `class StepSizeCalibrator:`
- members:
  - `_compute_relative_change(self, old_val, new_val)` — [`L374`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L374) — Compute relative change as a percentage.
  - `get_step_size_text(self)` — [`L385`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L385) — Generate step-size recommendations for the proposal prompt.
  - `record(self, changes: dict, old_config: dict, val_bpb: float, best_bpb_before: float, status: str)` — [`L355`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L355) — Record the magnitude of a parameter change and its outcome.
- protocol/private: `__init__`[`L351`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L351), `_history`[`L353`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L353)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`step_calibrator`](runner.md#TrainRunner.step_calibrator)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L106)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L113`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L113)
  - `depth` — [`L115`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L115)
  - `description` — [`L114`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L114)
  - `iteration` — [`L107`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L107)
  - `num_params_m` — [`L111`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L111)
  - `peak_vram_mb` — [`L109`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L109)
  - `status` — [`L112`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L112)
  - `training_seconds` — [`L110`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L110)
  - `val_bpb` — [`L108`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L108)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`add`](runner.md#TrainTrace.add), [`summary`](runner.md#TrainTrace.summary), [`results`](runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:840`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L840)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1370`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1370) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1508`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1508) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1414`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1414) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1379`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1379) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1522`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1522) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1175`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1175) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1424`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1424) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L1139`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L1139) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L905`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L905) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L844`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L844)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L845`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L845)
  - `artifacts_dir` — [`L860`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L860)
  - `client` — [`L858`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L858)
  - `crash_memory` — [`L870`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L870)
  - `current_code` — [`L866`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L866)
  - `elite_pool` — [`L876`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L876)
  - `momentum` — [`L873`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L873)
  - `original_code` — [`L865`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L865)
  - `plateau_detector` — [`L882`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L882)
  - `search_config` — [`L859`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L859)
  - `simple_mode` — [`L861`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L861)
  - `step_calibrator` — [`L879`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L879)
  - `trace` — [`L867`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L867)
  - `train_py` — [`L856`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L856)
  - `work_dir` — [`L857`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L857)
- protocol/private: `__init__`[`L847`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L847), `_best_code`[`L901`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L901), `_crossover_frequency`[`L885`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L885), `_exploration_frequency`[`L889`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L889), `_iters_since_improvement`[`L902`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L902), `_max_acceptable_regression`[`L892`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L892), `_proposal_count`[`L886`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L886), `_sa_cooling_rate`[`L896`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L896), `_sa_initial_temp`[`L895`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L895), `_sa_iteration_count`[`L898`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L898), `_sa_temp`[`L897`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L897), `_stagnation_threshold`[`L903`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L903)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../core/llm_client.md#LLMClient.call), [`LLMClient`](../../../../../../core/llm_client.md#LLMClient), [`logger`](runner.md#logger), [`record`](runner.md#CrashMemory.record), [`add`](runner.md#TrainTrace.add), [`summary`](runner.md#TrainTrace.summary), [`best_bpb`](runner.md#TrainTrace.best_bpb), [`check_plateau`](runner.md#PlateauDetector.check_plateau), [`get_warning_text`](runner.md#CrashMemory.get_warning_text), [`val_bpb`](runner.md#TrainResult.val_bpb), [`TrainResult`](runner.md#TrainResult), [`status`](runner.md#TrainResult.status), [`generate_crossover`](runner.md#ElitePool.generate_crossover), [`record`](runner.md#MomentumTracker.record), [`description`](runner.md#TrainResult.description), [`iteration`](runner.md#TrainResult.iteration), [`add`](runner.md#ElitePool.add), [`changes`](runner.md#TrainResult.changes), [`num_params_m`](runner.md#TrainResult.num_params_m), [`peak_vram_mb`](runner.md#TrainResult.peak_vram_mb), [`record`](runner.md#PlateauDetector.record), [`record`](runner.md#StepSizeCalibrator.record), [`training_seconds`](runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](runner.md#_is_infrastructure_error), [`get_elite_text`](runner.md#ElitePool.get_elite_text), [`get_momentum_text`](runner.md#MomentumTracker.get_momentum_text), [`get_step_size_text`](runner.md#StepSizeCalibrator.get_step_size_text), [`PROPOSE_PROMPT`](runner.md#PROPOSE_PROMPT), [`depth`](runner.md#TrainResult.depth), [`CrashMemory`](runner.md#CrashMemory), [`ElitePool`](runner.md#ElitePool), [`MomentumTracker`](runner.md#MomentumTracker), [`PlateauDetector`](runner.md#PlateauDetector), [`StepSizeCalibrator`](runner.md#StepSizeCalibrator), [`TrainTrace`](runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py:128`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L128)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L133`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L133)
  - `summary(self, last_n: int = 10)` — [`L139`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L139)
  - `best_bpb` — [`L130`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L130)
  - `best_iteration` — [`L131`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L131)
  - `results` — [`L129`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L129)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner.md#TrainResult.val_bpb), [`TrainResult`](runner.md#TrainResult), [`status`](runner.md#TrainResult.status), [`description`](runner.md#TrainResult.description), [`iteration`](runner.md#TrainResult.iteration)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`trace`](runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L823`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L823) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L812`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L812)
- `MULTI_CANDIDATE_PROMPT` — [`L723`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L723)
- `PICK_CANDIDATE_PROMPT` — [`L784`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L784)
- `PROPOSE_PROMPT` — [`L683`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L683)
- `PROPOSE_SYSTEM` — [`L678`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L678)
- `logger` — [`L99`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_B/B3/runner.py#L99)

