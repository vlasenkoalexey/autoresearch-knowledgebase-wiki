---
title: OpenAIClient — the default backend, doubling as an OpenAI-compatible router
type: concept
provenance: mixed
concept: rlm-clients-openai
updated: 2026-08-12
status: fresh
---
# OpenAIClient — the default backend, doubling as an OpenAI-compatible router

## Overview

[`OpenAIClient`](../catalog/rlm/clients/openai.md#OpenAIClient) is the default [`BaseLM`](rlm-clients-base_lm.md)
implementation (`RLM.__init__`'s `backend: ClientBackend = "openai"`). Its own docstring notes it "works
with vLLM as well" — it is written against the OpenAI-compatible HTTP surface, not the OpenAI SDK's
vendor-specific features, which is what lets one client class also reach OpenRouter, Prime Intellect's
hosted inference, and Vercel's AI gateway.

## Design rationale

**One client class, several default API-key/base-URL pairs.** [`__init__`](../catalog/rlm/clients/openai.md#OpenAIClient.__init__)
recognizes distinct default constants — `DEFAULT_OPENAI_API_KEY`, `DEFAULT_OPENROUTER_API_KEY`,
`DEFAULT_PRIME_API_KEY`/`DEFAULT_PRIME_INTELLECT_BASE_URL`, `DEFAULT_VERCEL_API_KEY` — rather than one
hardcoded provider, so switching backends is a constructor-argument change, not a different client class.
This is the same "the interface doesn't change, the endpoint does" pattern
[`rlm-environments-base_env`](rlm-environments-base_env.md) uses for sandboxes, applied here to model
providers.

## Entry points
- [`OpenAIClient.acompletion`](../catalog/rlm/clients/openai.md#OpenAIClient.acompletion) — the async
  completion path, used by [`rlm-core-lm_handler`](rlm-core-lm_handler.md)'s batched-request handler for
  concurrent sub-calls.
- [`OpenAIClient.get_usage_summary`](../catalog/rlm/clients/openai.md#OpenAIClient.get_usage_summary) —
  aggregates per-model call counts, costs, and token totals into a `UsageSummary`.

## See also
- [`rlm-clients-base_lm`](rlm-clients-base_lm.md) — the contract this implements.
- [`rlm-clients-anthropic`](rlm-clients-anthropic.md), [`rlm-clients-gemini`](rlm-clients-gemini.md),
  [`rlm-clients-portkey`](rlm-clients-portkey.md) — sibling implementations.
