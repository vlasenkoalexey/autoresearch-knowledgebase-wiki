---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D2.mechanism_sessions.round_2.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrustRegionConstraint.update_region: TrustRegionConstraint#update_region().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  TrainRunner.search_config: TrainRunner#search_config.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  TrustRegionConstraint.constrain_proposal: TrustRegionConstraint#constrain_proposal().
  TrustRegionConstraint.get_region_status: TrustRegionConstraint#get_region_status().
  TrainResult.status: TrainResult#status.
  TrustRegionConstraint.radii: TrustRegionConstraint#radii.
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  TrustRegionConstraint.reset_region: TrustRegionConstraint#reset_region().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  TrustRegionConstraint.history: TrustRegionConstraint#history.
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  TrustRegionConstraint.initial_radii: TrustRegionConstraint#initial_radii.
  TrainRunner.client: TrainRunner#client.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  TrainRunner.original_code: TrainRunner#original_code.
  TrustRegionConstraint.logger: TrustRegionConstraint#logger.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  TrainResult.depth: TrainResult#depth.
  TrainTrace.best_iteration: TrainTrace#best_iteration.
  PROPOSE_PROMPT: PROPOSE_PROMPT.
  TrustRegionConstraint.min_radius: TrustRegionConstraint#min_radius.
  TrustRegionConstraint.max_radius: TrustRegionConstraint#max_radius.
  TrustRegionConstraint.success_count: TrustRegionConstraint#success_count.
  TrustRegionConstraint.total_updates: TrustRegionConstraint#total_updates.
  TrustRegionConstraint.bounded_params: TrustRegionConstraint#bounded_params.
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
  TrustRegionConstraint.contraction_factor: TrustRegionConstraint#contraction_factor.
  TrustRegionConstraint.expansion_factor: TrustRegionConstraint#expansion_factor.
  TrustRegionConstraint.success_threshold: TrustRegionConstraint#success_threshold.
  TrustRegionConstraint.log_scale_params: TrustRegionConstraint#log_scale_params.
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  TrustRegionConstraint: TrustRegionConstraint#
  TrustRegionConstraint.__init__: TrustRegionConstraint#__init__().
  TrustRegionConstraint.window_size: TrustRegionConstraint#window_size.
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py)

## Classes
### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py:113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L122)
  - `description` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L116)
  - `status` — [`L119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L115)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py:478`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L478)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1008`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1008) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1150) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1052`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1052) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1017`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1017) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1164`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1164) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L813`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L813) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1062`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L1062) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L777`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L777) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L543`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L543) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L482`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L482)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L483`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L483)
  - `artifacts_dir` — [`L498`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L498)
  - `client` — [`L496`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L496)
  - `crash_memory` — [`L508`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L508)
  - `current_code` — [`L504`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L504)
  - `elite_pool` — [`L514`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L514)
  - `momentum` — [`L511`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L511)
  - `original_code` — [`L503`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L503)
  - `plateau_detector` — [`L520`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L520)
  - `search_config` — [`L497`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L497)
  - `simple_mode` — [`L499`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L499)
  - `step_calibrator` — [`L517`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L517)
  - `trace` — [`L505`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L505)
  - `train_py` — [`L494`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L494)
  - `work_dir` — [`L495`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L495)
- protocol/private: `__init__`[`L485`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L485), `_best_code`[`L539`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L539), `_crossover_frequency`[`L523`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L523), `_exploration_frequency`[`L527`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L527), `_iters_since_improvement`[`L540`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L540), `_max_acceptable_regression`[`L530`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L530), `_proposal_count`[`L524`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L524), `_sa_cooling_rate`[`L534`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L534), `_sa_initial_temp`[`L533`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L533), `_sa_iteration_count`[`L536`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L536), `_sa_temp`[`L535`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L535), `_stagnation_threshold`[`L541`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L541)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`TrainTrace`](05_patched_runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](05_patched_runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](05_patched_runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py:126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L129)
  - `results` — [`L127`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

### `TrustRegionConstraint`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py:329`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L329)
- doc: Manages trust regions for hyperparameter exploration.
- signature: `class TrustRegionConstraint:`
- members:
  - `__init__(self, initial_radii: Dict[str, float], contraction_factor: float = 0.8, expansion_factor: float = 1.2, min_radius: Optional[Dict[str, float]] = None, max_radius: Optional[Dict[str, float]] = None, success_threshold: float = 0, window_size: int = 3)` — [`L332`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L332) — Args:
  - `constrain_proposal(self, current_params: Dict[str, float], proposed_params: Dict[str, float])` — [`L373`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L373) — Clip proposed parameters to stay within trust region of current best.
  - `get_region_status(self)` — [`L453`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L453) — Return current radii and success statistics for logging.
  - `reset_region(self, param: Optional[str] = None)` — [`L467`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L467) — Reset trust region for specific parameter or all parameters.
  - `update_region(self, current_params: Dict[str, float], new_params: Dict[str, float], improvement: float, iteration: int)` — [`L409`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L409) — Update trust radii based on success/failure of last step.
  - `bounded_params` — [`L368`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L368)
  - `contraction_factor` — [`L355`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L355)
  - `expansion_factor` — [`L356`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L356)
  - `history` — [`L362`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L362)
  - `initial_radii` — [`L354`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L354)
  - `log_scale_params` — [`L367`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L367)
  - `logger` — [`L365`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L365)
  - `max_radius` — [`L358`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L358)
  - `min_radius` — [`L357`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L357)
  - `radii` — [`L353`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L353)
  - `success_count` — [`L363`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L363)
  - `success_threshold` — [`L359`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L359)
  - `total_updates` — [`L364`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L364)
  - `window_size` — [`L360`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L360)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L150)
- `logger` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/mechanism_sessions/round_2/05_patched_runner.py#L106)

