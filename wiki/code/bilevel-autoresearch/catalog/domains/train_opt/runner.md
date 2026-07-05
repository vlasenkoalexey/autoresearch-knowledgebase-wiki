---
title: 'Module: domains/train_opt/runner.py'
type: catalog
provenance: extracted
module: domains/train_opt/runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.runner`/
symbols:
  TrainRunner.run_iteration: TrainRunner#run_iteration().
  TrainRunner._propose: TrainRunner#_propose().
  TrainRunner.run_baseline: TrainRunner#run_baseline().
  logger: logger.
  TrainRunner.search_config: TrainRunner#search_config.
  TrainTrace.add: TrainTrace#add().
  TrainResult.val_bpb: TrainResult#val_bpb.
  TrainRunner.trace: TrainRunner#trace.
  TrainResult.status: TrainResult#status.
  TrainTrace.best_bpb: TrainTrace#best_bpb.
  TrainTrace.results: TrainTrace#results.
  TrainRunner._run_training: TrainRunner#_run_training().
  TrainTrace.summary: TrainTrace#summary().
  TrainResult.description: TrainResult#description.
  TrainResult.iteration: TrainResult#iteration.
  TrainResult: TrainResult#
  TrainRunner.current_code: TrainRunner#current_code.
  TrainTrace: TrainTrace#
  TrainTrace.best_iteration: TrainTrace#best_iteration.
  TrainRunner.simple_mode: TrainRunner#simple_mode.
  TrainResult.changes: TrainResult#changes.
  TrainRunner.elite_pool: TrainRunner#elite_pool.
  TrainRunner: TrainRunner#
  TrainRunner.knockout_screen: TrainRunner#knockout_screen.
  TrainRunner._sa_temp: TrainRunner#_sa_temp.
  TrainResult.num_params_m: TrainResult#num_params_m.
  TrainRunner._proposal_count: TrainRunner#_proposal_count.
  TrainRunner._inject_time_budget: TrainRunner#_inject_time_budget().
  TrainRunner.artifacts_dir: TrainRunner#artifacts_dir.
  TrainRunner.target_of_opportunity: TrainRunner#target_of_opportunity.
  TrainRunner._extract_hyperparams: TrainRunner#_extract_hyperparams().
  TrainResult.peak_vram_mb: TrainResult#peak_vram_mb.
  TrainResult.training_seconds: TrainResult#training_seconds.
  TrainRunner.crash_memory: TrainRunner#crash_memory.
  TrainRunner.grn: TrainRunner#grn.
  TrainRunner.excavation_grid: TrainRunner#excavation_grid.
  TrainRunner.work_dir: TrainRunner#work_dir.
  TrainRunner._iters_since_improvement: TrainRunner#_iters_since_improvement.
  TrainRunner._extract_changes_from_file: TrainRunner#_extract_changes_from_file().
  TrainRunner.momentum: TrainRunner#momentum.
  TrainRunner.fossil_record: TrainRunner#fossil_record.
  TrainRunner.seasonal_cycling: TrainRunner#seasonal_cycling.
  TrainRunner.spectral_decomposition: TrainRunner#spectral_decomposition.
  TrainRunner.back_translation: TrainRunner#back_translation.
  TrainRunner.__init__: TrainRunner#__init__().
  TrainRunner.step_calibrator: TrainRunner#step_calibrator.
  TrainRunner.plateau_detector: TrainRunner#plateau_detector.
  TrainRunner.epistasis_map: TrainRunner#epistasis_map.
  TrainRunner.transgenic: TrainRunner#transgenic.
  TrainRunner.stratigraphy: TrainRunner#stratigraphy.
  TrainRunner.context_stratigraphy: TrainRunner#context_stratigraphy.
  TrainRunner.compost_heap: TrainRunner#compost_heap.
  TrainRunner.soil_health: TrainRunner#soil_health.
  TrainRunner.perennial_classifier: TrainRunner#perennial_classifier.
  TrainRunner.survey_tiling: TrainRunner#survey_tiling.
  TrainRunner.adaptive_optics: TrainRunner#adaptive_optics.
  TrainRunner.parallax_estimator: TrainRunner#parallax_estimator.
  TrainRunner.semantic_equivalence: TrainRunner#semantic_equivalence.
  TrainRunner.register_adaptation: TrainRunner#register_adaptation.
  TrainRunner.domestication: TrainRunner#domestication.
  TrainRunner.post_editing: TrainRunner#post_editing.
  TrainResult.depth: TrainResult#depth.
  PROPOSE_SYSTEM: PROPOSE_SYSTEM.
  TrainRunner.client: TrainRunner#client.
  TrainRunner._best_code: TrainRunner#_best_code.
  _is_infrastructure_error: _is_infrastructure_error().
  TrainRunner.original_code: TrainRunner#original_code.
  TrainRunner._sa_initial_temp: TrainRunner#_sa_initial_temp.
  PROPOSE_PROMPT: PROPOSE_PROMPT.
  TrainRunner.QUICK_TEST_BUDGET: TrainRunner#QUICK_TEST_BUDGET.
  TrainRunner.QUICK_TEST_LOSS_THRESHOLD: TrainRunner#QUICK_TEST_LOSS_THRESHOLD.
  TrainRunner._crossover_frequency: TrainRunner#_crossover_frequency.
  TrainRunner._max_acceptable_regression: TrainRunner#_max_acceptable_regression.
  TrainRunner._sa_iteration_count: TrainRunner#_sa_iteration_count.
  TrainRunner._apply_changes: TrainRunner#_apply_changes().
  MULTI_CANDIDATE_PROMPT: MULTI_CANDIDATE_PROMPT.
  PICK_CANDIDATE_PROMPT: PICK_CANDIDATE_PROMPT.
  INFRA_ERROR_PATTERNS: INFRA_ERROR_PATTERNS.
  TrainRunner.train_py: TrainRunner#train_py.
  TrainRunner._knockout_frequency: TrainRunner#_knockout_frequency.
  TrainRunner._exploration_frequency: TrainRunner#_exploration_frequency.
  TrainRunner._sa_cooling_rate: TrainRunner#_sa_cooling_rate.
  TrainRunner._stagnation_threshold: TrainRunner#_stagnation_threshold.
  TrainRunner._parse_results: TrainRunner#_parse_results().
---
# Module: [`domains/train_opt/runner.py`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py)

## Classes
### `TrainResult`
- def: [`domains/train_opt/runner.py:210`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L210) — documented in [domains-train_opt-runner](../../../concepts/domains-train_opt-runner.md)
- signature: `class TrainResult:`
- members:
  - `changes` — [`L217`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L217) — documented in [domains-train_opt-runner](../../../concepts/domains-train_opt-runner.md)
  - `depth` — [`L219`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L219)
  - `description` — [`L218`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L218) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `iteration` — [`L211`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L211) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `num_params_m` — [`L215`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L215)
  - `peak_vram_mb` — [`L213`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L213)
  - `status` — [`L216`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L216) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `training_seconds` — [`L214`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L214)
  - `val_bpb` — [`L212`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L212) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`run_group_d`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`run`](outer.md#TrainOuterLoop.run), [`_analyze`](outer.md#TrainOuterLoop._analyze), [`run_group_a`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_a), [`cmd_inner`](cli.md#cmd_inner), [`add`](runner.md#TrainTrace.add), [`results`](runner.md#TrainTrace.results), [`summary`](runner.md#TrainTrace.summary), [`_build_report`](outer.md#TrainOuterLoop._build_report)  (8 test-only)

### `TrainRunner`
- def: [`domains/train_opt/runner.py:580`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L580)
- doc: Runs the inner loop: propose → modify train.py → train → evaluate → keep/discard.
- signature: `class TrainRunner:`
- members:
  - `_apply_changes(self, code: str, changes: dict)` — [`L1758`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1758) — Replace hyperparameter values in train.py code.
  - `_extract_changes_from_file(self, train_path: Path)` — [`L1945`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1945) — Extract the hyperparameter changes applied to a modified train.py file.
  - `_extract_hyperparams(self, code: str)` — [`L1818`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1818) — Parse current hyperparameter values from train.py code.
  - `_inject_time_budget(self, code: str, override_budget: int | None = None)` — [`L1771`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1771) — Override TIME_BUDGET if search_config specifies a non-default value.
  - `_parse_results(self, stdout: str)` — [`L1964`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1964) — Parse val_bpb and other metrics from training output.
  - `_propose(self, current_config: dict, iteration: int)` — [`L1366`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1366) — Ask LLM to propose hyperparameter changes. — documented in [core-llm_client](../../../concepts/core-llm_client.md)
  - `_run_training(self, train_path: Path, iter_dir: Path, quick_test: bool = False)` — [`L1831`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1831) — Execute train.py and parse results. Returns None on crash. — documented in [domains-train_opt-runner](../../../concepts/domains-train_opt-runner.md)
  - `run_baseline(self)` — [`L1305`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L1305) — Run the unmodified train.py to establish baseline. — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `run_iteration(self, iteration: int)` — [`L766`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L766) — Run one inner loop iteration. — documented in [domains-train_opt-mechanisms-register_adaptation](../../../concepts/domains-train_opt-mechanisms-register_adaptation.md)
  - `QUICK_TEST_BUDGET` — [`L586`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L586)
  - `QUICK_TEST_LOSS_THRESHOLD` — [`L587`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L587)
  - `adaptive_optics` — [`L704`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L704)
  - `artifacts_dir` — [`L604`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L604)
  - `back_translation` — [`L716`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L716)
  - `client` — [`L602`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L602)
  - `compost_heap` — [`L683`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L683)
  - `context_stratigraphy` — [`L673`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L673)
  - `crash_memory` — [`L618`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L618)
  - `current_code` — [`L612`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L612)
  - `domestication` — [`L725`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L725)
  - `elite_pool` — [`L628`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L628)
  - `epistasis_map` — [`L643`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L643)
  - `excavation_grid` — [`L678`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L678)
  - `fossil_record` — [`L668`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L668)
  - `grn` — [`L648`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L648)
  - `knockout_screen` — [`L653`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L653)
  - `momentum` — [`L623`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L623)
  - `original_code` — [`L611`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L611)
  - `parallax_estimator` — [`L713`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L713)
  - `perennial_classifier` — [`L698`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L698)
  - `plateau_detector` — [`L638`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L638)
  - `post_editing` — [`L728`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L728)
  - `register_adaptation` — [`L722`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L722)
  - `search_config` — [`L603`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L603)
  - `seasonal_cycling` — [`L693`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L693)
  - `semantic_equivalence` — [`L719`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L719)
  - `simple_mode` — [`L605`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L605)
  - `soil_health` — [`L688`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L688)
  - `spectral_decomposition` — [`L710`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L710)
  - `step_calibrator` — [`L633`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L633)
  - `stratigraphy` — [`L663`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L663)
  - `survey_tiling` — [`L701`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L701)
  - `target_of_opportunity` — [`L707`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L707)
  - `trace` — [`L613`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L613) — documented in [domains-train_opt-runner](../../../concepts/domains-train_opt-runner.md)
  - `train_py` — [`L600`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L600)
  - `transgenic` — [`L658`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L658)
  - `work_dir` — [`L601`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L601)
- protocol/private: `__init__`[`L591`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L591), `_best_code`[`L760`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L760), `_crossover_frequency`[`L736`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L736), `_exploration_frequency`[`L742`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L742), `_iters_since_improvement`[`L761`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L761), `_knockout_frequency`[`L731`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L731), `_max_acceptable_regression`[`L747`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L747), `_proposal_count`[`L737`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L737), `_sa_cooling_rate`[`L753`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L753), `_sa_initial_temp`[`L752`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L752), `_sa_iteration_count`[`L755`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L755), `_sa_temp`[`L754`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L754), `_stagnation_threshold`[`L762`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L762)
- uses (calls/refs, reference-scoped): [`active_params`](config.md#SearchConfig.active_params), [`parse_json_response`](../../core/llm_client.md#parse_json_response), [`call`](../../core/llm_client.md#LLMClient.call), [`SearchConfig`](config.md#SearchConfig), [`frozen_params`](config.md#SearchConfig.frozen_params), [`strategy`](config.md#SearchConfig.strategy), [`LLMClient`](../../core/llm_client.md#LLMClient), [`time_budget`](config.md#SearchConfig.time_budget), [`HYPERPARAM_NAMES`](config.md#HYPERPARAM_NAMES), [`guidance`](config.md#SearchConfig.guidance), [`logger`](runner.md#logger), [`add`](runner.md#TrainTrace.add), [`val_bpb`](runner.md#TrainResult.val_bpb), [`status`](runner.md#TrainResult.status), [`best_bpb`](runner.md#TrainTrace.best_bpb), [`summary`](runner.md#TrainTrace.summary), [`get_season_text`](mechanisms/seasonal_cycling.md#SeasonalCycling.get_season_text), [`record`](mechanisms/crash_memory.md#CrashMemory.record), [`_pool`](mechanisms/elite_pool.md#ElitePool._pool), [`advance`](mechanisms/seasonal_cycling.md#SeasonalCycling.advance), [`description`](runner.md#TrainResult.description), [`check_surprise`](mechanisms/target_of_opportunity.md#TargetOfOpportunity.check_surprise), [`get_domestication_text`](mechanisms/domestication.md#Domestication.get_domestication_text), [`record`](mechanisms/domestication.md#Domestication.record), [`record`](mechanisms/register_adaptation.md#RegisterAdaptation.record), [`iteration`](runner.md#TrainResult.iteration), [`check_plateau`](mechanisms/plateau_detector.md#PlateauDetector.check_plateau), [`get_register_text`](mechanisms/register_adaptation.md#RegisterAdaptation.get_register_text), [`get_seeing_text`](mechanisms/adaptive_optics.md#AdaptiveOptics.get_seeing_text), [`get_stratigraphy_text`](mechanisms/stratigraphic_record.md#StratigraphicRecord.get_stratigraphy_text), [`get_warning_text`](mechanisms/crash_memory.md#CrashMemory.get_warning_text), [`post_edit`](mechanisms/post_editing.md#PostEditing.post_edit), [`TrainResult`](runner.md#TrainResult), [`TrainTrace`](runner.md#TrainTrace), [`record`](mechanisms/excavation_grid.md#ExcavationGrid.record), [`build_rules`](mechanisms/gene_regulatory_network.md#GeneRegulatoryNetwork.build_rules), [`changes`](runner.md#TrainResult.changes), [`get_calibration_text`](mechanisms/back_translation.md#BackTranslation.get_calibration_text), [`get_compost_text`](mechanisms/compost_heap.md#CompostHeap.get_compost_text), [`get_epistasis_text`](mechanisms/epistasis_map.md#EpistasisMap.get_epistasis_text)  (+86 more)
- used by: [`run_group_d`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`run_group_c`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`run`](outer.md#TrainOuterLoop.run), [`_analyze`](outer.md#TrainOuterLoop._analyze), [`run_group_a`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_a), [`cmd_inner`](cli.md#cmd_inner), [`run_group_b`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_b), [`_build_report`](outer.md#TrainOuterLoop._build_report), [`cmd_bilevel`](cli.md#cmd_bilevel), [`_v`](../../experiments/ablations/paper_ablation/run_ablation.md#_v), [`_apply_analysis`](outer.md#TrainOuterLoop._apply_analysis), [`_v`](cli.md#_v), [`artifacts_dir`](outer.md#TrainOuterLoop.artifacts_dir), [`__init__`](outer.md#TrainOuterLoop.__init__)

### `TrainTrace`
- def: [`domains/train_opt/runner.py:226`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L226)
- signature: `class TrainTrace:`
- members:
  - `add(self, result: TrainResult)` — [`L233`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L233) — documented in [domains-train_opt-runner](../../../concepts/domains-train_opt-runner.md)
  - `summary(self, last_n: int = 10)` — [`L241`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L241) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `best_bpb` — [`L228`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L228) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `best_iteration` — [`L229`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L229) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `results` — [`L227`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L227) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
- uses (calls/refs, reference-scoped): [`val_bpb`](runner.md#TrainResult.val_bpb), [`status`](runner.md#TrainResult.status), [`description`](runner.md#TrainResult.description), [`iteration`](runner.md#TrainResult.iteration), [`TrainResult`](runner.md#TrainResult)
- used by: [`run_iteration`](runner.md#TrainRunner.run_iteration), [`_propose`](runner.md#TrainRunner._propose), [`run_group_d`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_d), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`run_group_c`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`run`](outer.md#TrainOuterLoop.run), [`_analyze`](outer.md#TrainOuterLoop._analyze), [`run_group_a`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_a), [`cmd_inner`](cli.md#cmd_inner), [`trace`](runner.md#TrainRunner.trace), [`_build_report`](outer.md#TrainOuterLoop._build_report)  (10 test-only)

## Functions
- `_is_infrastructure_error(stderr: str)` — [`L554`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L554) — Check if a crash was caused by infrastructure (not training).

## Module values
- `INFRA_ERROR_PATTERNS` — [`L540`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L540)
- `MULTI_CANDIDATE_PROMPT` — [`L326`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L326)
- `PICK_CANDIDATE_PROMPT` — [`L496`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L496)
- `PROPOSE_PROMPT` — [`L268`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L268)
- `PROPOSE_SYSTEM` — [`L261`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L261)
- `logger` — [`L198`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/runner.py#L198)

