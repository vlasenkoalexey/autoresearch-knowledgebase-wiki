---
title: 'Module: rlm/clients/portkey.py'
type: catalog
provenance: extracted
module: rlm/clients/portkey.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.portkey`/PortkeyClient#
symbols:
  PortkeyClient.get_usage_summary: get_usage_summary().
  PortkeyClient: ''
  PortkeyClient.get_last_usage: get_last_usage().
  PortkeyClient._track_cost: _track_cost().
  PortkeyClient.completion: completion().
  PortkeyClient.acompletion: acompletion().
  PortkeyClient.client: client.
  PortkeyClient.async_client: async_client.
  PortkeyClient.model_call_counts: model_call_counts.
  PortkeyClient.__init__: __init__().
  PortkeyClient.model_name: model_name.
  PortkeyClient.model_input_tokens: model_input_tokens.
  PortkeyClient.model_output_tokens: model_output_tokens.
  PortkeyClient.model_total_tokens: model_total_tokens.
  PortkeyClient.last_prompt_tokens: last_prompt_tokens.
  PortkeyClient.last_completion_tokens: last_completion_tokens.
---
# Module: [`rlm/clients/portkey.py`](../../../../../../raw/code/rlm/rlm/clients/portkey.py)

## Classes
### `PortkeyClient`  ·  implements/extends BaseLM
- def: [`rlm/clients/portkey.py:11`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L11) — documented in [rlm-clients-portkey](../../../concepts/rlm-clients-portkey.md)
- doc: LM Client for running models with the Portkey API.
- signature: `class PortkeyClient(BaseLM):`
- members:
  - `acompletion(self, prompt: str | dict[str, Any], model: str | None = None)` — [`L53`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L53)
  - `completion(self, prompt: str | list[dict[str, Any]], model: str | None = None)` — [`L34`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L34)
  - `get_last_usage(self)` — [`L89`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L89)
  - `get_usage_summary(self)` — [`L79`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L79)
  - `async_client` — [`L25`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L25)
  - `client` — [`L24`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L24)
  - `last_completion_tokens` — [`L77`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L77)
  - `last_prompt_tokens` — [`L76`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L76)
  - `model_call_counts` — [`L29`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L29)
  - `model_input_tokens` — [`L30`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L30)
  - `model_name` — [`L26`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L26)
  - `model_output_tokens` — [`L31`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L31)
  - `model_total_tokens` — [`L32`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L32)
- protocol/private: `__init__`[`L16`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L16), `_track_cost`[`L69`](../../../../../../raw/code/rlm/rlm/clients/portkey.py#L69)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`BaseLM`](base_lm.md#BaseLM), [`model_usage_summaries`](../core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../core/types.md#ModelUsageSummary.total_output_tokens), [`__init__`](base_lm.md#BaseLM.__init__), [`timeout`](base_lm.md#BaseLM.timeout)
- used by: [`BaseLM`](base_lm.md#BaseLM), [`get_last_usage`](base_lm.md#BaseLM.get_last_usage), [`get_usage_summary`](base_lm.md#BaseLM.get_usage_summary), [`completion`](base_lm.md#BaseLM.completion), [`get_client`](__init__.md#get_client), [`acompletion`](base_lm.md#BaseLM.acompletion)  (6 test-only)

