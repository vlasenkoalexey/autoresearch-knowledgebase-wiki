---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D2.mechanism_sessions.round_1.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  GeneratedMechanism_20260324_142015._detect_phase_transition: GeneratedMechanism_20260324_142015#_detect_phase_transition().
  TrainRunner.search_config: TrainRunner#search_config.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  GeneratedMechanism_20260324_142015.update: GeneratedMechanism_20260324_142015#update().
  GeneratedMechanism_20260324_142015.get_specialized_instructions: GeneratedMechanism_20260324_142015#get_specialized_instructions().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  GeneratedMechanism_20260324_142015.discard_patterns: GeneratedMechanism_20260324_142015#discard_patterns.
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
  GeneratedMechanism_20260324_142015.history: GeneratedMechanism_20260324_142015#history.
  GeneratedMechanism_20260324_142015.phase: GeneratedMechanism_20260324_142015#phase.
  GeneratedMechanism_20260324_142015._update_discard_patterns: GeneratedMechanism_20260324_142015#_update_discard_patterns().
  GeneratedMechanism_20260324_142015._is_significant_improvement: GeneratedMechanism_20260324_142015#_is_significant_improvement().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  GeneratedMechanism_20260324_142015._get_recent_discard_summary: GeneratedMechanism_20260324_142015#_get_recent_discard_summary().
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  GeneratedMechanism_20260324_142015.iterations_in_current_phase: GeneratedMechanism_20260324_142015#iterations_in_current_phase.
  GeneratedMechanism_20260324_142015.improvements_in_phase: GeneratedMechanism_20260324_142015#improvements_in_phase.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  GeneratedMechanism_20260324_142015.stagnation_window: GeneratedMechanism_20260324_142015#stagnation_window.
  TrainRunner.client: TrainRunner#client.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  GeneratedMechanism_20260324_142015._get_stagnation_instructions: GeneratedMechanism_20260324_142015#_get_stagnation_instructions().
  GeneratedMechanism_20260324_142015._get_pattern_warnings: GeneratedMechanism_20260324_142015#_get_pattern_warnings().
  TrainRunner.original_code: TrainRunner#original_code.
  GeneratedMechanism_20260324_142015.last_phase_change: GeneratedMechanism_20260324_142015#last_phase_change.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  GeneratedMechanism_20260324_142015.get_phase: GeneratedMechanism_20260324_142015#get_phase().
  TrainResult.depth: TrainResult#depth.
  TrainTrace.best_iteration: TrainTrace#best_iteration.
  PROPOSE_PROMPT: PROPOSE_PROMPT.
  TrainRunner.QUICK_TEST_BUDGET: TrainRunner#QUICK_TEST_BUDGET.
  TrainRunner.QUICK_TEST_LOSS_THRESHOLD: TrainRunner#QUICK_TEST_LOSS_THRESHOLD.
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  TrainRunner._crossover_frequency: TrainRunner#_crossover_frequency.
  TrainRunner._max_acceptable_regression: TrainRunner#_max_acceptable_regression.
  TrainRunner._sa_iteration_count: TrainRunner#_sa_iteration_count.
  TrainRunner._apply_changes: TrainRunner#_apply_changes().
  TrainTrace: TrainTrace#
  MULTI_CANDIDATE_PROMPT: MULTI_CANDIDATE_PROMPT.
  PICK_CANDIDATE_PROMPT: PICK_CANDIDATE_PROMPT.
  INFRA_ERROR_PATTERNS: INFRA_ERROR_PATTERNS.
  GeneratedMechanism_20260324_142015.min_improvement: GeneratedMechanism_20260324_142015#min_improvement.
  GeneratedMechanism_20260324_142015._param_categories: GeneratedMechanism_20260324_142015#_param_categories.
  GeneratedMechanism_20260324_142015._get_exploration_instructions: GeneratedMechanism_20260324_142015#_get_exploration_instructions().
  GeneratedMechanism_20260324_142015._get_exploitation_instructions: GeneratedMechanism_20260324_142015#_get_exploitation_instructions().
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  GeneratedMechanism_20260324_142015: GeneratedMechanism_20260324_142015#
  GeneratedMechanism_20260324_142015.__init__: GeneratedMechanism_20260324_142015#__init__().
  GeneratedMechanism_20260324_142015.exploration_window: GeneratedMechanism_20260324_142015#exploration_window.
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py)

