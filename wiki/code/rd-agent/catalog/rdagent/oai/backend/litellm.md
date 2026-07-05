---
title: 'Module: rdagent/oai/backend/litellm.py'
type: catalog
provenance: extracted
module: rdagent/oai/backend/litellm.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.oai.backend.litellm`/
symbols:
  LiteLLMAPIBackend._create_chat_completion_inner_function: LiteLLMAPIBackend#_create_chat_completion_inner_function().
  LITELLM_SETTINGS: LITELLM_SETTINGS.
  LiteLLMAPIBackend.get_complete_kwargs: LiteLLMAPIBackend#get_complete_kwargs().
  LiteLLMAPIBackend._create_embedding_inner_function: LiteLLMAPIBackend#_create_embedding_inner_function().
  LiteLLMAPIBackend._calculate_token_from_messages: LiteLLMAPIBackend#_calculate_token_from_messages().
  LiteLLMAPIBackend.__init__: LiteLLMAPIBackend#__init__().
  LiteLLMAPIBackend.supports_response_schema: LiteLLMAPIBackend#supports_response_schema().
  LiteLLMAPIBackend.chat_token_limit: LiteLLMAPIBackend#chat_token_limit().
  cls: cls.
  LiteLLMAPIBackend: LiteLLMAPIBackend#
  ACC_COST: ACC_COST.
  LiteLLMSettings: LiteLLMSettings#
  LiteLLMAPIBackend._has_logged_settings: LiteLLMAPIBackend#_has_logged_settings.
  LiteLLMAPIBackend.CompleteKwargs: LiteLLMAPIBackend#CompleteKwargs#
  _reduce_no_init: _reduce_no_init().
  LiteLLMAPIBackend.CompleteKwargs.model: LiteLLMAPIBackend#CompleteKwargs#model.
  LiteLLMAPIBackend.CompleteKwargs.temperature: LiteLLMAPIBackend#CompleteKwargs#temperature.
  LiteLLMAPIBackend.CompleteKwargs.max_tokens: LiteLLMAPIBackend#CompleteKwargs#max_tokens.
  LiteLLMAPIBackend.CompleteKwargs.reasoning_effort: LiteLLMAPIBackend#CompleteKwargs#reasoning_effort.
  LiteLLMSettings.Config: LiteLLMSettings#Config#
  LiteLLMSettings.Config.env_prefix: LiteLLMSettings#Config#env_prefix.
---
# Module: [`rdagent/oai/backend/litellm.py`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py)

## Classes
### `CompleteKwargs`  ·  implements/extends _TypedDict
- def: [`rdagent/oai/backend/litellm.py:89`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L89)
- signature: `class CompleteKwargs(TypedDict):`
- members:
  - `max_tokens` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L92)
  - `model` — [`L90`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L90)
  - `reasoning_effort` — [`L93`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L93)
  - `temperature` — [`L91`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L91)
- used by: [`get_complete_kwargs`](litellm.md#LiteLLMAPIBackend.get_complete_kwargs)

### `Config`
- def: [`rdagent/oai/backend/litellm.py:37`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L37)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L38)

### `LiteLLMAPIBackend`  ·  implements/extends APIBackend
- def: [`rdagent/oai/backend/litellm.py:48`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L48)
- doc: LiteLLM implementation of APIBackend interface
- signature: `class LiteLLMAPIBackend(APIBackend):`
- members:
  - `_calculate_token_from_messages(self, messages: list[dict[str, Any]])` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L60) — Calculate the token count from messages
  - `_create_chat_completion_inner_function(self, messages: list[dict[str, Any]], response_format: Optional[Union[dict, Type[BaseModel]]] = None, *args, **kwargs)` — [`L127`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L127) — Call the chat completion function — documented in [rdagent-oai-backend-base](../../../../concepts/rdagent-oai-backend-base.md)
  - `_create_embedding_inner_function(self, input_content_list: list[str])` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L71) — Call the embedding function
  - `chat_token_limit(self)` — [`L233`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L233) — Suggest an input token limit, ensuring enough space in the context window for the maximum output tokens. — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `get_complete_kwargs(self)` — [`L95`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L95) — return several key settings for completion — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `supports_response_schema(self)` — [`L226`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L226) — Check if the backend supports function calling
- protocol/private: `__init__`[`L53`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L53), `_has_logged_settings`[`L51`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L51)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`warning`](../../log/logger.md#RDAgentLog.warning), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`LogColors`](../../log/utils/__init__.md#LogColors), [`LITELLM_SETTINGS`](litellm.md#LITELLM_SETTINGS), [`END`](../../log/utils/__init__.md#LogColors.END), [`chat_token_limit`](base.md#APIBackend.chat_token_limit), [`log_llm_chat_content`](../llm_conf.md#LLMSettings.log_llm_chat_content), [`_build_log_messages`](base.md#APIBackend._build_log_messages), [`CYAN`](../../log/utils/__init__.md#LogColors.CYAN), [`APIBackend`](base.md#APIBackend), [`chat_model`](../llm_conf.md#LLMSettings.chat_model), [`_tag`](../../log/logger.md#RDAgentLog._tag), [`chat_model_map`](../llm_conf.md#LLMSettings.chat_model_map), [`ACC_COST`](litellm.md#ACC_COST), [`chat_max_tokens`](../llm_conf.md#LLMSettings.chat_max_tokens), [`chat_stream`](../llm_conf.md#LLMSettings.chat_stream), [`MAGENTA`](../../log/utils/__init__.md#LogColors.MAGENTA), [`embedding_model`](../llm_conf.md#LLMSettings.embedding_model), [`CompleteKwargs`](litellm.md#LiteLLMAPIBackend.CompleteKwargs), [`BLUE`](../../log/utils/__init__.md#LogColors.BLUE), [`GREEN`](../../log/utils/__init__.md#LogColors.GREEN), [`__init__`](base.md#APIBackend.__init__), [`chat_temperature`](../llm_conf.md#LLMSettings.chat_temperature), [`reasoning_effort`](../llm_conf.md#LLMSettings.reasoning_effort), [`RED`](../../log/utils/__init__.md#LogColors.RED), [`YELLOW`](../../log/utils/__init__.md#LogColors.YELLOW), [`enable_response_schema`](../llm_conf.md#LLMSettings.enable_response_schema), [`max_tokens`](litellm.md#LiteLLMAPIBackend.CompleteKwargs.max_tokens), [`model`](litellm.md#LiteLLMAPIBackend.CompleteKwargs.model), [`reasoning_effort`](litellm.md#LiteLLMAPIBackend.CompleteKwargs.reasoning_effort), [`temperature`](litellm.md#LiteLLMAPIBackend.CompleteKwargs.temperature)
- used by: [`chat_token_limit`](base.md#APIBackend.chat_token_limit), [`get_agent_model`](pydantic_ai.md#get_agent_model), [`APIBackend`](base.md#APIBackend), [`supports_response_schema`](base.md#APIBackend.supports_response_schema), [`_calculate_token_from_messages`](base.md#APIBackend._calculate_token_from_messages), [`_create_chat_completion_inner_function`](base.md#APIBackend._create_chat_completion_inner_function), [`_create_embedding_inner_function`](base.md#APIBackend._create_embedding_inner_function)

### `LiteLLMSettings`  ·  implements/extends LLMSettings
- def: [`rdagent/oai/backend/litellm.py:35`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L35)
- signature: `class LiteLLMSettings(LLMSettings):`
- uses (calls/refs, reference-scoped): [`LLMSettings`](../llm_conf.md#LLMSettings)
- used by: [`LITELLM_SETTINGS`](litellm.md#LITELLM_SETTINGS), [`LLMSettings`](../llm_conf.md#LLMSettings)

## Functions
- `_reduce_no_init(exc: Exception)` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L25)

## Module values
- `ACC_COST` — [`L45`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L45)
- `LITELLM_SETTINGS` — [`L44`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L44)
- `cls` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/litellm.py#L31)

