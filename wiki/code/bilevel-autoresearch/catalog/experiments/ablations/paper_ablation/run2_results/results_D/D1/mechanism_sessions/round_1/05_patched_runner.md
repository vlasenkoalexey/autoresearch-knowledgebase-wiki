---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D1.mechanism_sessions.round_1.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  DiversityEnforcer.enforce_diversity: DiversityEnforcer#enforce_diversity().
  TrainRunner.search_config: TrainRunner#search_config.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
  DiversityEnforcer._normalize_config: DiversityEnforcer#_normalize_config().
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  DiversityEnforcer.min_distance_threshold: DiversityEnforcer#min_distance_threshold.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  DiversityEnforcer.PARAM_BOUNDS: DiversityEnforcer#PARAM_BOUNDS.
  TrainRunner.client: TrainRunner#client.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  TrainRunner.original_code: TrainRunner#original_code.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  TrainResult.depth: TrainResult#depth.
  TrainTrace.best_iteration: TrainTrace#best_iteration.
  PROPOSE_PROMPT: PROPOSE_PROMPT.
  DiversityEnforcer._compute_distance: DiversityEnforcer#_compute_distance().
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
  DiversityEnforcer.CATEGORICAL_OPTIONS: DiversityEnforcer#CATEGORICAL_OPTIONS.
  DiversityEnforcer.history_window: DiversityEnforcer#history_window.
  DiversityEnforcer.max_retries: DiversityEnforcer#max_retries.
  DiversityEnforcer.logger: DiversityEnforcer#logger.
  DiversityEnforcer._perturb_parameter: DiversityEnforcer#_perturb_parameter().
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  DiversityEnforcer: DiversityEnforcer#
  DiversityEnforcer.__init__: DiversityEnforcer#__init__().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py)

## Classes
### `DiversityEnforcer`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py:322`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L322)
- doc: Enforces diversity in hyperparameter proposals to avoid repetitive configurations.
- signature: `class DiversityEnforcer:`
- members:
  - `__init__(self, history_window: int = 5, min_distance_threshold: float = 0.3, max_retries: int = 3)` — [`L356`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L356) — Args:
  - `_compute_distance(self, norm_vec1: Dict[str, float], norm_vec2: Dict[str, float])` — [`L586`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L586) — Compute Euclidean distance between two normalized vectors.
  - `_normalize_config(self, config: Dict[str, Any])` — [`L518`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L518) — Normalize a configuration to [0,1] range.
  - `_perturb_parameter(self, param_name: str, original_value: Any, param_type: str, bounds: Optional[Tuple[float, float]], options: Optional[List[str]], norm_value: float, norm_closest: Optional[float])` — [`L602`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L602) — Apply targeted perturbation to a parameter.
  - `enforce_diversity(self, proposed_config: Dict[str, Any], recent_configs: List[Dict[str, Any]], iteration: int)` — [`L373`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L373) — Check if proposed config is sufficiently diverse from recent history.
  - `CATEGORICAL_OPTIONS` — [`L349`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L349)
  - `PARAM_BOUNDS` — [`L328`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L328)
  - `history_window` — [`L368`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L368)
  - `logger` — [`L371`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L371)
  - `max_retries` — [`L370`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L370)
  - `min_distance_threshold` — [`L369`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L369)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py:113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L122)
  - `description` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L116)
  - `status` — [`L119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L115)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py:663`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L663)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1193`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1193) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1335`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1335) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1237`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1237) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1202`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1202) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1349`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1349) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L998`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L998) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1247`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L1247) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L962`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L962) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L728`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L728) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L667`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L667)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L668`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L668)
  - `artifacts_dir` — [`L683`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L683)
  - `client` — [`L681`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L681)
  - `crash_memory` — [`L693`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L693)
  - `current_code` — [`L689`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L689)
  - `elite_pool` — [`L699`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L699)
  - `momentum` — [`L696`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L696)
  - `original_code` — [`L688`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L688)
  - `plateau_detector` — [`L705`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L705)
  - `search_config` — [`L682`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L682)
  - `simple_mode` — [`L684`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L684)
  - `step_calibrator` — [`L702`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L702)
  - `trace` — [`L690`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L690)
  - `train_py` — [`L679`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L679)
  - `work_dir` — [`L680`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L680)
- protocol/private: `__init__`[`L670`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L670), `_best_code`[`L724`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L724), `_crossover_frequency`[`L708`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L708), `_exploration_frequency`[`L712`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L712), `_iters_since_improvement`[`L725`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L725), `_max_acceptable_regression`[`L715`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L715), `_proposal_count`[`L709`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L709), `_sa_cooling_rate`[`L719`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L719), `_sa_initial_temp`[`L718`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L718), `_sa_iteration_count`[`L721`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L721), `_sa_temp`[`L720`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L720), `_stagnation_threshold`[`L726`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L726)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`TrainTrace`](05_patched_runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](05_patched_runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](05_patched_runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py:126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L129)
  - `results` — [`L127`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L150)
- `logger` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_1/05_patched_runner.py#L106)

