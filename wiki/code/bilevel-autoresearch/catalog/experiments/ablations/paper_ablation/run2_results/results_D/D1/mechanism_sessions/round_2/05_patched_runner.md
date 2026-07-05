---
title: 'Module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py'
type: catalog
provenance: extracted
module: experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `experiments.ablations.paper_ablation.run2_results.results_D.D1.mechanism_sessions.round_2.05_patched_runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrainTrace.add: TrainTrace#add().
  TrainRunner.trace: TrainRunner#trace.
  TrainTrace.summary: TrainTrace#summary().
  FixationDetector.proposal_history: FixationDetector#proposal_history.
  TrainRunner.search_config: TrainRunner#search_config.
  FixationDetector.check_fixation: FixationDetector#check_fixation().
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  TrainRunner.current_code: TrainRunner#current_code.
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainResult: TrainResult#
  FixationDetector.add_proposal: FixationDetector#add_proposal().
  TrainResult.status: TrainResult#status.
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult.description: TrainResult#description.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  FixationDetector.get_intervention_suggestion: FixationDetector#get_intervention_suggestion().
  FixationDetector.reset: FixationDetector#reset().
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainResult.changes: TrainResult#changes.
  FixationDetector._identify_fixated_parameter: FixationDetector#_identify_fixated_parameter().
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  FixationDetector.fixation_counter: FixationDetector#fixation_counter.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainTrace.results: TrainTrace#results.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  FixationDetector.window_size: FixationDetector#window_size.
  FixationDetector.iteration_history: FixationDetector#iteration_history.
  TrainRunner.client: TrainRunner#client.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  FixationDetector._detect_directional_pattern: FixationDetector#_detect_directional_pattern().
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
  FixationDetector.similarity_threshold: FixationDetector#similarity_threshold.
  FixationDetector.max_repetitions: FixationDetector#max_repetitions.
  FixationDetector._clean_proposal: FixationDetector#_clean_proposal().
  FixationDetector._jaccard_similarity: FixationDetector#_jaccard_similarity().
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
  FixationDetector: FixationDetector#
  FixationDetector.__init__: FixationDetector#__init__().
  TrainRunner: TrainRunner#
---
# Module: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py)

## Classes
### `FixationDetector`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py:319`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L319)
- doc: Detects when the LLM is stuck proposing similar parameter changes repeatedly.
- signature: `class FixationDetector:`
- members:
  - `__init__(self, window_size: int = 5, similarity_threshold: float = 0.7, max_repetitions: int = 3)` — [`L323`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L323) — window_size: How many recent proposals to track
  - `_clean_proposal(self, proposal_text: str)` — [`L426`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L426) — Clean proposal text and extract parameter changes
  - `_detect_directional_pattern(self)` — [`L507`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L507) — Detect if proposals show a consistent directional pattern
  - `_identify_fixated_parameter(self)` — [`L485`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L485) — Identify the most common parameter in recent proposals
  - `_jaccard_similarity(self, text1: str, text2: str)` — [`L470`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L470) — Compute Jaccard similarity between two texts based on tokens
  - `add_proposal(self, proposal_text: str, iteration: int)` — [`L342`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L342) — Record a new proposal for analysis
  - `check_fixation(self)` — [`L353`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L353) — Returns:
  - `get_intervention_suggestion(self)` — [`L392`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L392) — Returns a concrete suggestion to break the fixation pattern
  - `reset(self)` — [`L420`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L420) — Clear history after successful intervention
  - `fixation_counter` — [`L340`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L340)
  - `iteration_history` — [`L339`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L339)
  - `max_repetitions` — [`L336`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L336)
  - `proposal_history` — [`L338`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L338)
  - `similarity_threshold` — [`L335`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L335)
  - `window_size` — [`L334`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L334)

### `TrainResult`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py:113`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L113)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L120`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L120)
  - `depth` — [`L122`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L122)
  - `description` — [`L121`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L121)
  - `iteration` — [`L114`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L114)
  - `num_params_m` — [`L118`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L118)
  - `peak_vram_mb` — [`L116`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L116)
  - `status` — [`L119`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L119)
  - `training_seconds` — [`L117`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L117)
  - `val_bpb` — [`L115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L115)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`results`](05_patched_runner.md#TrainTrace.results)

### `TrainRunner`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py:531`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L531)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1061`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1061) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1203`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1203) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1105`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1105) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1070`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1070) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1217`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1217) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L866`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L866) — Ask LLM to propose hyperparameter changes.
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1115`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L1115) — Execute train.py and parse results. Returns None on crash.
  - `run_baseline(self)` — [`L830`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L830) — Run the unmodified train.py to establish baseline.
  - `run_iteration(self, iteration: int)` — [`L596`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L596) — Run one inner loop iteration.
  - `QUICK_TEST_BUDGET` — [`L535`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L535)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L536`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L536)
  - `artifacts_dir` — [`L551`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L551)
  - `client` — [`L549`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L549)
  - `crash_memory` — [`L561`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L561)
  - `current_code` — [`L557`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L557)
  - `elite_pool` — [`L567`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L567)
  - `momentum` — [`L564`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L564)
  - `original_code` — [`L556`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L556)
  - `plateau_detector` — [`L573`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L573)
  - `search_config` — [`L550`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L550)
  - `simple_mode` — [`L552`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L552)
  - `step_calibrator` — [`L570`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L570)
  - `trace` — [`L558`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L558)
  - `train_py` — [`L547`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L547)
  - `work_dir` — [`L548`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L548)
