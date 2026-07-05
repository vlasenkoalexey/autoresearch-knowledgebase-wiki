---
title: 'Module: rdagent/oai/backend/deprec.py'
type: catalog
provenance: extracted
module: rdagent/oai/backend/deprec.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.oai.backend.deprec`/
symbols:
  DeprecBackend._create_chat_completion_inner_function: DeprecBackend#_create_chat_completion_inner_function().
  DeprecBackend.gcr_endpoint: DeprecBackend#gcr_endpoint.
  DeprecBackend.embedding_api_key: DeprecBackend#embedding_api_key.
  DeprecBackend.client: DeprecBackend#client.
  DeprecBackend.embedding_api_version: DeprecBackend#embedding_api_version.
  DeprecBackend._calculate_token_from_messages: DeprecBackend#_calculate_token_from_messages().
  DeprecBackend.embedding_client: DeprecBackend#embedding_client.
  DEFAULT_QLIB_DOT_PATH: DEFAULT_QLIB_DOT_PATH.
  DeprecBackend.chat_client: DeprecBackend#chat_client.
  DeprecBackend.chat_model: DeprecBackend#chat_model.
  DeprecBackend.generator: DeprecBackend#generator.
  DeprecBackend._get_encoder: DeprecBackend#_get_encoder().
  DeprecBackend.encoder: DeprecBackend#encoder.
  DeprecBackend._create_embedding_inner_function: DeprecBackend#_create_embedding_inner_function().
  DeprecBackend.chat_api_version: DeprecBackend#chat_api_version.
  DeprecBackend.embedding_use_azure: DeprecBackend#embedding_use_azure.
  DeprecBackend.gcr_endpoint_key: DeprecBackend#gcr_endpoint_key.
  DeprecBackend.chat_stream: DeprecBackend#chat_stream.
  DeprecBackend.chat_use_azure: DeprecBackend#chat_use_azure.
  DeprecBackend.chat_api_key: DeprecBackend#chat_api_key.
  DeprecBackend.gcr_endpoint_deployment: DeprecBackend#gcr_endpoint_deployment.
  DeprecBackend.chat_model_map: DeprecBackend#chat_model_map.
  ConvManager.path: ConvManager#path.
  DeprecBackend.chat_use_azure_token_provider: DeprecBackend#chat_use_azure_token_provider.
  DeprecBackend.embedding_use_azure_token_provider: DeprecBackend#embedding_use_azure_token_provider.
  DeprecBackend.__init__: DeprecBackend#__init__().
  DeprecBackend.managed_identity_client_id: DeprecBackend#managed_identity_client_id.
  DeprecBackend.embedding_model: DeprecBackend#embedding_model.
  DeprecBackend.use_llama2: DeprecBackend#use_llama2.
  DeprecBackend.use_gcr_endpoint: DeprecBackend#use_gcr_endpoint.
  DeprecBackend.chat_use_azure_deepseek: DeprecBackend#chat_use_azure_deepseek.
  ConvManager._rotate_files: ConvManager#_rotate_files().
  DeprecBackend.gcr_endpoint_temperature: DeprecBackend#gcr_endpoint_temperature.
  DeprecBackend.gcr_endpoint_top_p: DeprecBackend#gcr_endpoint_top_p.
  DeprecBackend.gcr_endpoint_max_token: DeprecBackend#gcr_endpoint_max_token.
  DeprecBackend.chat_openai_base_url: DeprecBackend#chat_openai_base_url.
  DeprecBackend.embedding_openai_base_url: DeprecBackend#embedding_openai_base_url.
  DeprecBackend.chat_api_base: DeprecBackend#chat_api_base.
  DeprecBackend.chat_seed: DeprecBackend#chat_seed.
  DeprecBackend.embedding_api_base: DeprecBackend#embedding_api_base.
  ConvManager.append: ConvManager#append().
  DeprecBackend.gcr_endpoint_do_sample: DeprecBackend#gcr_endpoint_do_sample.
  DeprecBackend: DeprecBackend#
  DeprecBackend.headers: DeprecBackend#headers.
  ConvManager.__init__: ConvManager#__init__().
  ConvManager.recent_n: ConvManager#recent_n.
  DeprecBackend._azure_patch: DeprecBackend#_azure_patch().
  ConvManager: ConvManager#
  DeprecBackend.supports_response_schema: DeprecBackend#supports_response_schema().
---
# Module: [`rdagent/oai/backend/deprec.py`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py)

## Classes
### `ConvManager`
- def: [`rdagent/oai/backend/deprec.py:64`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L64)
- doc: This is a conversation manager of LLM
- signature: `class ConvManager:`
- members:
  - `append(self, conv: tuple[list, str])` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L92)
  - `path` — [`L75`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L75)
  - `recent_n` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L77)
- protocol/private: `__init__`[`L70`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L70), `_rotate_files`[`L79`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L79)
- uses (calls/refs, reference-scoped): [`DEFAULT_QLIB_DOT_PATH`](deprec.md#DEFAULT_QLIB_DOT_PATH)

### `DeprecBackend`  ·  implements/extends APIBackend
- def: [`rdagent/oai/backend/deprec.py:99`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L99)
- doc: This is a unified interface for different backends.
- signature: `class DeprecBackend(APIBackend):`
- members:
  - `_azure_patch(model: str)` — [`L246`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L246) — When using Azure API, self.chat_model is the deployment name that can be any string.
  - `_create_chat_completion_inner_function(self, messages: list[dict[str, Any]], response_format: Optional[Union[dict, Type[BaseModel]]] = None, add_json_in_prompt: bool = False, *args, **kwargs)` — [`L294`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L294) — seed : Optional[int] — documented in [rdagent-oai-backend-base](../../../../concepts/rdagent-oai-backend-base.md)
  - `_get_encoder(self)` — [`L238`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L238) — tiktoken.encoding_for_model(self.chat_model) does not cover all cases it should consider.
  - `supports_response_schema(self)` — [`L266`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L266) — Check if the backend supports function calling.
  - `chat_api_base` — [`L191`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L191)
  - `chat_api_key` — [`L179`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L179)
  - `chat_api_version` — [`L192`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L192)
  - `chat_client` — [`L211`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L211)
  - `chat_model` — [`L159`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L159)
  - `chat_model_map` — [`L158`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L158) — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `chat_openai_base_url` — [`L189`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L189)
  - `chat_seed` — [`L194`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L194)
  - `chat_stream` — [`L169`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L169)
  - `chat_use_azure` — [`L171`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L171)
  - `chat_use_azure_deepseek` — [`L236`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L236)
  - `chat_use_azure_token_provider` — [`L173`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L173)
  - `client` — [`L162`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L162)
  - `embedding_api_base` — [`L197`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L197)
  - `embedding_api_key` — [`L182`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L182)
  - `embedding_api_version` — [`L198`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L198)
  - `embedding_client` — [`L222`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L222)
  - `embedding_model` — [`L196`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L196)
  - `embedding_openai_base_url` — [`L190`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L190)
  - `embedding_use_azure` — [`L172`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L172)
  - `embedding_use_azure_token_provider` — [`L174`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L174)
  - `encoder` — [`L122`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L122)
  - `gcr_endpoint` — [`L128`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L128)
  - `gcr_endpoint_deployment` — [`L127`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L127)
  - `gcr_endpoint_do_sample` — [`L154`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L154)
  - `gcr_endpoint_key` — [`L126`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L126)
  - `gcr_endpoint_max_token` — [`L155`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L155)
  - `gcr_endpoint_temperature` — [`L152`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L152)
  - `gcr_endpoint_top_p` — [`L153`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L153)
  - `generator` — [`L116`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L116)
  - `headers` — [`L148`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L148)
  - `managed_identity_client_id` — [`L175`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L175)
  - `use_gcr_endpoint` — [`L235`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L235)
  - `use_llama2` — [`L234`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L234)
- protocol/private: `__init__`[`L109`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L109), `_calculate_token_from_messages`[`L467`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L467), `_create_embedding_inner_function`[`L273`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L273)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`LLM_SETTINGS`](../llm_conf.md#LLM_SETTINGS), [`warning`](../../log/logger.md#RDAgentLog.warning), [`LogColors`](../../log/utils/__init__.md#LogColors), [`error`](../../log/logger.md#RDAgentLog.error), [`END`](../../log/utils/__init__.md#LogColors.END), [`log_llm_chat_content`](../llm_conf.md#LLMSettings.log_llm_chat_content), [`_build_log_messages`](base.md#APIBackend._build_log_messages), [`CYAN`](../../log/utils/__init__.md#LogColors.CYAN), [`APIBackend`](base.md#APIBackend), [`chat_model`](../llm_conf.md#LLMSettings.chat_model), [`_tag`](../../log/logger.md#RDAgentLog._tag), [`chat_model_map`](../llm_conf.md#LLMSettings.chat_model_map), [`chat_max_tokens`](../llm_conf.md#LLMSettings.chat_max_tokens), [`chat_stream`](../llm_conf.md#LLMSettings.chat_stream), [`system_prompt_role`](../llm_conf.md#LLMSettings.system_prompt_role), [`chat_use_azure_deepseek`](../llm_conf.md#LLMSettings.chat_use_azure_deepseek), [`embedding_model`](../llm_conf.md#LLMSettings.embedding_model), [`openai_api_key`](../llm_conf.md#LLMSettings.openai_api_key), [`use_llama2`](../llm_conf.md#LLMSettings.use_llama2), [`__init__`](base.md#APIBackend.__init__), [`chat_temperature`](../llm_conf.md#LLMSettings.chat_temperature), [`embedding_max_str_num`](../llm_conf.md#LLMSettings.embedding_max_str_num), [`use_azure`](../llm_conf.md#LLMSettings.use_azure), [`use_gcr_endpoint`](../llm_conf.md#LLMSettings.use_gcr_endpoint), [`chat_azure_api_base`](../llm_conf.md#LLMSettings.chat_azure_api_base), [`chat_azure_api_version`](../llm_conf.md#LLMSettings.chat_azure_api_version), [`chat_azure_deepseek_endpoint`](../llm_conf.md#LLMSettings.chat_azure_deepseek_endpoint), [`chat_azure_deepseek_key`](../llm_conf.md#LLMSettings.chat_azure_deepseek_key), [`chat_frequency_penalty`](../llm_conf.md#LLMSettings.chat_frequency_penalty), [`chat_openai_api_key`](../llm_conf.md#LLMSettings.chat_openai_api_key), [`chat_openai_base_url`](../llm_conf.md#LLMSettings.chat_openai_base_url), [`chat_presence_penalty`](../llm_conf.md#LLMSettings.chat_presence_penalty), [`chat_seed`](../llm_conf.md#LLMSettings.chat_seed), [`chat_use_azure`](../llm_conf.md#LLMSettings.chat_use_azure), [`chat_use_azure_token_provider`](../llm_conf.md#LLMSettings.chat_use_azure_token_provider), [`embedding_azure_api_base`](../llm_conf.md#LLMSettings.embedding_azure_api_base), [`embedding_azure_api_version`](../llm_conf.md#LLMSettings.embedding_azure_api_version), [`embedding_openai_api_key`](../llm_conf.md#LLMSettings.embedding_openai_api_key)  (+27 more)
- used by: [`APIBackend`](base.md#APIBackend), [`supports_response_schema`](base.md#APIBackend.supports_response_schema), [`_calculate_token_from_messages`](base.md#APIBackend._calculate_token_from_messages), [`_create_chat_completion_inner_function`](base.md#APIBackend._create_chat_completion_inner_function), [`_create_embedding_inner_function`](base.md#APIBackend._create_embedding_inner_function)

## Module values
- `DEFAULT_QLIB_DOT_PATH` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/deprec.py#L30)

