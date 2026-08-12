---
title: GeminiClient
type: concept
provenance: mixed
concept: rlm-clients-gemini
updated: 2026-08-12
status: fresh
---
# GeminiClient

## Overview

[`GeminiClient`](../catalog/rlm/clients/gemini.md#GeminiClient) is the [`BaseLM`](rlm-clients-base_lm.md)
implementation over the Google Gemini API, following the same per-model cost-tracking shape as its siblings
([`_track_cost`](../catalog/rlm/clients/gemini.md#GeminiClient._track_cost) reads token counts off
`types.GenerateContentResponse` into `model_call_counts`/`model_input_tokens`/`model_output_tokens`, exactly
paralleling [`OpenAIClient`](rlm-clients-openai.md) and [`AnthropicClient`](rlm-clients-anthropic.md)'s own
`_track_cost` methods). The RLM paper's own experiments use GPT-5/GPT-5-mini and Qwen3 as root/sub-call
models (see [Recursive Language Models](../../../sources/recursive-language-models.md)); this client is the
Gemini-family counterpart in the implementation, not exercised in the paper's own headline results.

## See also
- [`rlm-clients-base_lm`](rlm-clients-base_lm.md) — the shared contract.
- [`rlm-clients-openai`](rlm-clients-openai.md), [`rlm-clients-anthropic`](rlm-clients-anthropic.md),
  [`rlm-clients-portkey`](rlm-clients-portkey.md) — sibling implementations.
