---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/evaluator.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/evaluator.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.evaluator`/
symbols:
  EvaluatorService.evaluate: EvaluatorService#evaluate().
  EvaluatorService._build_internal_error_result: EvaluatorService#_build_internal_error_result().
  EvaluationResult: EvaluationResult#
  EvaluatorService.evaluate_batch: EvaluatorService#evaluate_batch().
  EvaluatorService.__aenter__: EvaluatorService#__aenter__().
  EvaluatorService.get_stats: EvaluatorService#get_stats().
  EvaluationResult.request_id: EvaluationResult#request_id.
  EvaluationResult.output_dir: EvaluationResult#output_dir.
  EvaluationResult.reward: EvaluationResult#reward.
  EvaluationResult.step_index: EvaluationResult#step_index.
  EvaluationResult.task_id: EvaluationResult#task_id.
  EvaluationResult.success: EvaluationResult#success().
  EvaluatorService._gpu_client: EvaluatorService#_gpu_client.
  EvaluatorService._cpu_client: EvaluatorService#_cpu_client.
  EvaluationResult.score: EvaluationResult#score.
  EvaluationResult.run_time: EvaluationResult#run_time.
  EvaluationResult.submit_medal: EvaluationResult#submit_medal.
  EvaluationRequest.metadata: EvaluationRequest#metadata.
  EvaluationRequest.output_dir: EvaluationRequest#output_dir.
  EvaluationResult.status_code: EvaluationResult#status_code.
  EvaluationResult.status: EvaluationResult#status.
  EvaluationResult.clear_run_log: EvaluationResult#clear_run_log.
  EvaluatorService: EvaluatorService#
  EvaluatorService._resource_type_override: EvaluatorService#_resource_type_override.
  EvaluationRequest: EvaluationRequest#
  EvaluationRequest.step_index: EvaluationRequest#step_index.
  EvaluationResult.task_name: EvaluationResult#task_name.
  EvaluationResult.job_id: EvaluationResult#job_id.
  EvaluationResult.queue_time: EvaluationResult#queue_time.
  EvaluationResult.submit_grade: EvaluationResult#submit_grade.
  EvaluatorService._status_counts: EvaluatorService#_status_counts.
  EvaluatorService.__aexit__: EvaluatorService#__aexit__().
  EvaluationRequest.request_id: EvaluationRequest#request_id.
  EvaluationRequest.task_id: EvaluationRequest#task_id.
  EvaluationRequest.task_name: EvaluationRequest#task_name.
  EvaluationRequest.code: EvaluationRequest#code.
  EvaluationRequest.data_dir: EvaluationRequest#data_dir.
  EvaluationResult.raw_run_log: EvaluationResult#raw_run_log.
  EvaluationResult.feedback: EvaluationResult#feedback.
  EvaluatorService._successful_evaluations: EvaluatorService#_successful_evaluations.
  logger: logger.
  EvaluationRequest.generation_prompt_tokens: EvaluationRequest#generation_prompt_tokens.
  EvaluationRequest.generation_completion_tokens: EvaluationRequest#generation_completion_tokens.
  EvaluationRequest.generation_total_tokens: EvaluationRequest#generation_total_tokens.
  EvaluationResult.code: EvaluationResult#code.
  EvaluationResult.generation_prompt_tokens: EvaluationResult#generation_prompt_tokens.
  EvaluationResult.generation_completion_tokens: EvaluationResult#generation_completion_tokens.
  EvaluationResult.generation_total_tokens: EvaluationResult#generation_total_tokens.
  EvaluatorService._total_evaluations: EvaluatorService#_total_evaluations.
  EvaluatorService._failed_evaluations: EvaluatorService#_failed_evaluations.
  EvaluatorService._total_score: EvaluatorService#_total_score.
  EvaluationRequest.use_score2reward: EvaluationRequest#use_score2reward.
  EvaluationResult.metadata: EvaluationResult#metadata.
  EvaluationResult.data_dir: EvaluationResult#data_dir.
  EvaluationResult.error: EvaluationResult#error.
  EvaluatorService._base_url: EvaluatorService#_base_url.
  EvaluatorService._cpu_base_url: EvaluatorService#_cpu_base_url.
  EvaluationResult.timestamp: EvaluationResult#timestamp.
  EvaluatorService._concurrency: EvaluatorService#_concurrency.
  EvaluatorService._semaphore: EvaluatorService#_semaphore.
  EvaluatorService._job_timeout: EvaluatorService#_job_timeout.
  EvaluatorService._wait_timeout: EvaluatorService#_wait_timeout.
  EvaluatorService._poll_interval: EvaluatorService#_poll_interval.
  EvaluatorService.__init__: EvaluatorService#__init__().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/evaluator.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py)

## Classes
### `EvaluationRequest`
- def: [`OpenMLE-ERL/SFT/tts_search/services/evaluator.py:34`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L34) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- doc: Request for code evaluation.
- signature: `class EvaluationRequest:`
- members:
  - `code` — [`L40`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L40) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `data_dir` — [`L41`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L41) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `generation_completion_tokens` — [`L47`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L47)
  - `generation_prompt_tokens` — [`L46`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L46)
  - `generation_total_tokens` — [`L48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L48)
  - `metadata` — [`L42`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L42) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `output_dir` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L44) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `request_id` — [`L37`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L37)
  - `step_index` — [`L43`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L43) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `task_id` — [`L38`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L38)
  - `task_name` — [`L39`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L39)
  - `use_score2reward` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L45)
