---
title: 'Module: rlm/clients/openai.py'
type: catalog
provenance: extracted
module: rlm/clients/openai.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.openai`/
symbols:
  OpenAIClient.get_usage_summary: OpenAIClient#get_usage_summary().
  OpenAIClient: OpenAIClient#
  OpenAIClient.__init__: OpenAIClient#__init__().
  OpenAIClient.acompletion: OpenAIClient#acompletion().
  OpenAIClient.completion: OpenAIClient#completion().
  OpenAIClient.get_last_usage: OpenAIClient#get_last_usage().
  OpenAIClient._track_cost: OpenAIClient#_track_cost().
  OpenAIClient.last_cost: OpenAIClient#last_cost.
  DEFAULT_PRIME_INTELLECT_BASE_URL: DEFAULT_PRIME_INTELLECT_BASE_URL.
  OpenAIClient.client: OpenAIClient#client.
  OpenAIClient.model_call_counts: OpenAIClient#model_call_counts.
  _normalize_sampling_args: _normalize_sampling_args().
  _merge_extra_body: _merge_extra_body().
  OpenAIClient.model_name: OpenAIClient#model_name.
  OpenAIClient.model_input_tokens: OpenAIClient#model_input_tokens.
  OpenAIClient.model_output_tokens: OpenAIClient#model_output_tokens.
  OpenAIClient.model_costs: OpenAIClient#model_costs.
  DEFAULT_OPENAI_API_KEY: DEFAULT_OPENAI_API_KEY.
  DEFAULT_OPENROUTER_API_KEY: DEFAULT_OPENROUTER_API_KEY.
  DEFAULT_VERCEL_API_KEY: DEFAULT_VERCEL_API_KEY.
  DEFAULT_PRIME_API_KEY: DEFAULT_PRIME_API_KEY.
  OpenAIClient.async_client: OpenAIClient#async_client.
  OpenAIClient.model_total_tokens: OpenAIClient#model_total_tokens.
  OpenAIClient.last_prompt_tokens: OpenAIClient#last_prompt_tokens.
  OpenAIClient.last_completion_tokens: OpenAIClient#last_completion_tokens.
  OpenAIClient.base_url: OpenAIClient#base_url.
---
# Module: [`rlm/clients/openai.py`](../../../../../../raw/code/rlm/rlm/clients/openai.py)

## Classes
### `OpenAIClient`  ·  implements/extends BaseLM
- def: [`rlm/clients/openai.py:45`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L45) — documented in [rlm-clients-openai](../../../concepts/rlm-clients-openai.md)
- doc: LM Client for running models with the OpenAI API. Works with vLLM as well.
- signature: `class OpenAIClient(BaseLM):`
- members:
  - `acompletion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L120`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L120) — documented in [rlm-clients-openai](../../../concepts/rlm-clients-openai.md)
  - `completion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L94`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L94)
  - `get_last_usage(self)` — [`L197`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L197)
  - `get_usage_summary(self)` — [`L185`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L185) — documented in [rlm-clients-openai](../../../concepts/rlm-clients-openai.md)
  - `async_client` — [`L83`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L83)
  - `base_url` — [`L85`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L85)
  - `client` — [`L82`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L82)
  - `last_completion_tokens` — [`L161`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L161)
  - `last_cost` — [`L165`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L165)
  - `last_prompt_tokens` — [`L160`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L160)
  - `model_call_counts` — [`L88`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L88)
  - `model_costs` — [`L92`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L92)
  - `model_input_tokens` — [`L89`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L89)
  - `model_name` — [`L84`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L84)
  - `model_output_tokens` — [`L90`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L90)
  - `model_total_tokens` — [`L91`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L91)
- protocol/private: `__init__`[`L54`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L54), `_track_cost`[`L148`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L148)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`BaseLM`](base_lm.md#BaseLM), [`model_usage_summaries`](../core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](base_lm.md#BaseLM.__init__), [`timeout`](base_lm.md#BaseLM.timeout), [`total_cost`](../core/types.md#ModelUsageSummary.total_cost), [`sampling_args`](base_lm.md#BaseLM.sampling_args), [`DEFAULT_PRIME_INTELLECT_BASE_URL`](openai.md#DEFAULT_PRIME_INTELLECT_BASE_URL), [`_merge_extra_body`](openai.md#_merge_extra_body), [`_normalize_sampling_args`](openai.md#_normalize_sampling_args), [`DEFAULT_OPENAI_API_KEY`](openai.md#DEFAULT_OPENAI_API_KEY), [`DEFAULT_OPENROUTER_API_KEY`](openai.md#DEFAULT_OPENROUTER_API_KEY), [`DEFAULT_PRIME_API_KEY`](openai.md#DEFAULT_PRIME_API_KEY), [`DEFAULT_VERCEL_API_KEY`](openai.md#DEFAULT_VERCEL_API_KEY), [`kwargs`](base_lm.md#BaseLM.kwargs)
- used by: [`BaseLM`](base_lm.md#BaseLM), [`get_last_usage`](base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](base_lm.md#BaseLM.get_usage_summary), [`completion`](base_lm.md#BaseLM.completion), [`get_client`](__init__.md#get_client), [`acompletion`](base_lm.md#BaseLM.acompletion)  (6 test-only)

## Functions
- `_merge_extra_body(hardcoded: dict[str, Any], sampling_args: dict[str, Any] | None)` — [`L34`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L34) — Merge an ``extra_body`` from sampling_args into the hardcoded extra_body.
- `_normalize_sampling_args(sampling_args: dict[str, Any])` — [`L21`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L21) — Match the rename done by verifiers' OpenAIChatCompletionsClient so the

## Module values
- `DEFAULT_OPENAI_API_KEY` — [`L14`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L14)
- `DEFAULT_OPENROUTER_API_KEY` — [`L15`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L15)
- `DEFAULT_PRIME_API_KEY` — [`L17`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L17)
- `DEFAULT_PRIME_INTELLECT_BASE_URL` — [`L18`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L18)
- `DEFAULT_VERCEL_API_KEY` — [`L16`](../../../../../../raw/code/rlm/rlm/clients/openai.py#L16)

