---
title: 'Module: rlm/clients/anthropic.py'
type: catalog
provenance: extracted
module: rlm/clients/anthropic.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.anthropic`/AnthropicClient#
symbols:
  AnthropicClient.get_usage_summary: get_usage_summary().
  AnthropicClient.get_last_usage: get_last_usage().
  AnthropicClient.completion: completion().
  AnthropicClient.acompletion: acompletion().
  AnthropicClient._track_cost: _track_cost().
  AnthropicClient: ''
  AnthropicClient.client: client.
  AnthropicClient.async_client: async_client.
  AnthropicClient.model_call_counts: model_call_counts.
  AnthropicClient.__init__: __init__().
  AnthropicClient.model_name: model_name.
  AnthropicClient.max_tokens: max_tokens.
  AnthropicClient.model_input_tokens: model_input_tokens.
  AnthropicClient.model_output_tokens: model_output_tokens.
  AnthropicClient._prepare_messages: _prepare_messages().
  AnthropicClient.model_total_tokens: model_total_tokens.
  AnthropicClient.last_prompt_tokens: last_prompt_tokens.
  AnthropicClient.last_completion_tokens: last_completion_tokens.
---
# Module: [`rlm/clients/anthropic.py`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py)

## Classes
### `AnthropicClient`  ·  implements/extends BaseLM
- def: [`rlm/clients/anthropic.py:10`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L10)
- doc: LM Client for running models with the Anthropic API.
- signature: `class AnthropicClient(BaseLM):`
- members:
  - `_prepare_messages(self, prompt: str | list[dict[str, Any]])` — [`L66`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L66) — Prepare messages and extract system prompt for Anthropic API.
  - `acompletion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L49`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L49)
  - `completion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L34`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L34)
  - `get_last_usage(self)` — [`L107`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L107)
  - `get_usage_summary(self)` — [`L97`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L97)
  - `async_client` — [`L24`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L24)
  - `client` — [`L23`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L23)
  - `last_completion_tokens` — [`L95`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L95)
  - `last_prompt_tokens` — [`L94`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L94)
  - `max_tokens` — [`L26`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L26)
  - `model_call_counts` — [`L29`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L29)
  - `model_input_tokens` — [`L30`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L30)
  - `model_name` — [`L25`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L25)
  - `model_output_tokens` — [`L31`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L31)
  - `model_total_tokens` — [`L32`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L32)
- protocol/private: `__init__`[`L15`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L15), `_track_cost`[`L87`](../../../../../../raw/code/rlm/rlm/clients/anthropic.py#L87)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`BaseLM`](base_lm.md#BaseLM), [`model_usage_summaries`](../core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](base_lm.md#BaseLM.__init__), [`timeout`](base_lm.md#BaseLM.timeout)
- used by: [`BaseLM`](base_lm.md#BaseLM), [`get_last_usage`](base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](base_lm.md#BaseLM.get_usage_summary), [`completion`](base_lm.md#BaseLM.completion), [`get_client`](__init__.md#get_client), [`acompletion`](base_lm.md#BaseLM.acompletion)  (3 test-only)

