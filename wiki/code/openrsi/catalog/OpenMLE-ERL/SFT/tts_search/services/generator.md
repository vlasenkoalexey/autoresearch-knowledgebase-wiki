---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/generator.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/generator.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.generator`/
symbols:
  GeneratorService.generate: GeneratorService#generate().
  logger: logger.
  GeneratorService.get_stats: GeneratorService#get_stats().
  GenerationResult: GenerationResult#
  GenerationResult.request_id: GenerationResult#request_id.
  GenerationResult.task_id: GenerationResult#task_id.
  GenerationRequest.model_name: GenerationRequest#model_name.
  GenerationRequest.step_index: GenerationRequest#step_index.
  GenerationResult.step_index: GenerationResult#step_index.
  GenerationRequest.task_id: GenerationRequest#task_id.
  GenerationResult.success: GenerationResult#success().
  GenerationRequest.task_name: GenerationRequest#task_name.
  GenerationResult.code: GenerationResult#code.
  GenerationRequest: GenerationRequest#
  GenerationRequest.messages: GenerationRequest#messages.
  GenerationResult.total_tokens: GenerationResult#total_tokens.
  GenerationResult.messages: GenerationResult#messages.
  GenerationResult.raw_text: GenerationResult#raw_text.
  GenerationResult.reasoning_content: GenerationResult#reasoning_content.
  GenerationResult.prompt_tokens: GenerationResult#prompt_tokens.
  GenerationResult.completion_tokens: GenerationResult#completion_tokens.
  GenerationResult.cost: GenerationResult#cost.
  GenerationResult.model_name: GenerationResult#model_name.
  GenerationResult.search_metadata: GenerationResult#search_metadata.
  GeneratorService.generate_batch: GeneratorService#generate_batch().
  handler: handler.
  GenerationRequest.output_dir: GenerationRequest#output_dir.
  GenerationResult.task_name: GenerationResult#task_name.
  GenerationResult.output_dir: GenerationResult#output_dir.
  GeneratorService._acompletion_stream_collect: GeneratorService#_acompletion_stream_collect().
  GeneratorService._get_model_litellm_params: GeneratorService#_get_model_litellm_params().
  GenerationResult.metadata: GenerationResult#metadata.
  GenerationResult.data_dir: GenerationResult#data_dir.
  GenerationRequest.request_id: GenerationRequest#request_id.
  GeneratorService._total_tokens: GeneratorService#_total_tokens.
  GeneratorService._total_prompt_tokens: GeneratorService#_total_prompt_tokens.
  GeneratorService._total_completion_tokens: GeneratorService#_total_completion_tokens.
  GeneratorService._get_streaming_config: GeneratorService#_get_streaming_config().
  GenerationRequest.data_dir: GenerationRequest#data_dir.
  GenerationRequest.metadata: GenerationRequest#metadata.
  GenerationRequest.search_metadata: GenerationRequest#search_metadata.
  GenerationResult.error: GenerationResult#error.
  GeneratorService: GeneratorService#
  GeneratorService._total_cost: GeneratorService#_total_cost.
  GeneratorService._total_prompt_cost: GeneratorService#_total_prompt_cost.
  GeneratorService._total_response_cost: GeneratorService#_total_response_cost.
  GeneratorService._request_queue: GeneratorService#_request_queue.
  GeneratorService._result_queue: GeneratorService#_result_queue.
  GeneratorService._router: GeneratorService#_router.
  GeneratorService._semaphore: GeneratorService#_semaphore.
  GeneratorService._max_retries: GeneratorService#_max_retries.
  GeneratorService._total_requests: GeneratorService#_total_requests.
  GeneratorService._successful_requests: GeneratorService#_successful_requests.
  GeneratorService._failed_requests: GeneratorService#_failed_requests.
  GeneratorService._to_plain_dict: GeneratorService#_to_plain_dict().
  GenerationResult.timestamp: GenerationResult#timestamp.
  GeneratorService._model_list: GeneratorService#_model_list.
  MidStreamFallbackError.__init__: MidStreamFallbackError#__init__().
  MidStreamFallbackError.llm_provider: MidStreamFallbackError#llm_provider.
  MidStreamFallbackError.model: MidStreamFallbackError#model.
  MidStreamFallbackError.response: MidStreamFallbackError#response.
  GeneratorService.__init__: GeneratorService#__init__().
  GeneratorService._running: GeneratorService#_running.
  GeneratorService._workers: GeneratorService#_workers.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/generator.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py)

## Classes
### `GenerationRequest`
- def: [`OpenMLE-ERL/SFT/tts_search/services/generator.py:62`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L62) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- doc: Request for code generation.
- signature: `class GenerationRequest:`
- members:
  - `data_dir` — [`L70`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L70) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `messages` — [`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L68) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `metadata` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L71)
  - `model_name` — [`L69`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L69) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `output_dir` — [`L73`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L73) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `request_id` — [`L65`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L65) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `search_metadata` — [`L74`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L74) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `step_index` — [`L72`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L72) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `task_id` — [`L66`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L66) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `task_name` — [`L67`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L67) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`generate`](generator.md#GeneratorService.generate), [`_create_requests`](scheduler.md#Scheduler._create_requests), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`generate_batch`](generator.md#GeneratorService.generate_batch), [`_request_queue`](generator.md#GeneratorService._request_queue)

### `GenerationResult`
- def: [`OpenMLE-ERL/SFT/tts_search/services/generator.py:78`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L78) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- doc: Result from code generation.
- signature: `class GenerationResult:`
- members:
  - `success(self)` — [`L102`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L102) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
  - `code` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L84) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `completion_tokens` — [`L88`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L88) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `cost` — [`L90`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L90) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `data_dir` — [`L95`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L95) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `error` — [`L98`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L98) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `messages` — [`L92`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L92)
  - `metadata` — [`L93`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L93)
  - `model_name` — [`L91`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L91)
  - `output_dir` — [`L96`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L96) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `prompt_tokens` — [`L87`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L87) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `raw_text` — [`L85`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L85) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `reasoning_content` — [`L86`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L86) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `request_id` — [`L81`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L81) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
  - `search_metadata` — [`L97`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L97) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `step_index` — [`L94`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L94)
  - `task_id` — [`L82`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L82)
  - `task_name` — [`L83`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L83)
  - `timestamp` — [`L99`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L99)
  - `total_tokens` — [`L89`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L89) — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`_create_task_result`](scheduler.md#Scheduler._create_task_result), [`_on_eval_result`](scheduler.md#Scheduler._on_eval_result), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`generate`](generator.md#GeneratorService.generate), [`_build_tree_program_from_eval`](scheduler.md#Scheduler._build_tree_program_from_eval), [`_on_gen_result`](scheduler.md#Scheduler._on_gen_result), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`_run_eval_loop`](scheduler.md#Scheduler._run_eval_loop), [`_attach_slime_message_token_count`](scheduler.md#Scheduler._attach_slime_message_token_count), [`_eval_record_search_metadata`](scheduler.md#Scheduler._eval_record_search_metadata), [`_eval_queue`](scheduler.md#Scheduler._eval_queue), [`_build_sft_assistant_content`](scheduler.md#Scheduler._build_sft_assistant_content), [`_gen_results`](scheduler.md#Scheduler._gen_results), [`generate_batch`](generator.md#GeneratorService.generate_batch), [`_result_queue`](generator.md#GeneratorService._result_queue)

### `GeneratorService`
- def: [`OpenMLE-ERL/SFT/tts_search/services/generator.py:106`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L106)
- doc: Service for code generation using LLM.
- signature: `class GeneratorService:`
- members:
  - `__init__(self, router: Router, concurrency: int = 64, max_retries: int = 10, model_list: list[Any] | None = None)` — [`L117`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L117) — Initialize the generator service.
  - `generate(self, request: GenerationRequest)` — [`L152`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L152) — Generate code for a single request. — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `generate_batch(self, requests: list[GenerationRequest])` — [`L667`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L667) — Generate code for multiple requests concurrently. — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
  - `get_stats(self)` — [`L682`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L682) — Get service statistics. — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- protocol/private: `_acompletion_stream_collect`[`L599`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L599), `_failed_requests`[`L144`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L144), `_get_model_litellm_params`[`L583`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L583), `_get_streaming_config`[`L591`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L591), `_max_retries`[`L134`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L134), `_model_list`[`L135`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L135), `_request_queue`[`L136`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L136), `_result_queue`[`L137`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L137), `_router`[`L132`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L132), `_running`[`L138`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L138), `_semaphore`[`L133`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L133), `_successful_requests`[`L143`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L143), `_to_plain_dict`[`L574`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L574), `_total_completion_tokens`[`L147`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L147), `_total_cost`[`L148`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L148), `_total_prompt_cost`[`L149`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L149), `_total_prompt_tokens`[`L146`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L146), `_total_requests`[`L142`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L142), `_total_response_cost`[`L150`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L150), `_total_tokens`[`L145`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L145), `_workers`[`L139`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L139)
- uses (calls/refs, reference-scoped): [`logger`](generator.md#logger), [`GenerationResult`](generator.md#GenerationResult), [`request_id`](generator.md#GenerationResult.request_id), [`task_id`](generator.md#GenerationResult.task_id), [`model_name`](generator.md#GenerationRequest.model_name), [`step_index`](generator.md#GenerationRequest.step_index), [`step_index`](generator.md#GenerationResult.step_index), [`task_id`](generator.md#GenerationRequest.task_id), [`code`](generator.md#GenerationResult.code), [`task_name`](generator.md#GenerationRequest.task_name), [`GenerationRequest`](generator.md#GenerationRequest), [`messages`](generator.md#GenerationRequest.messages), [`messages`](generator.md#GenerationResult.messages), [`total_tokens`](generator.md#GenerationResult.total_tokens), [`completion_tokens`](generator.md#GenerationResult.completion_tokens), [`cost`](generator.md#GenerationResult.cost), [`model_name`](generator.md#GenerationResult.model_name), [`prompt_tokens`](generator.md#GenerationResult.prompt_tokens), [`raw_text`](generator.md#GenerationResult.raw_text), [`reasoning_content`](generator.md#GenerationResult.reasoning_content), [`search_metadata`](generator.md#GenerationResult.search_metadata), [`extract_code`](../reward_func_utils.md#extract_code), [`output_dir`](generator.md#GenerationRequest.output_dir), [`output_dir`](generator.md#GenerationResult.output_dir), [`task_name`](generator.md#GenerationResult.task_name), [`data_dir`](generator.md#GenerationResult.data_dir), [`metadata`](generator.md#GenerationResult.metadata), [`request_id`](generator.md#GenerationRequest.request_id), [`data_dir`](generator.md#GenerationRequest.data_dir), [`error`](generator.md#GenerationResult.error), [`metadata`](generator.md#GenerationRequest.metadata), [`search_metadata`](generator.md#GenerationRequest.search_metadata)
- used by: [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`get_stats`](scheduler.md#Scheduler.get_stats), [`_generator`](scheduler.md#Scheduler._generator)

## Module values
- `handler` — [`L54`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L54)
- `logger` — [`L52`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/generator.py#L52)

