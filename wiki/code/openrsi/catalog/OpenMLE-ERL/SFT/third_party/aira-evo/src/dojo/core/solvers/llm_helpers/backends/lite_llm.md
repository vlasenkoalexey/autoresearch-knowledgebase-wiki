---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.backends.lite_llm`/
symbols:
  LiteLLMClient._query_client: LiteLLMClient#_query_client().
  LiteLLMClient._should_stream: LiteLLMClient#_should_stream().
  LiteLLMClient.model: LiteLLMClient#model.
  LiteLLMClient.query: LiteLLMClient#query().
  logger: logger.
  formatter: formatter.
  FunctionSpec.as_openai_tool_dict: FunctionSpec#as_openai_tool_dict().
  LiteLLMClient.model_prefix: LiteLLMClient#model_prefix.
  FunctionSpec.as_anthropic_tool_dict: FunctionSpec#as_anthropic_tool_dict().
  FunctionSpec.name: FunctionSpec#name.
  LiteLLMClient._calculate_cost: LiteLLMClient#_calculate_cost().
  LiteLLMClient.provider: LiteLLMClient#provider.
  _to_dict: _to_dict().
  LiteLLMClient.client_content_key: LiteLLMClient#client_content_key().
  LiteLLMClient.OutputType: LiteLLMClient#OutputType.
  LiteLLMClient.base_url: LiteLLMClient#base_url.
  LiteLLMClient.api_key: LiteLLMClient#api_key.
  LiteLLMClient._consume_stream: LiteLLMClient#_consume_stream().
  FunctionSpec.json_schema: FunctionSpec#json_schema.
  FunctionSpec.__post_init__: FunctionSpec#__post_init__().
  FunctionSpec.openai_tool_choice_dict: FunctionSpec#openai_tool_choice_dict().
  FunctionSpec.anthropic_tool_choice_dict: FunctionSpec#anthropic_tool_choice_dict().
  handler: handler.
  FunctionSpec: FunctionSpec#
  FunctionSpec.description: FunctionSpec#description.
  LiteLLMClient: LiteLLMClient#
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
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py)

## Classes
### `FunctionSpec`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py:71`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L71)
- signature: `class FunctionSpec(DataClassJsonMixin):`
- members:
  - `anthropic_tool_choice_dict(self)` — [`L107`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L107) — Convert to Anthropic's tool choice format.
  - `as_anthropic_tool_dict(self)` — [`L98`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L98) — Convert to Anthropic's tool format.
  - `as_openai_tool_dict(self)` — [`L81`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L81) — Convert to OpenAI's function format.
  - `openai_tool_choice_dict(self)` — [`L91`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L91)
  - `description` — [`L74`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L74)
  - `json_schema` — [`L73`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L73)
  - `name` — [`L72`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L72)
- protocol/private: `__post_init__`[`L76`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L76)
- used by: [`_query_client`](lite_llm.md#LiteLLMClient._query_client), [`_should_stream`](lite_llm.md#LiteLLMClient._should_stream)

### `LiteLLMClient`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py:115`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L115)
- signature: `class LiteLLMClient:`
- members:
  - `__init__(self, client_cfg)` — [`L120`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L120) — Initialize the OpenAI client with any desired default arguments or configuration.
  - `_calculate_cost(self, prompt_tokens, completion_tokens)` — [`L148`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L148) — Calculate the API cost for a request based on token usage and provider-specific pricing.
  - `client_content_key(self)` — [`L145`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L145)
  - `count_tokens(self, text)` — [`L180`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L180) — Utility method to count tokens in a given text string.
  - `query(self, messages: List[Dict[str, str]], json_schema: Optional[str] = None, function_name: Optional[str] = None, function_description: Optional[str] = None, **model_kwargs)` — [`L403`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L403) — General LLM query for various backends with a single system and user message.
  - `FunctionCallType` — [`L117`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L117)
  - `OutputType` — [`L118`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L118)
  - `PromptType` — [`L116`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L116)
  - `api_key` — [`L128`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L128)
  - `base_url` — [`L125`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L125)
  - `model` — [`L124`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L124)
  - `model_prefix` — [`L134`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L134)
  - `provider` — [`L132`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L132)
  - `use_azure_client` — [`L131`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L131)
- protocol/private: `_consume_stream`[`L199`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L199), `_query_client`[`L238`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L238), `_should_stream`[`L188`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L188)
- uses (calls/refs, reference-scoped): [`as_openai_tool_dict`](lite_llm.md#FunctionSpec.as_openai_tool_dict), [`logger`](lite_llm.md#logger), [`name`](lite_llm.md#FunctionSpec.name), [`_to_dict`](lite_llm.md#_to_dict), [`FunctionSpec`](lite_llm.md#FunctionSpec), [`NUM_RETRIES`](lite_llm.md#NUM_RETRIES), [`NUM_RETRIES_ENV`](lite_llm.md#NUM_RETRIES_ENV), [`STREAM_ENV`](lite_llm.md#STREAM_ENV), [`TIMEOUT`](lite_llm.md#TIMEOUT), [`TIMEOUT_ENV`](lite_llm.md#TIMEOUT_ENV), [`_env_bool`](lite_llm.md#_env_bool), [`_env_float`](lite_llm.md#_env_float), [`_env_int`](lite_llm.md#_env_int)
- used by: [`get_client`](utils.md#get_client)

## Functions
- `_env_bool(name: str, default: bool)` — [`L39`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L39)
- `_env_float(name: str, default: float)` — [`L51`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L51)
- `_env_int(name: str, default: int)` — [`L46`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L46)
- `_to_dict(value: Any)` — [`L56`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L56)

## Module values
- `NUM_RETRIES` — [`L23`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L23)
- `NUM_RETRIES_ENV` — [`L27`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L27)
- `STREAM_ENV` — [`L25`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L25)
- `TIMEOUT` — [`L24`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L24)
- `TIMEOUT_ENV` — [`L26`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L26)
- `formatter` — [`L34`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L34)
- `handler` — [`L33`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L33)
- `logger` — [`L31`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/lite_llm.py#L31)

