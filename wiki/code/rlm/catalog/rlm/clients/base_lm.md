---
title: 'Module: rlm/clients/base_lm.py'
type: catalog
provenance: extracted
module: rlm/clients/base_lm.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.clients.base_lm`/
symbols:
  BaseLM: BaseLM#
  BaseLM.get_usage_summary: BaseLM#get_usage_summary().
  BaseLM.get_last_usage: BaseLM#get_last_usage().
  BaseLM.completion: BaseLM#completion().
  BaseLM.acompletion: BaseLM#acompletion().
  BaseLM.__init__: BaseLM#__init__().
  BaseLM.timeout: BaseLM#timeout.
  BaseLM.model_name: BaseLM#model_name.
  BaseLM.sampling_args: BaseLM#sampling_args.
  DEFAULT_TIMEOUT.DEFAULT_TIMEOUT: DEFAULT_TIMEOUT.DEFAULT_TIMEOUT.
  BaseLM.kwargs: BaseLM#kwargs.
---
# Module: [`rlm/clients/base_lm.py`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py)

## Classes
### `BaseLM`  ·  implements/extends ABC
- def: [`rlm/clients/base_lm.py:10`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L10) — documented in [rlm-clients-base_lm](../../../concepts/rlm-clients-base_lm.md)
- doc: Base class for all language model routers / clients. When the RLM makes sub-calls, it currently
- signature: `class BaseLM(ABC):`
- members:
  - `acompletion(self, prompt: str | dict[str, Any])` — [`L36`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L36)
  - `completion(self, prompt: str | dict[str, Any])` — [`L32`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L32) — documented in [rlm-clients-base_lm](../../../concepts/rlm-clients-base_lm.md)
  - `get_last_usage(self)` — [`L45`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L45) — Get the last cost summary of the model. — documented in [rlm-clients-base_lm](../../../concepts/rlm-clients-base_lm.md)
  - `get_usage_summary(self)` — [`L40`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L40) — Get cost summary for all model calls.
  - `kwargs` — [`L29`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L29)
  - `model_name` — [`L23`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L23)
  - `sampling_args` — [`L28`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L28)
  - `timeout` — [`L24`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L24)
- protocol/private: `__init__`[`L16`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L16)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../core/types.md#UsageSummary), [`ModelUsageSummary`](../core/types.md#ModelUsageSummary), [`get_usage_summary`](openai.md#OpenAIClient.get_usage_summary), [`get_usage_summary`](gemini.md#GeminiClient.get_usage_summary), [`GeminiClient`](gemini.md#GeminiClient), [`OpenAIClient`](openai.md#OpenAIClient), [`get_usage_summary`](anthropic.md#AnthropicClient.get_usage_summary), [`get_usage_summary`](azure_openai.md#AzureOpenAIClient.get_usage_summary), [`get_usage_summary`](portkey.md#PortkeyClient.get_usage_summary), [`acompletion`](openai.md#OpenAIClient.acompletion), [`completion`](openai.md#OpenAIClient.completion), [`get_last_usage`](openai.md#OpenAIClient.get_last_usage), [`PortkeyClient`](portkey.md#PortkeyClient), [`get_last_usage`](gemini.md#GeminiClient.get_last_usage), [`get_last_usage`](anthropic.md#AnthropicClient.get_last_usage), [`get_last_usage`](azure_openai.md#AzureOpenAIClient.get_last_usage), [`get_last_usage`](portkey.md#PortkeyClient.get_last_usage), [`completion`](gemini.md#GeminiClient.completion), [`acompletion`](anthropic.md#AnthropicClient.acompletion), [`completion`](anthropic.md#AnthropicClient.completion), [`acompletion`](gemini.md#GeminiClient.acompletion), [`AnthropicClient`](anthropic.md#AnthropicClient), [`completion`](portkey.md#PortkeyClient.completion), [`acompletion`](azure_openai.md#AzureOpenAIClient.acompletion), [`acompletion`](portkey.md#PortkeyClient.acompletion), [`completion`](azure_openai.md#AzureOpenAIClient.completion), [`AzureOpenAIClient`](azure_openai.md#AzureOpenAIClient), [`DEFAULT_TIMEOUT`](base_lm.md#DEFAULT_TIMEOUT.DEFAULT_TIMEOUT)  (25 test-only)
- used by: [`_subcall`](../core/rlm.md#RLM._subcall), [`_spawn_completion_context`](../core/rlm.md#RLM._spawn_completion_context), [`_handle_batched`](../core/lm_handler.md#LMRequestHandler._handle_batched), [`_handle_single`](../core/lm_handler.md#LMRequestHandler._handle_single), [`get_client`](__init__.md#get_client), [`GeminiClient`](gemini.md#GeminiClient), [`OpenAIClient`](openai.md#OpenAIClient), [`__init__`](openai.md#OpenAIClient.__init__), [`acompletion`](openai.md#OpenAIClient.acompletion), [`get_usage_summary`](../core/lm_handler.md#LMHandler.get_usage_summary), [`completion`](openai.md#OpenAIClient.completion), [`PortkeyClient`](portkey.md#PortkeyClient), [`_fallback_answer`](../core/rlm.md#RLM._fallback_answer), [`get_client`](../core/lm_handler.md#LMHandler.get_client), [`AnthropicClient`](anthropic.md#AnthropicClient), [`completion`](../core/lm_handler.md#LMHandler.completion), [`register_client`](../core/lm_handler.md#LMHandler.register_client), [`__init__`](gemini.md#GeminiClient.__init__), [`AzureOpenAIClient`](azure_openai.md#AzureOpenAIClient), [`clients`](../core/lm_handler.md#LMHandler.clients), [`batch_max_concurrent`](../core/lm_handler.md#LMHandler.batch_max_concurrent), [`__init__`](azure_openai.md#AzureOpenAIClient.__init__), [`async_client`](anthropic.md#AnthropicClient.async_client), [`async_client`](azure_openai.md#AzureOpenAIClient.async_client), [`async_client`](portkey.md#PortkeyClient.async_client), [`client`](anthropic.md#AnthropicClient.client), [`client`](azure_openai.md#AzureOpenAIClient.client), [`client`](portkey.md#PortkeyClient.client), [`run_one`](../core/lm_handler.md#LMRequestHandler.run_one), [`__init__`](anthropic.md#AnthropicClient.__init__), [`__init__`](portkey.md#PortkeyClient.__init__), [`__init__`](../core/lm_handler.md#LMHandler.__init__)  (15 test-only)

## Module values
- `DEFAULT_TIMEOUT` — [`L7`](../../../../../../raw/code/rlm/rlm/clients/base_lm.py#L7)

