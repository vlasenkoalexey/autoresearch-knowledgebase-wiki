---
title: Model — the provider-agnostic model descriptor
type: concept
provenance: mixed
concept: packages-ai-src-types.ts
updated: 2026-08-12
status: fresh
---
# Model — the provider-agnostic model descriptor

## Overview

[`Model`](../catalog/packages/ai/src/types.ts.md#Model) is `packages/ai`'s uniform descriptor for any
backing LLM — [`id`](../catalog/packages/ai/src/types.ts.md#Model.id),
[`provider`](../catalog/packages/ai/src/types.ts.md#Model.provider),
[`baseUrl`](../catalog/packages/ai/src/types.ts.md#Model.baseUrl), context window, cost, and capability
flags — the TypeScript analog of [rlm](../../rlm/overview.md)'s `BaseLM` client abstraction: one shape every
vendor (Bedrock, Azure OpenAI, Google Vertex, and others under `packages/ai/src/providers/`) is normalized
into, so the rest of the agent never branches on vendor identity.

## See also
- [`rlm-clients-base_lm`](../../rlm/concepts/rlm-clients-base_lm.md) — the closest structural analog in the
  Python reference implementation.
