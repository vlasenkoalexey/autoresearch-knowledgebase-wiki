---
title: SubLLMProxy — the training-time HTTP LM proxy
type: concept
provenance: mixed
concept: training-src-rlm_train-proxy
updated: 2026-08-12
status: fresh
---
# SubLLMProxy — the training-time HTTP LM proxy

## Overview

`SubLLMProxy` is [`LMHandler`](rlm-core-lm_handler.md)'s training-time counterpart: an HTTP server (rather
than a raw socket server) that a training rollout's sandboxed [`Worker`](training-src-rlm_train-worker.md)
posts sub-LLM requests to, backed by `_handle_single`/`_handle_batched` handlers structurally identical in
shape to `LMRequestHandler`'s.

## Design rationale

**Concurrency is bounded per-model via semaphores**, the same mechanism
[`rlm-core-lm_handler`](rlm-core-lm_handler.md)'s batched handler uses at inference time — `_semaphores`
keyed by model, `max_concurrent` capping in-flight sub-calls. This is the training-time enforcement of the
same "don't let a rollout's fan-out overwhelm the backing model API" concern the inference stack solves with
`max_concurrent_subcalls`.

**`fake_query`/`fake_query_batched` on `state_ref` indicate the proxy can be run against a stub client** —
useful for offline testing or dry runs of the training environment without hitting a real model API, a
capability not present in the inference-time `LMHandler`.

## Entry points
- [`SubLLMProxy.start`](../catalog/training/src/rlm_train/proxy.md#SubLLMProxy.start) /
  [`stop`](../catalog/training/src/rlm_train/proxy.md#SubLLMProxy.stop) — lifecycle, mirroring
  `RLMTrainEnv.setup_state`'s lazy-start pattern.
- [`SubLLMProxy._completion`](../catalog/training/src/rlm_train/proxy.md#SubLLMProxy._completion) — the
  actual model call, resolving a `ClientHandle` and normalizing the prompt shape before dispatch.

## See also
- [`training-src-rlm_train-env`](training-src-rlm_train-env.md) — the caller that starts this proxy per rollout.
- [`rlm-core-lm_handler`](rlm-core-lm_handler.md) — the inference-time counterpart.
