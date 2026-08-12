---
title: 'Module: rlm/clients/azure_openai.py'
type: catalog
provenance: extracted
module: rlm/clients/azure_openai.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.azure_openai`/
symbols:
  AzureOpenAIClient.get_usage_summary: AzureOpenAIClient#get_usage_summary().
  AzureOpenAIClient.get_last_usage: AzureOpenAIClient#get_last_usage().
  AzureOpenAIClient._track_cost: AzureOpenAIClient#_track_cost().
  AzureOpenAIClient.completion: AzureOpenAIClient#completion().
  AzureOpenAIClient.acompletion: AzureOpenAIClient#acompletion().
  AzureOpenAIClient: AzureOpenAIClient#
  AzureOpenAIClient.__init__: AzureOpenAIClient#__init__().
  AzureOpenAIClient.client: AzureOpenAIClient#client.
  AzureOpenAIClient.async_client: AzureOpenAIClient#async_client.
  AzureOpenAIClient.model_call_counts: AzureOpenAIClient#model_call_counts.
  AzureOpenAIClient.model_name: AzureOpenAIClient#model_name.
  AzureOpenAIClient.model_input_tokens: AzureOpenAIClient#model_input_tokens.
  AzureOpenAIClient.model_output_tokens: AzureOpenAIClient#model_output_tokens.
  DEFAULT_AZURE_OPENAI_API_KEY: DEFAULT_AZURE_OPENAI_API_KEY.
  AzureOpenAIClient.model_total_tokens: AzureOpenAIClient#model_total_tokens.
  AzureOpenAIClient.last_prompt_tokens: AzureOpenAIClient#last_prompt_tokens.
  AzureOpenAIClient.last_completion_tokens: AzureOpenAIClient#last_completion_tokens.
  AzureOpenAIClient.azure_deployment: AzureOpenAIClient#azure_deployment.
---
# Module: [`rlm/clients/azure_openai.py`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py)

## Classes
### `AzureOpenAIClient`  ·  implements/extends BaseLM
- def: [`rlm/clients/azure_openai.py:17`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L17)
- doc: LM Client for running models with the Azure OpenAI API.
- signature: `class AzureOpenAIClient(BaseLM):`
- members:
  - `acompletion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L93`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L93)
  - `completion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L74`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L74)
  - `get_last_usage(self)` — [`L139`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L139)
  - `get_usage_summary(self)` — [`L129`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L129)
  - `async_client` — [`L58`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L58)
  - `azure_deployment` — [`L66`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L66)
  - `client` — [`L51`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L51)
  - `last_completion_tokens` — [`L127`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L127)
  - `last_prompt_tokens` — [`L126`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L126)
  - `model_call_counts` — [`L69`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L69)
  - `model_input_tokens` — [`L70`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L70)
  - `model_name` — [`L65`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L65)
  - `model_output_tokens` — [`L71`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L71)
  - `model_total_tokens` — [`L72`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L72)
- protocol/private: `__init__`[`L22`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L22), `_track_cost`[`L114`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L114)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`BaseLM`](base_lm.md#BaseLM), [`model_usage_summaries`](../core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](base_lm.md#BaseLM.__init__), [`timeout`](base_lm.md#BaseLM.timeout), [`DEFAULT_AZURE_OPENAI_API_KEY`](azure_openai.md#DEFAULT_AZURE_OPENAI_API_KEY)
- used by: [`BaseLM`](base_lm.md#BaseLM), [`get_last_usage`](base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](base_lm.md#BaseLM.get_usage_summary), [`completion`](base_lm.md#BaseLM.completion), [`get_client`](__init__.md#get_client), [`acompletion`](base_lm.md#BaseLM.acompletion)  (1 test-only)

## Module values
- `DEFAULT_AZURE_OPENAI_API_KEY` — [`L14`](../../../../../../raw/code/rlm/rlm/clients/azure_openai.py#L14)

