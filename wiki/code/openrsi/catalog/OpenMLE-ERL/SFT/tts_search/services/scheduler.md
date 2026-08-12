---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/scheduler.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/scheduler.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.scheduler`/
symbols:
  Scheduler._run_looping_tasks: Scheduler#_run_looping_tasks().
  Scheduler._process_eval_batch: Scheduler#_process_eval_batch().
  Scheduler._create_task_result: Scheduler#_create_task_result().
  Scheduler._on_eval_result: Scheduler#_on_eval_result().
  Scheduler.run_evaluation_only: Scheduler#run_evaluation_only().
  Scheduler._gen_worker: Scheduler#_gen_worker().
  Scheduler._build_tree_program_from_eval: Scheduler#_build_tree_program_from_eval().
  Scheduler._on_gen_result: Scheduler#_on_gen_result().
  Scheduler._write_tree_search_state: Scheduler#_write_tree_search_state().
  Scheduler.get_progress: Scheduler#get_progress().
  Scheduler._config: Scheduler#_config.
  Scheduler._create_requests: Scheduler#_create_requests().
  _HAS_MATPLOTLIB: _HAS_MATPLOTLIB.
  rebuild_task_states_from_results: rebuild_task_states_from_results().
  Scheduler._search_algorithm: Scheduler#_search_algorithm.
  Scheduler._preload_tree_database_from_checkpoint: Scheduler#_preload_tree_database_from_checkpoint().
  Scheduler._eval_progress: Scheduler#_eval_progress.
  Scheduler._gen_progress: Scheduler#_gen_progress.
  Scheduler._run_eval_loop: Scheduler#_run_eval_loop().
  build_task_states_from_progress: build_task_states_from_progress().
  Scheduler._write_progress_snapshot_and_chart: Scheduler#_write_progress_snapshot_and_chart().
  Scheduler._eval_record_search_metadata: Scheduler#_eval_record_search_metadata().
  Scheduler._attach_slime_message_token_count: Scheduler#_attach_slime_message_token_count().
  logger: logger.
  Scheduler.get_stats: Scheduler#get_stats().
  Scheduler._decision_for_eval: Scheduler#_decision_for_eval().
  Scheduler._update_loop_progress_totals: Scheduler#_update_loop_progress_totals().
  Scheduler._progress_lock: Scheduler#_progress_lock.
  Scheduler.run_tasks: Scheduler#run_tasks().
  Scheduler._tree_search_enabled: Scheduler#_tree_search_enabled().
  SchedulerConfig: SchedulerConfig#
  TaskLoopState.target_count: TaskLoopState#target_count.
  TaskLoopState.done: TaskLoopState#done.
  TaskLoopState: TaskLoopState#
  Scheduler._database: Scheduler#_database.
  Scheduler._eval_queue: Scheduler#_eval_queue.
  Scheduler._refresh_completion_locked: Scheduler#_refresh_completion_locked().
  GenerationProgress.pending: GenerationProgress#pending().
  TaskLoopState.accepted_count: TaskLoopState#accepted_count.
  TaskLoopState.completed_count: TaskLoopState#completed_count.
  TaskLoopState.generated_count: TaskLoopState#generated_count.
  _eval_result_has_medal: _eval_result_has_medal().
  Scheduler._build_sft_assistant_content: Scheduler#_build_sft_assistant_content().
  Scheduler._drain_eval_queue: Scheduler#_drain_eval_queue().
  Scheduler._evaluator: Scheduler#_evaluator.
  Scheduler._task_states: Scheduler#_task_states.
  GenerationProgress.success: GenerationProgress#success.
  Scheduler._completed_tasks: Scheduler#_completed_tasks.
  Scheduler._generator: Scheduler#_generator.
  SchedulerConfig.enable_sandbox_eval: SchedulerConfig#enable_sandbox_eval.
  EvaluationProgress.success: EvaluationProgress#success.
  Scheduler._update_progress_trend_chart: Scheduler#_update_progress_trend_chart().
  GenerationProgress.failed: GenerationProgress#failed.
  EvaluationProgress.failed: EvaluationProgress#failed.
  TaskLoopState.next_step_index: TaskLoopState#next_step_index.
  Scheduler._start_time: Scheduler#_start_time.
  Scheduler._gen_results: Scheduler#_gen_results.
  SchedulerConfig.sandbox_concurrency: SchedulerConfig#sandbox_concurrency.
  TaskLoopState.task_id: TaskLoopState#task_id.
  TaskLoopState.task_name: TaskLoopState#task_name.
  _loop_target_met: _loop_target_met().
  load_checkpoint: load_checkpoint().
  Scheduler._eval_result_hook: Scheduler#_eval_result_hook.
  Scheduler._eval_record_metadata_hook: Scheduler#_eval_record_metadata_hook.
  Scheduler._eval_writer: Scheduler#_eval_writer.
  GenerationProgress.total: GenerationProgress#total.
  EvaluationProgress.pending_in_queue: EvaluationProgress#pending_in_queue.
  TaskLoopState.medal_count: TaskLoopState#medal_count.
  TaskLoopState.accepted_target: TaskLoopState#accepted_target.
  Scheduler._total_tasks: Scheduler#_total_tasks.
  Scheduler._end_time: Scheduler#_end_time.
  Scheduler._gen_writer: Scheduler#_gen_writer.
  Scheduler._enqueue_requests: Scheduler#_enqueue_requests().
  SchedulerConfig.task_subdir: SchedulerConfig#task_subdir.
  GenerationProgress.in_progress: GenerationProgress#in_progress.
  TaskResult: TaskResult#
  TaskLoopState.success_count: TaskLoopState#success_count.
  TaskLoopState.pending_gen: TaskLoopState#pending_gen.
  safe_task_output_name: safe_task_output_name().
  Scheduler.__init__: Scheduler#__init__().
  Scheduler._collect_completed_eval_tasks: Scheduler#_collect_completed_eval_tasks().
  SchedulerConfig.max_steps: SchedulerConfig#max_steps.
  SchedulerConfig.tree_search_algorithm: SchedulerConfig#tree_search_algorithm.
  GenerationProgress.start_time: GenerationProgress#start_time.
  EvaluationProgress.total: EvaluationProgress#total.
  EvaluationProgress.in_progress: EvaluationProgress#in_progress.
  EvaluationProgress.active_sandbox_slots: EvaluationProgress#active_sandbox_slots.
  EvaluationProgress.start_time: EvaluationProgress#start_time.
  TaskLoopState.max_target: TaskLoopState#max_target.
  load_progress_snapshot: load_progress_snapshot().
  Scheduler._step_code_path: Scheduler#_step_code_path().
  TaskResult.samples: TaskResult#samples.
  TaskResult.best_program: TaskResult#best_program.
  Scheduler._eval_results: Scheduler#_eval_results.
  Scheduler._progress_history_loop: Scheduler#_progress_history_loop().
  Scheduler._build_accepted_targets: Scheduler#_build_accepted_targets().
  Scheduler._submit_pending_requests: Scheduler#_submit_pending_requests().
  SchedulerConfig.llm_concurrency: SchedulerConfig#llm_concurrency.
  SchedulerConfig.sandbox_base_url: SchedulerConfig#sandbox_base_url.
  SchedulerConfig.sandbox_cpu_base_url: SchedulerConfig#sandbox_cpu_base_url.
  SchedulerConfig.sandbox_resource_type_override: SchedulerConfig#sandbox_resource_type_override.
  SchedulerConfig.job_timeout: SchedulerConfig#job_timeout.
  SchedulerConfig.wait_timeout: SchedulerConfig#wait_timeout.
  SchedulerConfig.poll_interval: SchedulerConfig#poll_interval.
  SchedulerConfig.skip_eval_for_done_tasks: SchedulerConfig#skip_eval_for_done_tasks.
  SchedulerConfig.loop_medal_target: SchedulerConfig#loop_medal_target.
  SchedulerConfig.loop_target_increment: SchedulerConfig#loop_target_increment.
  SchedulerConfig.loop_max_target: SchedulerConfig#loop_max_target.
  SchedulerConfig.resume_rebuild_task_states: SchedulerConfig#resume_rebuild_task_states.
  SchedulerConfig.rejection_target: SchedulerConfig#rejection_target.
  SchedulerConfig.rejection_apply_baseline_filters: SchedulerConfig#rejection_apply_baseline_filters.
  SchedulerConfig.rejection_baseline_token_limit: SchedulerConfig#rejection_baseline_token_limit.
  SchedulerConfig.rejection_baseline_tokenizer_model: SchedulerConfig#rejection_baseline_tokenizer_model.
  SchedulerConfig.rejection_baseline_relative_gap_limit: SchedulerConfig#rejection_baseline_relative_gap_limit.
  SchedulerConfig.rejection_mixed_leaderboard_target: SchedulerConfig#rejection_mixed_leaderboard_target.
  SchedulerConfig.rejection_mixed_no_leaderboard_target: SchedulerConfig#rejection_mixed_no_leaderboard_target.
  SchedulerConfig.tree_search_enabled: SchedulerConfig#tree_search_enabled.
  SchedulerConfig.tree_search_max_pending_per_task: SchedulerConfig#tree_search_max_pending_per_task.
  SchedulerConfig.tree_search_db_path: SchedulerConfig#tree_search_db_path.
  GenerationProgress: GenerationProgress#
  GenerationProgress.end_time: GenerationProgress#end_time.
  EvaluationProgress: EvaluationProgress#
  EvaluationProgress.end_time: EvaluationProgress#end_time.
  TaskResult.task_name: TaskResult#task_name.
  TaskResult.status_counts: TaskResult#status_counts.
  progress_snapshot_has_medal_counts: progress_snapshot_has_medal_counts().
  Scheduler: Scheduler#
  Scheduler._output_dir: Scheduler#_output_dir.
  Scheduler._baseline_tokenizer: Scheduler#_baseline_tokenizer.
  Scheduler._task_search_paths: Scheduler#_task_search_paths().
  SchedulerConfig.llm_max_retries_per_step: SchedulerConfig#llm_max_retries_per_step.
  SchedulerConfig.use_score2reward: SchedulerConfig#use_score2reward.
  SchedulerConfig.eval_queue_maxsize: SchedulerConfig#eval_queue_maxsize.
  SchedulerConfig.loop_enabled: SchedulerConfig#loop_enabled.
  SchedulerConfig.loop_success_target: SchedulerConfig#loop_success_target.
  SchedulerConfig.loop_success_metric: SchedulerConfig#loop_success_metric.
  SchedulerConfig.rejection_policy: SchedulerConfig#rejection_policy.
  SchedulerConfig.rejection_score_threshold: SchedulerConfig#rejection_score_threshold.
  SchedulerConfig.rejection_reward_threshold: SchedulerConfig#rejection_reward_threshold.
  SchedulerConfig.rejection_reference_scores_path: SchedulerConfig#rejection_reference_scores_path.
  SchedulerConfig.rejection_accepted_medals: SchedulerConfig#rejection_accepted_medals.
  SchedulerConfig.tree_search_db_max_per_task: SchedulerConfig#tree_search_db_max_per_task.
  SchedulerConfig.greedy_num_drafts: SchedulerConfig#greedy_num_drafts.
  SchedulerConfig.greedy_debug_prob: SchedulerConfig#greedy_debug_prob.
  SchedulerConfig.greedy_draft_prob: SchedulerConfig#greedy_draft_prob.
  SchedulerConfig.gen_retry_max: SchedulerConfig#gen_retry_max.
  TaskResult.task_id: TaskResult#task_id.
  TaskResult.best_score: TaskResult#best_score.
  TaskResult.best_reward: TaskResult#best_reward.
  TaskResult.total_cost: TaskResult#total_cost.
  TaskResult.total_tokens: TaskResult#total_tokens.
  TaskResult.num_samples: TaskResult#num_samples.
  TaskResult.medal_count: TaskResult#medal_count.
  TaskResult.medal_counts: TaskResult#medal_counts.
  TaskResult.test_time: TaskResult#test_time.
  Scheduler._results_lock: Scheduler#_results_lock.
  Scheduler._relative_to_task_dir: Scheduler#_relative_to_task_dir().
  Scheduler._code_sha256: Scheduler#_code_sha256().
  SchedulerConfig.n_samples_per_task: SchedulerConfig#n_samples_per_task.
  SchedulerConfig.batch_size: SchedulerConfig#batch_size.
  SchedulerConfig.task_concurrency: SchedulerConfig#task_concurrency.
  SchedulerConfig.eval_batch_timeout: SchedulerConfig#eval_batch_timeout.
  SchedulerConfig.progress_history_interval_seconds: SchedulerConfig#progress_history_interval_seconds.
  TaskResult.val_time: TaskResult#val_time.
  Scheduler.null_evaluator_ctx: Scheduler#null_evaluator_ctx().
  SchedulerConfig.progress_trend_fig_width_min: SchedulerConfig#progress_trend_fig_width_min.
  SchedulerConfig.progress_trend_fig_width_max: SchedulerConfig#progress_trend_fig_width_max.
  SchedulerConfig.progress_trend_inches_per_hour: SchedulerConfig#progress_trend_inches_per_hour.
  TaskResult.timestamp: TaskResult#timestamp.
  Scheduler._router: Scheduler#_router.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py)

## Classes
### `EvaluationProgress`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:171`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L171)
- doc: Progress tracking for evaluation pipeline.
- signature: `class EvaluationProgress:`
- members:
  - `active_sandbox_slots` — [`L179`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L179)
  - `end_time` — [`L181`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L181)
  - `failed` — [`L178`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L178)
  - `in_progress` — [`L176`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L176)
  - `pending_in_queue` — [`L177`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L177)
  - `start_time` — [`L180`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L180)
  - `success` — [`L175`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L175)
  - `total` — [`L174`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L174)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`get_progress`](scheduler.md#Scheduler.get_progress), [`_eval_progress`](scheduler.md#Scheduler._eval_progress), [`_run_eval_loop`](scheduler.md#Scheduler._run_eval_loop), [`_write_progress_snapshot_and_chart`](scheduler.md#Scheduler._write_progress_snapshot_and_chart), [`_update_loop_progress_totals`](scheduler.md#Scheduler._update_loop_progress_totals), [`_drain_eval_queue`](scheduler.md#Scheduler._drain_eval_queue)

### `GenerationProgress`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:155`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L155)
- doc: Progress tracking for generation pipeline.
- signature: `class GenerationProgress:`
- members:
  - `pending(self)` — [`L166`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L166)
  - `end_time` — [`L163`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L163)
  - `failed` — [`L161`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L161)
  - `in_progress` — [`L160`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L160)
  - `start_time` — [`L162`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L162)
  - `success` — [`L159`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L159)
  - `total` — [`L158`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L158)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`get_progress`](scheduler.md#Scheduler.get_progress), [`_gen_progress`](scheduler.md#Scheduler._gen_progress), [`_write_progress_snapshot_and_chart`](scheduler.md#Scheduler._write_progress_snapshot_and_chart), [`_update_loop_progress_totals`](scheduler.md#Scheduler._update_loop_progress_totals)

### `Scheduler`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:526`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L526)
- doc: Scheduler for coordinating generation and evaluation.
- signature: `class Scheduler:`
- members:
  - `__init__(self, router: Router, config: SchedulerConfig, database: ProgramDatabase | None = None, output_dir: Path | str | None = None, litellm_model_list: list[Any] | None = None)` — [`L537`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L537) — Initialize the scheduler.
  - `_create_task_result(self, task_id: str, task_name: str, generation_results: list[GenerationResult], evaluation_results: list[EvaluationResult], metadata: dict[str, Any])` — [`L2379`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2379) — Create TaskResult from generation and evaluation results. — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
  - `_process_eval_batch(self, gen_results: list[GenerationResult], output_dir: Path, store_results: bool = True)` — [`L2233`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2233) — Process a batch of generation results through evaluation. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `_run_eval_loop(self, output_dir: Path, store_results: bool = True)` — [`L2108`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2108) — Core evaluation loop using fire-and-forget pattern. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `_run_looping_tasks(self, tasks: list[dict[str, Any]], model_name: str, output_dir: Path, resume: bool = True)` — [`L873`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L873) — Run looping evaluation with per-task success/target tracking. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `_update_progress_trend_chart(self, output_dir: Path, history_path: Path)` — [`L1982`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1982) — Read progress_history.jsonl and save progress_trend.png (generation/evaluation/completed_tasks over time).
  - `_write_progress_snapshot_and_chart(self, output_dir: Path)` — [`L2077`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2077) — Take a snapshot of gen/eval/completed_tasks under lock, append to progress_history.jsonl, update trend chart.
  - `get_progress(self)` — [`L2538`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2538) — Get real-time progress information for both pipelines.
  - `get_stats(self)` — [`L2520`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2520) — Get scheduler statistics. — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `null_evaluator_ctx()` — [`L1095`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1095)
  - `run_evaluation_only(self, output_dir: Path, tasks: list[dict[str, Any]] | None = None)` — [`L631`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L631) — Run evaluation only on existing generation results. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `run_tasks(self, tasks: list[dict[str, Any]], model_name: str, output_dir: Path | None = None, resume: bool = True)` — [`L830`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L830) — Run pass@k evaluation for multiple tasks. — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
- protocol/private: `_attach_slime_message_token_count`[`L1785`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1785), `_baseline_tokenizer`[`L597`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L597), `_build_accepted_targets`[`L1726`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1726), `_build_sft_assistant_content`[`L1770`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1770), `_build_tree_program_from_eval`[`L1861`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1861), `_code_sha256`[`L1767`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1767), `_collect_completed_eval_tasks`[`L2159`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2159), `_completed_tasks`[`L582`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L582), `_config`[`L555`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L555), `_create_requests`[`L1200`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1200), `_database`[`L556`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L556), `_decision_for_eval`[`L1104`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1104), `_drain_eval_queue`[`L2132`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2132), `_end_time`[`L587`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L587), `_enqueue_requests`[`L1283`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1283), `_eval_progress`[`L577`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L577), `_eval_queue`[`L571`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L571), `_eval_record_metadata_hook`[`L596`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L596), `_eval_record_search_metadata`[`L1114`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1114), `_eval_result_hook`[`L593`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L593), `_eval_results`[`L591`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L591), `_eval_writer`[`L601`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L601), `_evaluator`[`L568`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L568), `_gen_progress`[`L576`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L576), `_gen_results`[`L590`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L590), `_gen_worker`[`L1523`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1523), `_gen_writer`[`L600`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L600), `_generator`[`L560`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L560), `_on_eval_result`[`L1352`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1352), `_on_gen_result`[`L1288`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1288), `_output_dir`[`L557`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L557), `_preload_tree_database_from_checkpoint`[`L1915`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1915), `_progress_history_loop`[`L1655`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1655), `_progress_lock`[`L578`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L578), `_refresh_completion_locked`[`L1194`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1194), `_relative_to_task_dir`[`L1752`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1752), `_results_lock`[`L592`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L592), `_router`[`L554`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L554), `_search_algorithm`[`L602`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L602), `_start_time`[`L586`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L586), `_step_code_path`[`L1762`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1762), `_submit_pending_requests`[`L2148`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L2148), `_task_search_paths`[`L1747`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1747), `_task_states`[`L583`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L583), `_total_tasks`[`L581`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L581), `_tree_search_enabled`[`L1744`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1744), `_update_loop_progress_totals`[`L1975`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1975), `_write_tree_search_state`[`L1810`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L1810)
- uses (calls/refs, reference-scoped): [`generate`](generator.md#GeneratorService.generate), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`rebuild_task_states_from_results`](scheduler.md#rebuild_task_states_from_results), [`add`](../program_database.md#ProgramDatabase.add), [`select`](../greedy.md#GreedySearch.select), [`build_rejection_policy`](rejection.md#build_rejection_policy), [`build_task_states_from_progress`](scheduler.md#build_task_states_from_progress), [`Program`](../program_database.md#Program), [`get_stats`](generator.md#GeneratorService.get_stats), [`EvaluationResult`](evaluator.md#EvaluationResult), [`evaluate_batch`](evaluator.md#EvaluatorService.evaluate_batch), [`logger`](scheduler.md#logger), [`GenerationResult`](generator.md#GenerationResult), [`advance_after_completion`](generation_loop.md#GenerationLoopController.advance_after_completion), [`request_id`](generator.md#GenerationResult.request_id), [`task_id`](generator.md#GenerationResult.task_id), [`model_name`](generator.md#GenerationRequest.model_name), [`step_index`](generator.md#GenerationRequest.step_index), [`step_index`](generator.md#GenerationResult.step_index), [`get_stats`](evaluator.md#EvaluatorService.get_stats), [`SchedulerConfig`](scheduler.md#SchedulerConfig), [`SearchEvent`](tree_search_state.md#SearchEvent), [`done`](scheduler.md#TaskLoopState.done), [`metadata`](../program_database.md#Program.metadata), [`output_dir`](evaluator.md#EvaluationResult.output_dir), [`request_id`](evaluator.md#EvaluationResult.request_id), [`target_count`](scheduler.md#TaskLoopState.target_count), [`task_id`](generator.md#GenerationRequest.task_id), [`SearchState`](tree_search_state.md#SearchState), [`TaskLoopState`](scheduler.md#TaskLoopState), [`reward`](evaluator.md#EvaluationResult.reward), [`success`](generator.md#GenerationResult.success), [`write`](result_persistence.md#StreamingJSONLWriter.write), [`atomic_write_search_state`](tree_search_state.md#atomic_write_search_state), [`accepted_count`](scheduler.md#TaskLoopState.accepted_count), [`append_search_event`](tree_search_state.md#append_search_event), [`code`](generator.md#GenerationResult.code), [`completed_count`](scheduler.md#TaskLoopState.completed_count), [`fitness`](../program_database.md#Program.fitness), [`generated_count`](scheduler.md#TaskLoopState.generated_count)  (+218 more)
- used by: [`run_pass_k_evaluation`](../evaluate_pass_k.md#run_pass_k_evaluation), [`monitor_progress`](../evaluate_pass_k.md#run_pass_k_evaluation.monitor_progress)

### `SchedulerConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:80`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L80)
- doc: Configuration for the scheduler.
- signature: `class SchedulerConfig:`
- members:
  - `batch_size` — [`L100`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L100)
  - `enable_sandbox_eval` — [`L102`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L102)
  - `eval_batch_timeout` — [`L107`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L107)
  - `eval_queue_maxsize` — [`L106`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L106)
  - `gen_retry_max` — [`L144`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L144)
  - `greedy_debug_prob` — [`L140`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L140)
  - `greedy_draft_prob` — [`L141`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L141)
  - `greedy_num_drafts` — [`L139`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L139)
  - `job_timeout` — [`L94`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L94)
  - `llm_concurrency` — [`L86`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L86)
  - `llm_max_retries_per_step` — [`L87`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L87)
  - `loop_enabled` — [`L113`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L113)
  - `loop_max_target` — [`L118`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L118)
  - `loop_medal_target` — [`L116`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L116)
  - `loop_success_metric` — [`L115`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L115)
  - `loop_success_target` — [`L114`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L114)
  - `loop_target_increment` — [`L117`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L117)
  - `max_steps` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L84)
  - `n_samples_per_task` — [`L85`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L85)
  - `poll_interval` — [`L96`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L96)
  - `progress_history_interval_seconds` — [`L147`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L147)
  - `progress_trend_fig_width_max` — [`L150`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L150)
  - `progress_trend_fig_width_min` — [`L149`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L149)
  - `progress_trend_inches_per_hour` — [`L151`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L151)
  - `rejection_accepted_medals` — [`L125`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L125)
  - `rejection_apply_baseline_filters` — [`L126`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L126)
  - `rejection_baseline_relative_gap_limit` — [`L129`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L129)
  - `rejection_baseline_token_limit` — [`L127`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L127)
  - `rejection_baseline_tokenizer_model` — [`L128`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L128)
  - `rejection_mixed_leaderboard_target` — [`L130`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L130)
  - `rejection_mixed_no_leaderboard_target` — [`L131`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L131)
  - `rejection_policy` — [`L120`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L120)
  - `rejection_reference_scores_path` — [`L124`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L124)
  - `rejection_reward_threshold` — [`L123`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L123)
  - `rejection_score_threshold` — [`L122`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L122)
  - `rejection_target` — [`L121`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L121)
  - `resume_rebuild_task_states` — [`L119`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L119)
  - `sandbox_base_url` — [`L90`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L90)
  - `sandbox_concurrency` — [`L93`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L93)
  - `sandbox_cpu_base_url` — [`L91`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L91)
  - `sandbox_resource_type_override` — [`L92`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L92)
  - `skip_eval_for_done_tasks` — [`L103`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L103)
  - `task_concurrency` — [`L101`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L101)
  - `task_subdir` — [`L110`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L110)
  - `tree_search_algorithm` — [`L135`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L135)
  - `tree_search_db_max_per_task` — [`L138`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L138)
  - `tree_search_db_path` — [`L137`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L137)
  - `tree_search_enabled` — [`L134`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L134)
  - `tree_search_max_pending_per_task` — [`L136`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L136)
  - `use_score2reward` — [`L97`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L97)
  - `wait_timeout` — [`L95`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L95)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`run_pass_k_evaluation`](../evaluate_pass_k.md#run_pass_k_evaluation), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`_create_task_result`](scheduler.md#Scheduler._create_task_result), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`_on_gen_result`](scheduler.md#Scheduler._on_gen_result), [`_write_tree_search_state`](scheduler.md#Scheduler._write_tree_search_state), [`get_progress`](scheduler.md#Scheduler.get_progress), [`_create_requests`](scheduler.md#Scheduler._create_requests), [`_search_algorithm`](scheduler.md#Scheduler._search_algorithm), [`_run_eval_loop`](scheduler.md#Scheduler._run_eval_loop), [`_attach_slime_message_token_count`](scheduler.md#Scheduler._attach_slime_message_token_count), [`run_tasks`](scheduler.md#Scheduler.run_tasks), [`_tree_search_enabled`](scheduler.md#Scheduler._tree_search_enabled), [`_eval_queue`](scheduler.md#Scheduler._eval_queue), [`_generator`](scheduler.md#Scheduler._generator), [`monitor_progress`](../evaluate_pass_k.md#run_pass_k_evaluation.monitor_progress), [`__init__`](scheduler.md#Scheduler.__init__)

### `TaskLoopState`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:206`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L206) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
- doc: Per-task state for looping evaluation.
- signature: `class TaskLoopState:`
- members:
  - `accepted_count` — [`L213`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L213)
  - `accepted_target` — [`L219`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L219)
  - `completed_count` — [`L214`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L214)
  - `done` — [`L221`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L221) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
  - `generated_count` — [`L215`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L215)
  - `max_target` — [`L218`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L218)
  - `medal_count` — [`L212`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L212)
  - `next_step_index` — [`L220`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L220)
  - `pending_gen` — [`L216`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L216)
  - `success_count` — [`L211`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L211)
  - `target_count` — [`L217`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L217) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
  - `task_id` — [`L209`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L209)
  - `task_name` — [`L210`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L210)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`run_pass_k_evaluation`](../evaluate_pass_k.md#run_pass_k_evaluation), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`_on_eval_result`](scheduler.md#Scheduler._on_eval_result), [`_on_gen_result`](scheduler.md#Scheduler._on_gen_result), [`_write_tree_search_state`](scheduler.md#Scheduler._write_tree_search_state), [`get_progress`](scheduler.md#Scheduler.get_progress), [`_create_requests`](scheduler.md#Scheduler._create_requests), [`rebuild_task_states_from_results`](scheduler.md#rebuild_task_states_from_results), [`_write_progress_snapshot_and_chart`](scheduler.md#Scheduler._write_progress_snapshot_and_chart), [`build_task_states_from_progress`](scheduler.md#build_task_states_from_progress), [`_update_loop_progress_totals`](scheduler.md#Scheduler._update_loop_progress_totals), [`_refresh_completion_locked`](scheduler.md#Scheduler._refresh_completion_locked), [`_task_states`](scheduler.md#Scheduler._task_states), [`_loop_target_met`](scheduler.md#_loop_target_met)

### `TaskResult`
- def: [`OpenMLE-ERL/SFT/tts_search/services/scheduler.py:185`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L185)
- doc: Result for a single task after pass@k evaluation.
- signature: `class TaskResult:`
- members:
  - `best_program` — [`L191`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L191) — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
  - `best_reward` — [`L193`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L193)
  - `best_score` — [`L192`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L192)
  - `medal_count` — [`L198`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L198)
  - `medal_counts` — [`L199`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L199)
  - `num_samples` — [`L196`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L196)
  - `samples` — [`L190`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L190) — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
  - `status_counts` — [`L197`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L197)
  - `task_id` — [`L188`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L188)
  - `task_name` — [`L189`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L189)
  - `test_time` — [`L201`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L201)
  - `timestamp` — [`L202`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L202)
  - `total_cost` — [`L194`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L194)
  - `total_tokens` — [`L195`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L195)
  - `val_time` — [`L200`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L200)
- uses (calls/refs, reference-scoped): [`Program`](../program_database.md#Program)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`run_pass_k_evaluation`](../evaluate_pass_k.md#run_pass_k_evaluation), [`_create_task_result`](scheduler.md#Scheduler._create_task_result), [`run_tasks`](scheduler.md#Scheduler.run_tasks)

## Functions
- `_eval_result_has_medal(data: dict[str, Any], metadata: dict[str, Any] | None = None)` — [`L329`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L329)
- `_loop_target_met(state: TaskLoopState, rejection_target: int)` — [`L354`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L354)
- `build_task_states_from_progress(progress_snapshot: dict[str, Any] | None, tasks: list[dict[str, Any]], loop_increment: int, loop_max_target: int | None, rejection_policy_name: str = "accept_scored")` — [`L368`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L368) — Build task states from progress.json snapshot if available. — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
- `load_checkpoint(output_dir: Path)` — [`L224`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L224) — Load checkpoint state from output directory.
- `load_progress_snapshot(output_dir: Path)` — [`L311`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L311) — Load progress.json if available for resume.
- `progress_snapshot_has_medal_counts(progress_snapshot: dict[str, Any] | None)` — [`L361`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L361)
- `rebuild_task_states_from_results(tasks: list[dict[str, Any]], gen_results_data: list[dict[str, Any]], eval_results_data: list[dict[str, Any]], loop_increment: int, loop_success_target: int, loop_success_metric: str = "success", loop_medal_target: int | None = None, loop_max_target: int | None = None, rejection_policy: RejectionPolicy | None = None, rejection_target: int | None = None, accepted_targets: Mapping[str, int] | None = None, count_successful_generation_as_completed: bool = False)` — [`L410`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L410) — Rebuild task states from gen/eval result records. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `safe_task_output_name(task_name: str, task_id: str | None)` — [`L322`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L322) — Return a task output directory name that is unique for duplicate task names.

## Module values
- `_HAS_MATPLOTLIB` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L36)
- `logger` — [`L76`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/scheduler.py#L76)

