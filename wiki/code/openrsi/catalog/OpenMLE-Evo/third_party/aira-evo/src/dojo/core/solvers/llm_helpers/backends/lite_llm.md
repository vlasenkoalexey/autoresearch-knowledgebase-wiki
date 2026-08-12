---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.backends.lite_llm`/
symbols:
  LiteLLMClient._query_client: LiteLLMClient#_query_client().
  LiteLLMClient._should_stream: LiteLLMClient#_should_stream().
  LiteLLMClient.query: LiteLLMClient#query().
  LiteLLMClient.model: LiteLLMClient#model.
  logger: logger.
  formatter: formatter.
  FunctionSpec.as_openai_tool_dict: FunctionSpec#as_openai_tool_dict().
  LiteLLMClient.api_key: LiteLLMClient#api_key.
  FunctionSpec.as_anthropic_tool_dict: FunctionSpec#as_anthropic_tool_dict().
  FunctionSpec.name: FunctionSpec#name.
  LiteLLMClient.model_prefix: LiteLLMClient#model_prefix.
  LiteLLMClient._calculate_cost: LiteLLMClient#_calculate_cost().
  LiteLLMClient.provider: LiteLLMClient#provider.
  _to_dict: _to_dict().
  LiteLLMClient.client_content_key: LiteLLMClient#client_content_key().
  LiteLLMClient.OutputType: LiteLLMClient#OutputType.
  LiteLLMClient._consume_stream: LiteLLMClient#_consume_stream().
  FunctionSpec.json_schema: FunctionSpec#json_schema.
  FunctionSpec.__post_init__: FunctionSpec#__post_init__().
  FunctionSpec.openai_tool_choice_dict: FunctionSpec#openai_tool_choice_dict().
  FunctionSpec.anthropic_tool_choice_dict: FunctionSpec#anthropic_tool_choice_dict().
  handler: handler.
  FunctionSpec: FunctionSpec#
  FunctionSpec.description: FunctionSpec#description.
  LiteLLMClient: LiteLLMClient#
  LiteLLMClient.base_url: LiteLLMClient#base_url.
  LiteLLMClient.count_tokens: LiteLLMClient#count_tokens().
  NUM_RETRIES: NUM_RETRIES.
  TIMEOUT: TIMEOUT.
  STREAM_ENV: STREAM_ENV.
  TIMEOUT_ENV: TIMEOUT_ENV.
  NUM_RETRIES_ENV: NUM_RETRIES_ENV.
  _env_bool: _env_bool().
  _env_int: _env_int().
  _env_float: _env_float().
  LiteLLMClient.FunctionCallType: LiteLLMClient#FunctionCallType.
  LiteLLMClient.use_azure_client: LiteLLMClient#use_azure_client.
  LiteLLMClient.PromptType: LiteLLMClient#PromptType.
  LiteLLMClient.__init__: LiteLLMClient#__init__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py)

## Classes
### `FunctionSpec`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py:72`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L72)
- signature: `class FunctionSpec(DataClassJsonMixin):`
- members:
  - `anthropic_tool_choice_dict(self)` — [`L108`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L108) — Convert to Anthropic's tool choice format.
  - `as_anthropic_tool_dict(self)` — [`L99`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L99) — Convert to Anthropic's tool format.
  - `as_openai_tool_dict(self)` — [`L82`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L82) — Convert to OpenAI's function format.
  - `openai_tool_choice_dict(self)` — [`L92`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L92)
  - `description` — [`L75`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L75)
  - `json_schema` — [`L74`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L74)
  - `name` — [`L73`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L73)
- protocol/private: `__post_init__`[`L77`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L77)
- used by: [`_query_client`](lite_llm.md#LiteLLMClient._query_client), [`_should_stream`](lite_llm.md#LiteLLMClient._should_stream)

### `LiteLLMClient`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py:116`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L116)
- signature: `class LiteLLMClient:`
- members:
  - `__init__(self, client_cfg)` — [`L121`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L121) — Initialize the OpenAI client with any desired default arguments or configuration.
  - `_calculate_cost(self, prompt_tokens, completion_tokens)` — [`L151`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L151) — Calculate the API cost for a request based on token usage and provider-specific pricing.
  - `client_content_key(self)` — [`L148`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L148)
  - `count_tokens(self, text)` — [`L183`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L183) — Utility method to count tokens in a given text string.
  - `query(self, messages: List[Dict[str, str]], json_schema: Optional[str] = None, function_name: Optional[str] = None, function_description: Optional[str] = None, **model_kwargs)` — [`L405`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L405) — General LLM query for various backends with a single system and user message.
  - `FunctionCallType` — [`L118`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L118)
  - `OutputType` — [`L119`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L119)
  - `PromptType` — [`L117`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L117)
  - `api_key` — [`L129`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L129)
  - `base_url` — [`L126`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L126)
  - `model` — [`L125`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L125)
  - `model_prefix` — [`L139`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L139)
  - `provider` — [`L137`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L137)
  - `use_azure_client` — [`L136`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L136)
- protocol/private: `_consume_stream`[`L202`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L202), `_query_client`[`L241`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L241), `_should_stream`[`L191`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L191)
- uses (calls/refs, reference-scoped): [`as_openai_tool_dict`](lite_llm.md#FunctionSpec.as_openai_tool_dict), [`logger`](lite_llm.md#logger), [`name`](lite_llm.md#FunctionSpec.name), [`_to_dict`](lite_llm.md#_to_dict), [`FunctionSpec`](lite_llm.md#FunctionSpec), [`NUM_RETRIES`](lite_llm.md#NUM_RETRIES), [`NUM_RETRIES_ENV`](lite_llm.md#NUM_RETRIES_ENV), [`STREAM_ENV`](lite_llm.md#STREAM_ENV), [`TIMEOUT`](lite_llm.md#TIMEOUT), [`TIMEOUT_ENV`](lite_llm.md#TIMEOUT_ENV), [`_env_bool`](lite_llm.md#_env_bool), [`_env_float`](lite_llm.md#_env_float), [`_env_int`](lite_llm.md#_env_int)
- used by: [`get_client`](utils.md#get_client)

## Functions
- `_env_bool(name: str, default: bool)` — [`L40`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L40)
- `_env_float(name: str, default: float)` — [`L52`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L52)
- `_env_int(name: str, default: int)` — [`L47`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L47)
- `_to_dict(value: Any)` — [`L57`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L57)

## Module values
- `NUM_RETRIES` — [`L24`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L24)
- `NUM_RETRIES_ENV` — [`L28`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L28)
- `STREAM_ENV` — [`L26`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L26)
- `TIMEOUT` — [`L25`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L25)
- `TIMEOUT_ENV` — [`L27`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L27)
- `formatter` — [`L35`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L35)
- `handler` — [`L34`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L34)
- `logger` — [`L32`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L32)

