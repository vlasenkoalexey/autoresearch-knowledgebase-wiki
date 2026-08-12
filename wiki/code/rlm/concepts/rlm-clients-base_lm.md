---
title: BaseLM — the model-agnostic client contract
type: concept
provenance: mixed
concept: rlm-clients-base_lm
updated: 2026-08-12
status: fresh
---
# BaseLM — the model-agnostic client contract

## Overview

[`BaseLM`](../catalog/rlm/clients/base_lm.md#BaseLM) is the abstract interface every vendor client
implements — [`AnthropicClient`](rlm-clients-anthropic.md), [`OpenAIClient`](rlm-clients-openai.md),
[`GeminiClient`](rlm-clients-gemini.md), [`PortkeyClient`](rlm-clients-portkey.md), plus an
`AzureOpenAIClient` and test doubles (`EchoLM`, `MockLM`) not otherwise covered in this batch. Its own
docstring states the reason it exists plainly: sub-calls are handled "in a model-agnostic way," so
[`LMHandler`](rlm-core-lm_handler.md) and [`RLM._subcall`](rlm-core-rlm.md) never need vendor-specific
branches — they hold a `BaseLM` reference and call three methods.

## Design rationale

**Three abstract methods, and cost tracking is one of them.** `completion`, `get_last_usage`, and
`get_usage_summary` are all abstract — meaning every client, regardless of vendor, is *required* to report
its own [`ModelUsageSummary`](../catalog/rlm/core/types.md#ModelUsageSummary), not just answer prompts. This
is what makes [`UsageSummary`](rlm-core-types.md)'s per-model cost breakdown possible across an arbitrary
mix of vendors in one recursive tree — the contract enforces that every client can answer "what did the last
call cost."

## Entry points
- [`BaseLM.completion`](../catalog/rlm/clients/base_lm.md#BaseLM.completion) — called from
  [`RLM._subcall`](rlm-core-rlm.md) via [`get_client`](rlm-core-rlm.md).
- [`BaseLM.get_last_usage`](../catalog/rlm/clients/base_lm.md#BaseLM.get_last_usage) — called immediately
  after a completion to attribute cost to that specific call.

## See also
- [`rlm-clients-anthropic`](rlm-clients-anthropic.md), [`rlm-clients-openai`](rlm-clients-openai.md),
  [`rlm-clients-gemini`](rlm-clients-gemini.md), [`rlm-clients-portkey`](rlm-clients-portkey.md) — the
  concrete implementations.
- [`rlm-core-lm_handler`](rlm-core-lm_handler.md) — the caller that resolves a `BaseLM` by model name.