- used by: [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`evaluate`](evaluator.md#EvaluatorService.evaluate), [`_build_internal_error_result`](evaluator.md#EvaluatorService._build_internal_error_result), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`evaluate_batch`](evaluator.md#EvaluatorService.evaluate_batch)

### `EvaluationResult`
- def: [`OpenMLE-ERL/SFT/tts_search/services/evaluator.py:52`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L52) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- doc: Result from code evaluation.
- signature: `class EvaluationResult:`
- members:
  - `success(self)` — [`L82`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L82)
  - `clear_run_log` — [`L66`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L66) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `code` — [`L73`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L73)
  - `data_dir` — [`L72`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L72)
  - `error` — [`L78`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L78)
  - `feedback` — [`L67`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L67) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `generation_completion_tokens` — [`L76`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L76)
  - `generation_prompt_tokens` — [`L75`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L75)
  - `generation_total_tokens` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L77)
  - `job_id` — [`L62`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L62) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `metadata` — [`L70`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L70)
  - `output_dir` — [`L74`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L74) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `queue_time` — [`L63`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L63) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `raw_run_log` — [`L65`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L65) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `request_id` — [`L55`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L55)
  - `reward` — [`L61`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L61) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `run_time` — [`L64`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L64) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `score` — [`L60`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L60) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `status` — [`L59`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L59) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `status_code` — [`L58`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L58) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `step_index` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L71)
  - `submit_grade` — [`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L68) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `submit_medal` — [`L69`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L69) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `task_id` — [`L56`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L56)
  - `task_name` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L57)
  - `timestamp` — [`L79`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L79)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`_create_task_result`](scheduler.md#Scheduler._create_task_result), [`_on_eval_result`](scheduler.md#Scheduler._on_eval_result), [`evaluate`](evaluator.md#EvaluatorService.evaluate), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_build_tree_program_from_eval`](scheduler.md#Scheduler._build_tree_program_from_eval), [`_build_internal_error_result`](evaluator.md#EvaluatorService._build_internal_error_result), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`_run_eval_loop`](scheduler.md#Scheduler._run_eval_loop), [`_attach_slime_message_token_count`](scheduler.md#Scheduler._attach_slime_message_token_count), [`_eval_record_search_metadata`](scheduler.md#Scheduler._eval_record_search_metadata), [`evaluate_batch`](evaluator.md#EvaluatorService.evaluate_batch), [`_decision_for_eval`](scheduler.md#Scheduler._decision_for_eval), [`_eval_record_metadata_hook`](scheduler.md#Scheduler._eval_record_metadata_hook), [`_eval_result_hook`](scheduler.md#Scheduler._eval_result_hook), [`_eval_results`](scheduler.md#Scheduler._eval_results)

### `EvaluatorService`
- def: [`OpenMLE-ERL/SFT/tts_search/services/evaluator.py:86`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L86)
- doc: Service for sandbox code evaluation.
- signature: `class EvaluatorService:`
- members:
  - `__aenter__(self)` — [`L181`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L181) — Create HTTP clients on context entry.
  - `__aexit__(self, exc_type, exc_val, exc_tb)` — [`L212`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L212) — Close HTTP clients on context exit.
  - `__init__(self, base_url: str, concurrency: int = 32, job_timeout: int = 3600, wait_timeout: int = 86400, poll_interval: int = 5, cpu_base_url: str | None = None, resource_type_override: str | None = None)` — [`L97`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L97) — Initialize the evaluator service.
  - `_build_internal_error_result(self, request: EvaluationRequest, exc: Exception)` — [`L143`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L143) — Convert unexpected evaluator exceptions into a normal failed result. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `evaluate(self, request: EvaluationRequest)` — [`L224`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L224) — Evaluate code in sandbox. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `evaluate_batch(self, requests: list[EvaluationRequest])` — [`L374`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L374) — Evaluate multiple code samples concurrently. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
  - `get_stats(self)` — [`L404`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L404) — Get service statistics.
- protocol/private: `_base_url`[`L119`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L119), `_concurrency`[`L121`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L121), `_cpu_base_url`[`L120`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L120), `_cpu_client`[`L134`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L134), `_failed_evaluations`[`L139`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L139), `_gpu_client`[`L133`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L133), `_job_timeout`[`L123`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L123), `_poll_interval`[`L125`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L125), `_resource_type_override`[`L126`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L126), `_semaphore`[`L122`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L122), `_status_counts`[`L141`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L141), `_successful_evaluations`[`L138`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L138), `_total_evaluations`[`L137`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L137), `_total_score`[`L140`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L140), `_wait_timeout`[`L124`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L124)
- uses (calls/refs, reference-scoped): [`EvaluationResult`](evaluator.md#EvaluationResult), [`score2reward`](../reward_func_utils.md#score2reward), [`get_sandbox_result`](../reward_func_utils.md#get_sandbox_result), [`output_dir`](evaluator.md#EvaluationResult.output_dir), [`request_id`](evaluator.md#EvaluationResult.request_id), [`reward`](evaluator.md#EvaluationResult.reward), [`step_index`](evaluator.md#EvaluationResult.step_index), [`task_id`](evaluator.md#EvaluationResult.task_id), [`build_submit_grade_and_medal`](../eval_utils.md#build_submit_grade_and_medal), [`run_time`](evaluator.md#EvaluationResult.run_time), [`score`](evaluator.md#EvaluationResult.score), [`submit_medal`](evaluator.md#EvaluationResult.submit_medal), [`format_sandbox_feedback`](../reward_func_utils.md#format_sandbox_feedback), [`clear_run_log`](evaluator.md#EvaluationResult.clear_run_log), [`get_clear_log`](../reward_func_utils.md#get_clear_log), [`metadata`](evaluator.md#EvaluationRequest.metadata), [`output_dir`](evaluator.md#EvaluationRequest.output_dir), [`status`](evaluator.md#EvaluationResult.status), [`status_code`](evaluator.md#EvaluationResult.status_code), [`EvaluationRequest`](evaluator.md#EvaluationRequest), [`job_id`](evaluator.md#EvaluationResult.job_id), [`load_leaderboard`](../eval_utils.md#load_leaderboard), [`normalize_sandbox_resource_type`](../reward_func_utils.md#normalize_sandbox_resource_type), [`queue_time`](evaluator.md#EvaluationResult.queue_time), [`step_index`](evaluator.md#EvaluationRequest.step_index), [`submit_grade`](evaluator.md#EvaluationResult.submit_grade), [`task_name`](evaluator.md#EvaluationResult.task_name), [`resolve_sandbox_resource_type`](../reward_func_utils.md#resolve_sandbox_resource_type), [`code`](evaluator.md#EvaluationRequest.code), [`data_dir`](evaluator.md#EvaluationRequest.data_dir), [`feedback`](evaluator.md#EvaluationResult.feedback), [`raw_run_log`](evaluator.md#EvaluationResult.raw_run_log), [`request_id`](evaluator.md#EvaluationRequest.request_id), [`task_id`](evaluator.md#EvaluationRequest.task_id), [`task_name`](evaluator.md#EvaluationRequest.task_name), [`code`](evaluator.md#EvaluationResult.code), [`generation_completion_tokens`](evaluator.md#EvaluationRequest.generation_completion_tokens), [`generation_completion_tokens`](evaluator.md#EvaluationResult.generation_completion_tokens), [`generation_prompt_tokens`](evaluator.md#EvaluationRequest.generation_prompt_tokens), [`generation_prompt_tokens`](evaluator.md#EvaluationResult.generation_prompt_tokens)  (+7 more)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`get_stats`](scheduler.md#Scheduler.get_stats), [`_evaluator`](scheduler.md#Scheduler._evaluator)

## Module values
- `logger` — [`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/evaluator.py#L30)

