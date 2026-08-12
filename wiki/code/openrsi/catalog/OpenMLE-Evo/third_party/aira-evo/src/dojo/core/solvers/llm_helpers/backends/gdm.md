---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.llm_helpers.backends.gdm`/
symbols:
  GDMClient._query_client: GDMClient#_query_client().
  GDMClient.generate_response: GDMClient#generate_response().
  formatter: formatter.
  FunctionSpec.as_openai_tool_dict: FunctionSpec#as_openai_tool_dict().
  GDMClient.query: GDMClient#query().
  logger: logger.
  GDMClient: GDMClient#
  GDMClient.OutputType: GDMClient#OutputType.
  GDMClient.to_schema: GDMClient#to_schema().
  GDMClient._client: GDMClient#_client.
  FunctionSpec.__post_init__: FunctionSpec#__post_init__().
  FunctionSpec.openai_tool_choice_dict: FunctionSpec#openai_tool_choice_dict().
  handler: handler.
  FunctionSpec.name: FunctionSpec#name.
  FunctionSpec.json_schema: FunctionSpec#json_schema.
  GDMClient.model: GDMClient#model.
  FunctionSpec: FunctionSpec#
  FunctionSpec.description: FunctionSpec#description.
  GDMClient.FunctionCallType: GDMClient#FunctionCallType.
  GDMClient.api_key: GDMClient#api_key.
  GDMClient.PromptType: GDMClient#PromptType.
  GDMClient.__init__: GDMClient#__init__().
  GDMClient.client_content_key: GDMClient#client_content_key().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py)

## Classes
### `FunctionSpec`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py:37`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L37)
- signature: `class FunctionSpec(DataClassJsonMixin):`
- members:
  - `as_openai_tool_dict(self)` — [`L47`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L47) — Convert to OpenAI's function format.
  - `openai_tool_choice_dict(self)` — [`L57`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L57)
  - `description` — [`L40`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L40)
  - `json_schema` — [`L39`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L39)
  - `name` — [`L38`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L38)
- protocol/private: `__post_init__`[`L42`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L42)
- used by: [`_query_client`](gdm.md#GDMClient._query_client)

### `GDMClient`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py:64`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L64)
- signature: `class GDMClient:`
- members:
  - `client_content_key(self)` — [`L76`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L76)
  - `generate_response(self, messages: list, functions: list = None, **model_kwargs)` — [`L79`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L79) — Call the Gemini model with a conversation and optional function definitions.
  - `query(self, messages: List[Dict[str, str]], json_schema: Optional[str] = None, function_name: Optional[str] = None, function_description: Optional[str] = None, **model_kwargs)` — [`L254`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L254) — General LLM query for various backends with a single system and user message.
  - `to_schema(schema)` — [`L109`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L109)
  - `FunctionCallType` — [`L66`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L66)
  - `OutputType` — [`L67`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L67)
  - `PromptType` — [`L65`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L65)
  - `api_key` — [`L71`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L71)
  - `model` — [`L70`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L70)
- protocol/private: `__init__`[`L69`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L69), `_client`[`L73`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L73), `_query_client`[`L216`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L216)
- uses (calls/refs, reference-scoped): [`as_openai_tool_dict`](gdm.md#FunctionSpec.as_openai_tool_dict), [`logger`](gdm.md#logger), [`FunctionSpec`](gdm.md#FunctionSpec)
- used by: [`generate_journal_report`](../../../../analysis_utils/meta_tree_analysis.md#generate_journal_report), [`summarize_single_crash`](../../../../analysis_utils/meta_error_summary.md#summarize_single_crash), [`get_client`](utils.md#get_client), [`final_report_from_summaries`](../../../../analysis_utils/meta_error_summary.md#final_report_from_summaries), [`create_client`](../../../../analysis_utils/meta_error_summary.md#create_client), [`create_client`](../../../../analysis_utils/meta_tree_analysis.md#create_client)

## Module values
- `formatter` — [`L31`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L31)
- `handler` — [`L30`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L30)
- `logger` — [`L28`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/llm_helpers/backends/gdm.py#L28)

