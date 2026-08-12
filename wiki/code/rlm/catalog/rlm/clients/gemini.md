---
title: 'Module: rlm/clients/gemini.py'
type: catalog
provenance: extracted
module: rlm/clients/gemini.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.gemini`/
symbols:
  GeminiClient.get_usage_summary: GeminiClient#get_usage_summary().
  GeminiClient: GeminiClient#
  GeminiClient._track_cost: GeminiClient#_track_cost().
  GeminiClient.get_last_usage: GeminiClient#get_last_usage().
  GeminiClient.completion: GeminiClient#completion().
  GeminiClient.acompletion: GeminiClient#acompletion().
  GeminiClient.__init__: GeminiClient#__init__().
  GeminiClient._prepare_contents: GeminiClient#_prepare_contents().
  GeminiClient.model_call_counts: GeminiClient#model_call_counts.
  GeminiClient.last_prompt_tokens: GeminiClient#last_prompt_tokens.
  GeminiClient.last_completion_tokens: GeminiClient#last_completion_tokens.
  GeminiClient.model_name: GeminiClient#model_name.
  GeminiClient.model_input_tokens: GeminiClient#model_input_tokens.
  GeminiClient.model_output_tokens: GeminiClient#model_output_tokens.
  GeminiClient.client: GeminiClient#client.
  DEFAULT_GEMINI_API_KEY: DEFAULT_GEMINI_API_KEY.
  GeminiClient.model_total_tokens: GeminiClient#model_total_tokens.
---
# Module: [`rlm/clients/gemini.py`](../../../../../../raw/code/rlm/rlm/clients/gemini.py)

## Classes
### `GeminiClient`  ·  implements/extends BaseLM
- def: [`rlm/clients/gemini.py:17`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L17) — documented in [rlm-clients-gemini](../../../concepts/rlm-clients-gemini.md)
- doc: LM Client for running models with the Google Gemini API.
- signature: `class GeminiClient(BaseLM):`
- members:
  - `_prepare_contents(self, prompt: str | list[dict[str, Any]])` — [`L97`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L97) — Prepare contents and extract system instruction for Gemini API.
  - `acompletion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L74`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L74)
  - `completion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L54`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L54)
  - `get_last_usage(self)` — [`L159`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L159)
  - `get_usage_summary(self)` — [`L149`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L149)
  - `client` — [`L41`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L41)
  - `last_completion_tokens` — [`L52`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L52)
  - `last_prompt_tokens` — [`L51`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L51)
  - `model_call_counts` — [`L45`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L45)
  - `model_input_tokens` — [`L46`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L46)
  - `model_name` — [`L42`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L42)
  - `model_output_tokens` — [`L47`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L47)
  - `model_total_tokens` — [`L48`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L48)
- protocol/private: `__init__`[`L23`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L23), `_track_cost`[`L129`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L129)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`BaseLM`](base_lm.md#BaseLM), [`model_usage_summaries`](../core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](base_lm.md#BaseLM.__init__), [`timeout`](base_lm.md#BaseLM.timeout), [`DEFAULT_GEMINI_API_KEY`](gemini.md#DEFAULT_GEMINI_API_KEY)
- used by: [`BaseLM`](base_lm.md#BaseLM), [`get_last_usage`](base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](base_lm.md#BaseLM.get_usage_summary), [`completion`](base_lm.md#BaseLM.completion), [`get_client`](__init__.md#get_client), [`acompletion`](base_lm.md#BaseLM.acompletion)  (16 test-only)

## Module values
- `DEFAULT_GEMINI_API_KEY` — [`L14`](../../../../../../raw/code/rlm/rlm/clients/gemini.py#L14)

