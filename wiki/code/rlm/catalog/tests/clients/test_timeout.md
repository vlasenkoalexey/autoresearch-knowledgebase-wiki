---
title: 'Module: tests/clients/test_timeout.py'
type: catalog
provenance: extracted
module: tests/clients/test_timeout.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.clients.test_timeout`/Test
symbols:
  TestDefaultTimeout.test_base_lm_stores_timeout: DefaultTimeout#test_base_lm_stores_timeout().
  TestDefaultTimeout.test_custom_timeout_override: DefaultTimeout#test_custom_timeout_override().
  TestOpenAIClientTimeout.test_timeout_raises_exception: OpenAIClientTimeout#test_timeout_raises_exception().
  TestDefaultTimeout.test_default_timeout_value: DefaultTimeout#test_default_timeout_value().
  TestOpenAIClientTimeout.test_timeout_passed_to_client: OpenAIClientTimeout#test_timeout_passed_to_client().
  TestAnthropicClientTimeout.test_timeout_passed_to_client: AnthropicClientTimeout#test_timeout_passed_to_client().
  TestAzureOpenAIClientTimeout.test_timeout_passed_to_client: AzureOpenAIClientTimeout#test_timeout_passed_to_client().
  TestPortkeyClientTimeout.test_timeout_passed_to_client: PortkeyClientTimeout#test_timeout_passed_to_client().
  TestGeminiClientTimeout.test_timeout_passed_to_client: GeminiClientTimeout#test_timeout_passed_to_client().
  TestDefaultTimeout: DefaultTimeout#
  TestOpenAIClientTimeout: OpenAIClientTimeout#
  TestAnthropicClientTimeout: AnthropicClientTimeout#
  TestAzureOpenAIClientTimeout: AzureOpenAIClientTimeout#
  TestPortkeyClientTimeout: PortkeyClientTimeout#
  TestGeminiClientTimeout: GeminiClientTimeout#
---
# Module: [`tests/clients/test_timeout.py`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py)

## Classes
### `TestAnthropicClientTimeout`
- def: [`tests/clients/test_timeout.py:76`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L76)
- doc: Tests for Anthropic client timeout.
- signature: `class TestAnthropicClientTimeout:`
- members:
  - `test_timeout_passed_to_client(self)` — [`L79`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L79) — Timeout should be passed to Anthropic client.
- uses (calls/refs, reference-scoped): [`AnthropicClient`](../../rlm/clients/anthropic.md#AnthropicClient)

### `TestAzureOpenAIClientTimeout`
- def: [`tests/clients/test_timeout.py:98`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L98)
- doc: Tests for Azure OpenAI client timeout.
- signature: `class TestAzureOpenAIClientTimeout:`
- members:
  - `test_timeout_passed_to_client(self)` — [`L101`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L101) — Timeout should be passed to Azure OpenAI client.
- uses (calls/refs, reference-scoped): [`AzureOpenAIClient`](../../rlm/clients/azure_openai.md#AzureOpenAIClient)

### `TestDefaultTimeout`
- def: [`tests/clients/test_timeout.py:11`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L11)
- doc: Tests for the default timeout constant.
- signature: `class TestDefaultTimeout:`
- members:
  - `test_base_lm_stores_timeout(self)` — [`L18`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L18) — BaseLM should store timeout in instance.
  - `test_custom_timeout_override(self)` — [`L27`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L27) — Custom timeout should override default.
  - `test_default_timeout_value(self)` — [`L14`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L14) — Default timeout should be 300 seconds.
- uses (calls/refs, reference-scoped): [`OpenAIClient`](../../rlm/clients/openai.md#OpenAIClient), [`timeout`](../../rlm/clients/base_lm.md#BaseLM.timeout), [`DEFAULT_TIMEOUT`](../../rlm/clients/base_lm.md#DEFAULT_TIMEOUT.DEFAULT_TIMEOUT)

### `TestGeminiClientTimeout`
- def: [`tests/clients/test_timeout.py:143`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L143)
- doc: Tests for Gemini client timeout.
- signature: `class TestGeminiClientTimeout:`
- members:
  - `test_timeout_passed_to_client(self)` — [`L146`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L146) — Timeout should be passed to Gemini client via http_options.
- uses (calls/refs, reference-scoped): [`GeminiClient`](../../rlm/clients/gemini.md#GeminiClient)

### `TestOpenAIClientTimeout`
- def: [`tests/clients/test_timeout.py:37`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L37)
- doc: Tests for OpenAI client timeout.
- signature: `class TestOpenAIClientTimeout:`
- members:
  - `test_timeout_passed_to_client(self)` — [`L40`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L40) — Timeout should be passed to OpenAI client.
  - `test_timeout_raises_exception(self)` — [`L58`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L58) — Timeout should raise appropriate exception.
- uses (calls/refs, reference-scoped): [`OpenAIClient`](../../rlm/clients/openai.md#OpenAIClient), [`completion`](../../rlm/clients/openai.md#OpenAIClient.completion)

### `TestPortkeyClientTimeout`
- def: [`tests/clients/test_timeout.py:123`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L123)
- doc: Tests for Portkey client timeout.
- signature: `class TestPortkeyClientTimeout:`
- members:
  - `test_timeout_passed_to_client(self)` — [`L126`](../../../../../../raw/code/rlm/tests/clients/test_timeout.py#L126) — Timeout should be passed to Portkey client.
- uses (calls/refs, reference-scoped): [`PortkeyClient`](../../rlm/clients/portkey.md#PortkeyClient)

