---
title: PortkeyClient
type: concept
provenance: mixed
concept: rlm-clients-portkey
updated: 2026-08-12
status: fresh
---
# PortkeyClient

## Overview

[`PortkeyClient`](../catalog/rlm/clients/portkey.md#PortkeyClient) routes through the Portkey API gateway —
a proxy that itself fronts multiple model providers — rather than talking to a single vendor directly. Its
[`_track_cost`](../catalog/rlm/clients/portkey.md#PortkeyClient._track_cost) reads a
`ChatCompletions` response object and updates the same per-model counters
([`OpenAIClient`](rlm-clients-openai.md), [`AnthropicClient`](rlm-clients-anthropic.md), and
[`GeminiClient`](rlm-clients-gemini.md) all shape this identically), so from
[`rlm-core-lm_handler`](rlm-core-lm_handler.md)'s point of view a Portkey-routed model is indistinguishable
from a direct vendor client — it's one more name registered against a `BaseLM`.

## See also
- [`rlm-clients-base_lm`](rlm-clients-base_lm.md) — the shared contract.
- [`rlm-clients-openai`](rlm-clients-openai.md), [`rlm-clients-anthropic`](rlm-clients-anthropic.md),
  [`rlm-clients-gemini`](rlm-clients-gemini.md) — sibling implementations.
