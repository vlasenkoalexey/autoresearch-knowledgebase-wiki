---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D3.mechanism_sessions.round_1.05_patched_runner`/
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
  StaleProposalDetector.record_outcome: StaleProposalDetector#record_outcome().
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  StaleProposalDetector.reset: StaleProposalDetector#reset().
  TrainResult: TrainResult#
  TrainResult.status: TrainResult#status.
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  StaleProposalDetector.record_proposal: StaleProposalDetector#record_proposal().
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
  StaleProposalDetector._last_proposed_params: StaleProposalDetector#_last_proposed_params.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  StaleProposalDetector._is_stale: StaleProposalDetector#_is_stale.
  TrainRunner.client: TrainRunner#client.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  TrainRunner.original_code: TrainRunner#original_code.
  StaleProposalDetector._discard_count: StaleProposalDetector#_discard_count.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  StaleProposalDetector.is_stale: StaleProposalDetector#is_stale().
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
  StaleProposalDetector.consecutive_discards_threshold: StaleProposalDetector#consecutive_discards_threshold.
  StaleProposalDetector.reset_on_any_accept: StaleProposalDetector#reset_on_any_accept.
  StaleProposalDetector.reset_on_parameter_change: StaleProposalDetector#reset_on_parameter_change.
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  StaleProposalDetector: StaleProposalDetector#
  StaleProposalDetector.__init__: StaleProposalDetector#__init__().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py)

## Classes
### `StaleProposalDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py:315`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L315)
- doc: Detects when the proposal stream is stuck in a discard loop.
- signature: `class StaleProposalDetector:`
- members:
  - `__init__(self, consecutive_discards_threshold: int = 3, reset_on_any_accept: bool = True, reset_on_parameter_change: bool = True)` — [`L324`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L324) — Args:
  - `is_stale(self)` — [`L385`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L385) — Returns True if the detector believes the proposal stream is stale
  - `record_outcome(self, accepted: bool)` — [`L368`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L368) — Update state based on whether the proposal was accepted or discarded.
  - `record_proposal(self, proposed_params: dict[str, float])` — [`L347`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L347) — Store the hyperparameters of the newly generated proposal.
  - `reset(self)` — [`L392`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L392) — Manually reset the detector (e.g., after a forced exploration move).
  - `consecutive_discards_threshold` — [`L339`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L339)
  - `reset_on_any_accept` — [`L340`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L340)
  - `reset_on_parameter_change` — [`L341`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L341)
- protocol/private: `_discard_count`[`L343`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L343), `_is_stale`[`L345`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L345), `_last_proposed_params`[`L344`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L344)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py:113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L122)
  - `description` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L116)
  - `status` — [`L119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L115)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py:402`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L402)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L932`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L932) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1074`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L1074) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L976`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L976) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L941`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L941) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1088`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L1088) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L737`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L737) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L986`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L986) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L701`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L701) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L467`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L467) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L406`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L406)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L407`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L407)
  - `artifacts_dir` — [`L422`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L422)
  - `client` — [`L420`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L420)
  - `crash_memory` — [`L432`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L432)
  - `current_code` — [`L428`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L428)
  - `elite_pool` — [`L438`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L438)
  - `momentum` — [`L435`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L435)
  - `original_code` — [`L427`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L427)
  - `plateau_detector` — [`L444`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L444)
  - `search_config` — [`L421`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L421)
  - `simple_mode` — [`L423`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L423)
  - `step_calibrator` — [`L441`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L441)
  - `trace` — [`L429`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L429)
  - `train_py` — [`L418`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L418)
  - `work_dir` — [`L419`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L419)
- protocol/private: `__init__`[`L409`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L409), `_best_code`[`L463`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L463), `_crossover_frequency`[`L447`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L447), `_exploration_frequency`[`L451`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L451), `_iters_since_improvement`[`L464`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L464), `_max_acceptable_regression`[`L454`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L454), `_proposal_count`[`L448`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L448), `_sa_cooling_rate`[`L458`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L458), `_sa_initial_temp`[`L457`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L457), `_sa_iteration_count`[`L460`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L460), `_sa_temp`[`L459`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L459), `_stagnation_threshold`[`L465`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L465)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`TrainTrace`](05_patched_runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](05_patched_runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](05_patched_runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py:126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L129)
  - `results` — [`L127`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L150)
- `logger` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D3/mechanism_sessions/round_1/05_patched_runner.py#L106)

