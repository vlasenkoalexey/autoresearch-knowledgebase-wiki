---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.backends.open_ai`/
symbols:
  OpenAIClient._query_client: OpenAIClient#_query_client().
  OpenAIClient.query: OpenAIClient#query().
  OpenAIClient._client: OpenAIClient#_client.
  logger: logger.
  formatter: formatter.
  FunctionSpec.as_openai_tool_dict: FunctionSpec#as_openai_tool_dict().
  OpenAIClient.client_content_key: OpenAIClient#client_content_key().
  OpenAIClient.OutputType: OpenAIClient#OutputType.
  FunctionSpec.name: FunctionSpec#name.
  OpenAIClient.use_azure_client: OpenAIClient#use_azure_client.
  FunctionSpec.__post_init__: FunctionSpec#__post_init__().
  FunctionSpec.openai_tool_choice_dict: FunctionSpec#openai_tool_choice_dict().
  handler: handler.
  FunctionSpec.json_schema: FunctionSpec#json_schema.
  OpenAIClient: OpenAIClient#
  OpenAIClient.model: OpenAIClient#model.
  OpenAIClient.base_url: OpenAIClient#base_url.
  OpenAIClient.api_key: OpenAIClient#api_key.
  FunctionSpec: FunctionSpec#
  FunctionSpec.description: FunctionSpec#description.
  OpenAIClient.FunctionCallType: OpenAIClient#FunctionCallType.
  OpenAIClient.PromptType: OpenAIClient#PromptType.
  OpenAIClient.__init__: OpenAIClient#__init__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py)

## Classes
### `FunctionSpec`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py:30`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L30)
- signature: `class FunctionSpec(DataClassJsonMixin):`
- members:
  - `as_openai_tool_dict(self)` — [`L40`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L40) — Convert to OpenAI's function format.
  - `openai_tool_choice_dict(self)` — [`L50`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L50)
  - `description` — [`L33`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L33)
  - `json_schema` — [`L32`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L32)
  - `name` — [`L31`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L31)
- protocol/private: `__post_init__`[`L35`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L35)
- used by: [`_query_client`](open_ai.md#OpenAIClient._query_client)

### `OpenAIClient`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py:57`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L57)
- signature: `class OpenAIClient:`
- members:
  - `__init__(self, client_cfg)` — [`L62`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L62) — Initialize the OpenAI client with any desired default arguments or configuration.
  - `client_content_key(self)` — [`L81`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L81)
  - `query(self, messages: List[Dict[str, str]], json_schema: Optional[str] = None, function_name: Optional[str] = None, function_description: Optional[str] = None, **model_kwargs)` — [`L164`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L164) — General LLM query for various backends with a single system and user message.
  - `FunctionCallType` — [`L59`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L59)
  - `OutputType` — [`L60`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L60)
  - `PromptType` — [`L58`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L58)
  - `api_key` — [`L68`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L68)
  - `base_url` — [`L67`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L67)
  - `model` — [`L66`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L66)
  - `use_azure_client` — [`L69`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L69)
- protocol/private: `_client`[`L72`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L72), `_query_client`[`L84`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L84)
- uses (calls/refs, reference-scoped): [`as_openai_tool_dict`](open_ai.md#FunctionSpec.as_openai_tool_dict), [`logger`](open_ai.md#logger), [`name`](open_ai.md#FunctionSpec.name), [`FunctionSpec`](open_ai.md#FunctionSpec)
- used by: [`__call__`](../generic_llm.md#GenericLLM.__call__), [`_query_client_with_limit`](../generic_llm.md#GenericLLM._query_client_with_limit), [`get_client`](utils.md#get_client), [`client_content_key`](../generic_llm.md#GenericLLM.client_content_key)

## Module values
- `formatter` — [`L24`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L24)
- `handler` — [`L23`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L23)
- `logger` — [`L21`](../../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/open_ai.py#L21)

