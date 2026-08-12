---
title: AnthropicClient
type: concept
provenance: mixed
concept: rlm-clients-anthropic
updated: 2026-08-12
status: fresh
---
# AnthropicClient

## Overview

`AnthropicClient` is the [`BaseLM`](rlm-clients-base_lm.md)
implementation over Anthropic's own SDK, structurally identical to [`OpenAIClient`](rlm-clients-openai.md)
and [`GeminiClient`](rlm-clients-gemini.md) at the interface level (`completion`, `acompletion`,
`get_last_usage`, `get_usage_summary`) but distinct in how a prompt is shaped: `_prepare_messages` handles
Anthropic's system/user message split before the call, and `max_tokens` is passed explicitly per call — a
required parameter on Anthropic's API, unlike OpenAI's.

## See also
- [`rlm-clients-base_lm`](rlm-clients-base_lm.md) — the shared contract.
- [`rlm-clients-openai`](rlm-clients-openai.md), [`rlm-clients-gemini`](rlm-clients-gemini.md) — sibling
  implementations.
