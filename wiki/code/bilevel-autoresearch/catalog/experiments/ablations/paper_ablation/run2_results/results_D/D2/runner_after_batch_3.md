---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D2.runner_after_batch_3`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  TrainRunner.search_config: TrainRunner#search_config.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
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
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
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
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py)

## Classes
### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py:113`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L122)
  - `description` — [`L121`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L116)
  - `status` — [`L119`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L115)
- used by: [`run_iteration`](runner_after_batch_3.md#TrainRunner.run_iteration), [`run_baseline`](runner_after_batch_3.md#TrainRunner.run_baseline), [`add`](runner_after_batch_3.md#TrainTrace.add), [`summary`](runner_after_batch_3.md#TrainTrace.summary), [`results`](runner_after_batch_3.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py:312`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L312)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L842`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L842) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L984`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L984) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L886`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L886) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L851`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L851) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L998`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L998) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L647`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L647) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L896`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L896) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L611`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L611) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L377`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L377) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L316`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L316)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L317`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L317)
  - `artifacts_dir` — [`L332`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L332)
  - `client` — [`L330`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L330)
  - `crash_memory` — [`L342`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L342)
  - `current_code` — [`L338`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L338)
  - `elite_pool` — [`L348`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L348)
  - `momentum` — [`L345`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L345)
  - `original_code` — [`L337`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L337)
  - `plateau_detector` — [`L354`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L354)
  - `search_config` — [`L331`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L331)
  - `simple_mode` — [`L333`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L333)
  - `step_calibrator` — [`L351`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L351)
  - `trace` — [`L339`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L339)
  - `train_py` — [`L328`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L328)
  - `work_dir` — [`L329`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L329)
- protocol/private: `__init__`[`L319`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L319), `_best_code`[`L373`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L373), `_crossover_frequency`[`L357`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L357), `_exploration_frequency`[`L361`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L361), `_iters_since_improvement`[`L374`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L374), `_max_acceptable_regression`[`L364`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L364), `_proposal_count`[`L358`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L358), `_sa_cooling_rate`[`L368`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L368), `_sa_initial_temp`[`L367`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L367), `_sa_iteration_count`[`L370`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L370), `_sa_temp`[`L369`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L369), `_stagnation_threshold`[`L375`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L375)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](runner_after_batch_3.md#logger), [`add`](runner_after_batch_3.md#TrainTrace.add), [`summary`](runner_after_batch_3.md#TrainTrace.summary), [`best_bpb`](runner_after_batch_3.md#TrainTrace.best_bpb), [`val_bpb`](runner_after_batch_3.md#TrainResult.val_bpb), [`TrainResult`](runner_after_batch_3.md#TrainResult), [`status`](runner_after_batch_3.md#TrainResult.status), [`description`](runner_after_batch_3.md#TrainResult.description), [`iteration`](runner_after_batch_3.md#TrainResult.iteration), [`changes`](runner_after_batch_3.md#TrainResult.changes), [`num_params_m`](runner_after_batch_3.md#TrainResult.num_params_m), [`peak_vram_mb`](runner_after_batch_3.md#TrainResult.peak_vram_mb), [`training_seconds`](runner_after_batch_3.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](runner_after_batch_3.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](runner_after_batch_3.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](runner_after_batch_3.md#PROPOSE_PROMPT), [`depth`](runner_after_batch_3.md#TrainResult.depth), [`TrainTrace`](runner_after_batch_3.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](runner_after_batch_3.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](runner_after_batch_3.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py:126`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L129)
  - `results` — [`L127`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner_after_batch_3.md#TrainResult.val_bpb), [`TrainResult`](runner_after_batch_3.md#TrainResult), [`status`](runner_after_batch_3.md#TrainResult.status), [`description`](runner_after_batch_3.md#TrainResult.description), [`iteration`](runner_after_batch_3.md#TrainResult.iteration)
- used by: [`run_iteration`](runner_after_batch_3.md#TrainRunner.run_iteration), [`_propose`](runner_after_batch_3.md#TrainRunner._propose), [`run_baseline`](runner_after_batch_3.md#TrainRunner.run_baseline), [`trace`](runner_after_batch_3.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L150)
- `logger` — [`L106`](../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D2/runner_after_batch_3.py#L106)

