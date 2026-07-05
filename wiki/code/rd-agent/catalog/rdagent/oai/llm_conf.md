---
title: 'Module: rdagent/oai/llm_conf.py'
type: catalog
provenance: extracted
module: rdagent/oai/llm_conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.oai.llm_conf`/LLM
symbols:
  LLM_SETTINGS: _SETTINGS.
  LLMSettings.log_llm_chat_content: Settings#log_llm_chat_content.
  LLMSettings.chat_model: Settings#chat_model.
  LLMSettings: Settings#
  LLMSettings.dump_chat_cache: Settings#dump_chat_cache.
  LLMSettings.use_chat_cache: Settings#use_chat_cache.
  LLMSettings.use_auto_chat_cache_seed_gen: Settings#use_auto_chat_cache_seed_gen.
  LLMSettings.chat_model_map: Settings#chat_model_map.
  LLMSettings.chat_max_tokens: Settings#chat_max_tokens.
  LLMSettings.chat_stream: Settings#chat_stream.
  LLMSettings.system_prompt_role: Settings#system_prompt_role.
  LLMSettings.embedding_model: Settings#embedding_model.
  LLMSettings.openai_api_key: Settings#openai_api_key.
  LLMSettings.use_llama2: Settings#use_llama2.
  LLMSettings.chat_use_azure_deepseek: Settings#chat_use_azure_deepseek.
  LLMSettings.reasoning_effort: Settings#reasoning_effort.
  LLMSettings.use_azure: Settings#use_azure.
  LLMSettings.max_retry: Settings#max_retry.
  LLMSettings.dump_embedding_cache: Settings#dump_embedding_cache.
  LLMSettings.use_embedding_cache: Settings#use_embedding_cache.
  LLMSettings.prompt_cache_path: Settings#prompt_cache_path.
  LLMSettings.chat_temperature: Settings#chat_temperature.
  LLMSettings.chat_token_limit: Settings#chat_token_limit.
  LLMSettings.default_system_prompt: Settings#default_system_prompt.
  LLMSettings.embedding_max_str_num: Settings#embedding_max_str_num.
  LLMSettings.use_gcr_endpoint: Settings#use_gcr_endpoint.
  LLMSettings.backend: Settings#backend.
  LLMSettings.enable_response_schema: Settings#enable_response_schema.
  LLMSettings.reasoning_think_rm: Settings#reasoning_think_rm.
  LLMSettings.chat_use_azure: Settings#chat_use_azure.
  LLMSettings.embedding_use_azure: Settings#embedding_use_azure.
  LLMSettings.chat_use_azure_token_provider: Settings#chat_use_azure_token_provider.
  LLMSettings.embedding_use_azure_token_provider: Settings#embedding_use_azure_token_provider.
  LLMSettings.managed_identity_client_id: Settings#managed_identity_client_id.
  LLMSettings.retry_wait_seconds: Settings#retry_wait_seconds.
  LLMSettings.max_past_message_include: Settings#max_past_message_include.
  LLMSettings.timeout_fail_limit: Settings#timeout_fail_limit.
  LLMSettings.violation_fail_limit: Settings#violation_fail_limit.
  LLMSettings.init_chat_cache_seed: Settings#init_chat_cache_seed.
  LLMSettings.openai_api_base: Settings#openai_api_base.
  LLMSettings.chat_openai_api_key: Settings#chat_openai_api_key.
  LLMSettings.chat_openai_base_url: Settings#chat_openai_base_url.
  LLMSettings.chat_azure_api_base: Settings#chat_azure_api_base.
  LLMSettings.chat_azure_api_version: Settings#chat_azure_api_version.
  LLMSettings.chat_seed: Settings#chat_seed.
  LLMSettings.chat_frequency_penalty: Settings#chat_frequency_penalty.
  LLMSettings.chat_presence_penalty: Settings#chat_presence_penalty.
  LLMSettings.embedding_openai_api_key: Settings#embedding_openai_api_key.
  LLMSettings.embedding_openai_base_url: Settings#embedding_openai_base_url.
  LLMSettings.embedding_azure_api_base: Settings#embedding_azure_api_base.
  LLMSettings.embedding_azure_api_version: Settings#embedding_azure_api_version.
  LLMSettings.embedding_max_length: Settings#embedding_max_length.
  LLMSettings.llama2_ckpt_dir: Settings#llama2_ckpt_dir.
  LLMSettings.llama2_tokenizer_path: Settings#llama2_tokenizer_path.
  LLMSettings.llams2_max_batch_size: Settings#llams2_max_batch_size.
  LLMSettings.gcr_endpoint_type: Settings#gcr_endpoint_type.
  LLMSettings.llama2_70b_endpoint: Settings#llama2_70b_endpoint.
  LLMSettings.llama2_70b_endpoint_key: Settings#llama2_70b_endpoint_key.
  LLMSettings.llama2_70b_endpoint_deployment: Settings#llama2_70b_endpoint_deployment.
  LLMSettings.llama3_70b_endpoint: Settings#llama3_70b_endpoint.
  LLMSettings.llama3_70b_endpoint_key: Settings#llama3_70b_endpoint_key.
  LLMSettings.llama3_70b_endpoint_deployment: Settings#llama3_70b_endpoint_deployment.
  LLMSettings.phi2_endpoint: Settings#phi2_endpoint.
  LLMSettings.phi2_endpoint_key: Settings#phi2_endpoint_key.
  LLMSettings.phi2_endpoint_deployment: Settings#phi2_endpoint_deployment.
  LLMSettings.phi3_4k_endpoint: Settings#phi3_4k_endpoint.
  LLMSettings.phi3_4k_endpoint_key: Settings#phi3_4k_endpoint_key.
  LLMSettings.phi3_4k_endpoint_deployment: Settings#phi3_4k_endpoint_deployment.
  LLMSettings.phi3_128k_endpoint: Settings#phi3_128k_endpoint.
  LLMSettings.phi3_128k_endpoint_key: Settings#phi3_128k_endpoint_key.
  LLMSettings.phi3_128k_endpoint_deployment: Settings#phi3_128k_endpoint_deployment.
  LLMSettings.gcr_endpoint_temperature: Settings#gcr_endpoint_temperature.
  LLMSettings.gcr_endpoint_top_p: Settings#gcr_endpoint_top_p.
  LLMSettings.gcr_endpoint_do_sample: Settings#gcr_endpoint_do_sample.
  LLMSettings.gcr_endpoint_max_token: Settings#gcr_endpoint_max_token.
  LLMSettings.chat_azure_deepseek_endpoint: Settings#chat_azure_deepseek_endpoint.
  LLMSettings.chat_azure_deepseek_key: Settings#chat_azure_deepseek_key.
---
# Module: [`rdagent/oai/llm_conf.py`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py)

## Classes
### `LLMSettings`  ·  implements/extends ExtendedBaseSettings
- def: [`rdagent/oai/llm_conf.py:11`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L11) — documented in [rdagent-core-conf](../../../concepts/rdagent-core-conf.md)
- signature: `class LLMSettings(ExtendedBaseSettings):`
- members:
  - `backend` — [`L13`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L13)
  - `chat_azure_api_base` — [`L67`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L67)
  - `chat_azure_api_version` — [`L68`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L68)
  - `chat_azure_deepseek_endpoint` — [`L127`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L127)
  - `chat_azure_deepseek_key` — [`L128`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L128)
  - `chat_frequency_penalty` — [`L73`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L73)
  - `chat_max_tokens` — [`L69`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L69)
  - `chat_model` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L15) — documented in [rdagent-oai-llm_conf](../../../concepts/rdagent-oai-llm_conf.md)
  - `chat_model_map` — [`L130`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L130)
  - `chat_openai_api_key` — [`L65`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L65)
  - `chat_openai_base_url` — [`L66`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L66)
  - `chat_presence_penalty` — [`L74`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L74)
  - `chat_seed` — [`L72`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L72)
  - `chat_stream` — [`L71`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L71)
  - `chat_temperature` — [`L70`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L70)
  - `chat_token_limit` — [`L75`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L75)
  - `chat_use_azure` — [`L35`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L35)
  - `chat_use_azure_deepseek` — [`L126`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L126)
  - `chat_use_azure_token_provider` — [`L38`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L38)
  - `default_system_prompt` — [`L78`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L78)
  - `dump_chat_cache` — [`L43`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L43)
  - `dump_embedding_cache` — [`L45`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L45)
  - `embedding_azure_api_base` — [`L86`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L86)
  - `embedding_azure_api_version` — [`L87`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L87)
  - `embedding_max_length` — [`L89`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L89)
  - `embedding_max_str_num` — [`L88`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L88)
  - `embedding_model` — [`L16`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L16)
  - `embedding_openai_api_key` — [`L84`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L84)
  - `embedding_openai_base_url` — [`L85`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L85)
  - `embedding_use_azure` — [`L36`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L36)
  - `embedding_use_azure_token_provider` — [`L39`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L39)
  - `enable_response_schema` — [`L19`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L19)
  - `gcr_endpoint_do_sample` — [`L123`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L123)
  - `gcr_endpoint_max_token` — [`L124`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L124)
  - `gcr_endpoint_temperature` — [`L121`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L121)
  - `gcr_endpoint_top_p` — [`L122`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L122)
  - `gcr_endpoint_type` — [`L99`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L99)
  - `init_chat_cache_seed` — [`L60`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L60)
  - `llama2_70b_endpoint` — [`L101`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L101)
  - `llama2_70b_endpoint_deployment` — [`L103`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L103)
  - `llama2_70b_endpoint_key` — [`L102`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L102)
  - `llama2_ckpt_dir` — [`L93`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L93)
  - `llama2_tokenizer_path` — [`L94`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L94)
  - `llama3_70b_endpoint` — [`L105`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L105)
  - `llama3_70b_endpoint_deployment` — [`L107`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L107)
  - `llama3_70b_endpoint_key` — [`L106`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L106)
  - `llams2_max_batch_size` — [`L95`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L95)
  - `log_llm_chat_content` — [`L32`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L32) — documented in [rdagent-oai-llm_conf](../../../concepts/rdagent-oai-llm_conf.md)
  - `managed_identity_client_id` — [`L40`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L40)
  - `max_past_message_include` — [`L48`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L48)
  - `max_retry` — [`L41`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L41)
  - `openai_api_base` — [`L64`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L64)
  - `openai_api_key` — [`L63`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L63)
  - `phi2_endpoint` — [`L109`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L109)
  - `phi2_endpoint_deployment` — [`L111`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L111)
  - `phi2_endpoint_key` — [`L110`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L110)
  - `phi3_128k_endpoint` — [`L117`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L117)
  - `phi3_128k_endpoint_deployment` — [`L119`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L119)
  - `phi3_128k_endpoint_key` — [`L118`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L118)
  - `phi3_4k_endpoint` — [`L113`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L113)
  - `phi3_4k_endpoint_deployment` — [`L115`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L115)
  - `phi3_4k_endpoint_key` — [`L114`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L114)
  - `prompt_cache_path` — [`L47`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L47)
  - `reasoning_effort` — [`L18`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L18)
  - `reasoning_think_rm` — [`L23`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L23) — ---
  - `retry_wait_seconds` — [`L42`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L42)
  - `system_prompt_role` — [`L79`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L79) — ---
  - `timeout_fail_limit` — [`L49`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L49)
  - `use_auto_chat_cache_seed_gen` — [`L53`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L53) — ---
  - `use_azure` — [`L34`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L34)
  - `use_chat_cache` — [`L44`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L44) — documented in [rdagent-oai-llm_conf](../../../concepts/rdagent-oai-llm_conf.md)
  - `use_embedding_cache` — [`L46`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L46)
  - `use_gcr_endpoint` — [`L98`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L98)
  - `use_llama2` — [`L92`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L92)
  - `violation_fail_limit` — [`L50`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L50)
- uses (calls/refs, reference-scoped): [`ExtendedBaseSettings`](../core/conf.md#ExtendedBaseSettings), [`LiteLLMSettings`](backend/litellm.md#LiteLLMSettings)
- used by: [`LLM_SETTINGS`](llm_conf.md#LLM_SETTINGS), [`_create_chat_completion_inner_function`](backend/deprec.md#DeprecBackend._create_chat_completion_inner_function), [`ExtendedBaseSettings`](../core/conf.md#ExtendedBaseSettings), [`_create_chat_completion_auto_continue`](backend/base.md#APIBackend._create_chat_completion_auto_continue), [`_try_create_chat_completion_or_embedding`](backend/base.md#APIBackend._try_create_chat_completion_or_embedding), [`gcr_endpoint`](backend/deprec.md#DeprecBackend.gcr_endpoint), [`_create_chat_completion_inner_function`](backend/litellm.md#LiteLLMAPIBackend._create_chat_completion_inner_function), [`llm_log_win`](../log/ui/ds_trace.md#llm_log_win), [`get_complete_kwargs`](backend/litellm.md#LiteLLMAPIBackend.get_complete_kwargs), [`get_sota_exp_to_submit`](../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector.get_sota_exp_to_submit), [`chat_token_limit`](backend/base.md#APIBackend.chat_token_limit), [`embedding_api_key`](backend/deprec.md#DeprecBackend.embedding_api_key), [`_create_embedding_inner_function`](backend/litellm.md#LiteLLMAPIBackend._create_embedding_inner_function), [`client`](backend/deprec.md#DeprecBackend.client), [`embedding_api_version`](backend/deprec.md#DeprecBackend.embedding_api_version), [`_calculate_token_from_messages`](backend/litellm.md#LiteLLMAPIBackend._calculate_token_from_messages), [`build_chat_completion_message`](backend/base.md#ChatSession.build_chat_completion_message), [`get_agent_model`](backend/pydantic_ai.md#get_agent_model), [`use_embedding_cache`](backend/base.md#APIBackend.use_embedding_cache), [`DEFAULT_QLIB_DOT_PATH`](backend/deprec.md#DEFAULT_QLIB_DOT_PATH), [`available_models`](../log/ui/ds_trace.md#available_models), [`chat_model`](backend/deprec.md#DeprecBackend.chat_model), [`generator`](backend/deprec.md#DeprecBackend.generator), [`get_embedding_max_tokens`](utils/embedding.md#get_embedding_max_tokens), [`_create_embedding_inner_function`](backend/deprec.md#DeprecBackend._create_embedding_inner_function), [`encoder`](backend/deprec.md#DeprecBackend.encoder), [`_build_messages`](backend/base.md#APIBackend._build_messages), [`chat_api_version`](backend/deprec.md#DeprecBackend.chat_api_version), [`get_api_backend`](llm_utils.md#get_api_backend), [`embedding_use_azure`](backend/deprec.md#DeprecBackend.embedding_use_azure), [`chat_stream`](backend/deprec.md#DeprecBackend.chat_stream), [`gcr_endpoint_key`](backend/deprec.md#DeprecBackend.gcr_endpoint_key), [`cache`](backend/base.md#SessionChatHistoryCache.cache), [`chat_api_key`](backend/deprec.md#DeprecBackend.chat_api_key), [`chat_use_azure`](backend/deprec.md#DeprecBackend.chat_use_azure), [`chat_model_map`](backend/deprec.md#DeprecBackend.chat_model_map), [`gcr_endpoint_deployment`](backend/deprec.md#DeprecBackend.gcr_endpoint_deployment), [`chat_use_azure_token_provider`](backend/deprec.md#DeprecBackend.chat_use_azure_token_provider), [`embedding_use_azure_token_provider`](backend/deprec.md#DeprecBackend.embedding_use_azure_token_provider), [`__init__`](../core/utils.md#CacheSeedGen.__init__)  (+25 more; 3 test-only)

## Module values
- `LLM_SETTINGS` — [`L133`](../../../../../../raw/code/rd-agent/rdagent/oai/llm_conf.py#L133) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)