- protocol/private: `__init__`[`L538`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L538), `_best_code`[`L592`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L592), `_crossover_frequency`[`L576`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L576), `_exploration_frequency`[`L580`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L580), `_iters_since_improvement`[`L593`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L593), `_max_acceptable_regression`[`L583`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L583), `_proposal_count`[`L577`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L577), `_sa_cooling_rate`[`L587`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L587), `_sa_initial_temp`[`L586`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L586), `_sa_iteration_count`[`L589`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L589), `_sa_temp`[`L588`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L588), `_stagnation_threshold`[`L594`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L594)
- uses (calls/refs, reference-scoped): [`active_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.active_params), [`parse_json_response`](../../../../../../../../core/llm_client.md#parse_json_response), [`call`](../../../../../../../../core/llm_client.md#LLMClient.call), [`SearchConfig`](../../../../../../../../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../../../../../../../../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../../../../../../../../domains/train_opt/config.md#SearchConfig.strategy), [`LLMClient`](../../../../../../../../core/llm_client.md#LLMClient), [`time_budget`](../../../../../../../../domains/train_opt/config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](../../../../../../../../domains/train_opt/config.md#HYPERPARAM_NAMES), [`guidance`](../../../../../../../../domains/train_opt/config.md#SearchConfig.guidance), [`logger`](05_patched_runner.md#logger), [`add`](05_patched_runner.md#TrainTrace.add), [`summary`](05_patched_runner.md#TrainTrace.summary), [`best_bpb`](05_patched_runner.md#TrainTrace.best_bpb), [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration), [`changes`](05_patched_runner.md#TrainResult.changes), [`num_params_m`](05_patched_runner.md#TrainResult.num_params_m), [`peak_vram_mb`](05_patched_runner.md#TrainResult.peak_vram_mb), [`training_seconds`](05_patched_runner.md#TrainResult.training_seconds), [`PROPOSE_SYSTEM`](05_patched_runner.md#PROPOSE_SYSTEM), [`_is_infrastructure_error`](05_patched_runner.md#_is_infrastructure_error), [`PROPOSE_PROMPT`](05_patched_runner.md#PROPOSE_PROMPT), [`depth`](05_patched_runner.md#TrainResult.depth), [`TrainTrace`](05_patched_runner.md#TrainTrace), [`MULTI_CANDIDATE_PROMPT`](05_patched_runner.md#MULTI_CANDIDATE_PROMPT), [`PICK_CANDIDATE_PROMPT`](05_patched_runner.md#PICK_CANDIDATE_PROMPT)

### `TrainTrace`
- def: [`experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py:126`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L126)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L131`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L131)
  - `summary(self, last_n: int = 10)` — [`L137`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L137)
  - `best_bpb` — [`L128`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L128)
  - `best_iteration` — [`L129`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L129)
  - `results` — [`L127`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L127)
- uses (calls/refs, reference-scoped): [`val_bpb`](05_patched_runner.md#TrainResult.val_bpb), [`TrainResult`](05_patched_runner.md#TrainResult), [`status`](05_patched_runner.md#TrainResult.status), [`description`](05_patched_runner.md#TrainResult.description), [`iteration`](05_patched_runner.md#TrainResult.iteration)
- used by: [`run_iteration`](05_patched_runner.md#TrainRunner.run_iteration), [`_propose`](05_patched_runner.md#TrainRunner._propose), [`run_baseline`](05_patched_runner.md#TrainRunner.run_baseline), [`trace`](05_patched_runner.md#TrainRunner.trace)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L295`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L295) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L284`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L284)
- `MULTI_CANDIDATE_PROMPT` — [`L195`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L195)
- `PICK_CANDIDATE_PROMPT` — [`L256`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L256)
- `PROPOSE_PROMPT` — [`L155`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L155)
- `PROPOSE_SYSTEM` — [`L150`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L150)
- `logger` — [`L106`](../../../../../../../../../../../../raw/code/bilevel-autoresearch/experiments/ablations/paper_ablation/run2_results/results_D/D1/mechanism_sessions/round_2/05_patched_runner.py#L106)