## Classes
### `GeneratedMechanism_20260324_142015`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py:323`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L323)
- doc: Adaptive Prompt Specializer: Dynamically adjusts LLM instructions based on
- signature: `class GeneratedMechanism_20260324_142015:`
- members:
  - `__init__(self, stagnation_window: int = 4, exploration_window: int = 3, min_improvement_threshold: float = 0.0003)` — [`L329`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L329) — Args:
  - `_detect_phase_transition(self, current_iteration: int)` — [`L432`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L432) — Determine current optimization phase based on recent history.
  - `_get_pattern_warnings(self)` — [`L545`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L545) — Generate warnings about repeated failure patterns.
  - `_get_recent_discard_summary(self)` — [`L531`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L531) — Get summary of recently failed parameters.
  - `_is_significant_improvement(self, recent_best: float)` — [`L473`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L473) — Check if recent improvement is significant compared to history.
  - `_update_discard_patterns(self, iteration: int, config: dict, discard_reason: str)` — [`L399`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L399) — Track patterns in failed parameter changes.
  - `get_phase(self)` — [`L570`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L570) — Return current phase: 'exploration', 'exploitation', or 'stagnation'.
  - `get_specialized_instructions(self)` — [`L489`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L489) — Return specialized prompt instructions based on current phase.
  - `update(self, iteration: int, result: Any, current_config: dict)` — [`L373`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L373) — Update internal state with latest iteration results.
  - `discard_patterns` — [`L351`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L351)
  - `exploration_window` — [`L342`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L342)
  - `history` — [`L346`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L346)
  - `improvements_in_phase` — [`L358`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L358)
  - `iterations_in_current_phase` — [`L357`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L357)
  - `last_phase_change` — [`L348`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L348)
  - `min_improvement` — [`L343`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L343)
  - `phase` — [`L347`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L347)
  - `stagnation_window` — [`L341`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L341)
- protocol/private: `_get_exploitation_instructions`[`L515`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L515), `_get_exploration_instructions`[`L508`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L508), `_get_stagnation_instructions`[`L522`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L522), `_param_categories`[`L361`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L361)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py:113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L122)
  - `description` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L116)
  - `status` — [`L119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L115)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py:576`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L576)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1106) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1248`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1248) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1150) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1115) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1262`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1262) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L911`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L911) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1160`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L1160) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L875`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L875) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L641`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L641) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L580`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L580)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L581`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L581)
  - `artifacts_dir` — [`L596`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L596)
  - `client` — [`L594`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L594)
  - `crash_memory` — [`L606`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L606)
  - `current_code` — [`L602`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L602)
  - `elite_pool` — [`L612`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L612)
  - `momentum` — [`L609`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L609)
  - `original_code` — [`L601`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L601)
  - `plateau_detector` — [`L618`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L618)
  - `search_config` — [`L595`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L595)
  - `simple_mode` — [`L597`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L597)
  - `step_calibrator` — [`L615`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L615)
  - `trace` — [`L603`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L603)
  - `train_py` — [`L592`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L592)
  - `work_dir` — [`L593`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L593)
- protocol/private: `__init__`[`L583`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L583), `_best_code`[`L637`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L637), `_crossover_frequency`[`L621`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L621), `_exploration_frequency`[`L625`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L625), `_iters_since_improvement`[`L638`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L638), `_max_acceptable_regression`[`L628`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L628), `_proposal_count`[`L622`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L622), `_sa_cooling_rate`[`L632`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L632), `_sa_initial_temp`[`L631`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L631), `_sa_iteration_count`[`L634`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L634), `_sa_temp`[`L633`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L633), `_stagnation_threshold`[`L639`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L639)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`TrainTrace`](05_patched_runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](05_patched_runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](05_patched_runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py:126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L129)
  - `results` — [`L127`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L150)
- `logger` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_1/05_patched_runner.py#L106)

