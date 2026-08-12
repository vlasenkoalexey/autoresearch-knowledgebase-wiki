---
title: RLMTrainEnv — the RL-training-time re-implementation of the RLM loop
type: concept
provenance: mixed
concept: training-src-rlm_train-env
updated: 2026-08-12
status: fresh
---
# RLMTrainEnv — the RL-training-time re-implementation of the RLM loop

## Overview

`training/` is a second, parallel implementation of the same core idea — this repo's own README describes
it as a `verifiers`-based training environment built on Prime Intellect's `prime-rl`, used to produce the
paper's [RLM-Qwen3-8B fine-tune](../../../sources/recursive-language-models.md). `RLMTrainEnv` plays the
role [`RLM`](rlm-core-rlm.md) plays at inference time, but reshaped around the `verifiers` framework's
`State`-passing contract (`setup_state`, `get_prompt_messages`) rather than a synchronous `completion()`
call — so that a training rollout can be scored and used for RL updates.

## Design rationale

**The inference-time and training-time stacks solve the same problem with parallel-but-distinct
machinery**, not a shared code path — `RLMTrainEnv._ensure_proxy` lazily starts a
[`SubLLMProxy`](training-src-rlm_train-proxy.md) exactly the way `RLM._spawn_completion_context` lazily
starts an [`LMHandler`](rlm-core-lm_handler.md), and `get_prompt_messages` re-derives the same system-prompt
construction ([`build_rlm_system_prompt`](../catalog/rlm/utils/prompts.md#build_rlm_system_prompt)) the
inference path uses — the training environment is a re-derivation of the inference contract, built to fit
`verifiers`' async, state-object-passing execution model rather than reusing `RLM` directly.

## Entry points
- [`RLMTrainEnv.setup_state`](../catalog/training/src/rlm_train/env.md#RLMTrainEnv.setup_state) — the
  `verifiers`-framework hook that initializes one rollout's state, starting the sub-LLM proxy and building
  the initial system prompt.
- [`RLMTrainEnv.get_prompt_messages`](../catalog/training/src/rlm_train/env.md#RLMTrainEnv.get_prompt_messages) —
  produces the next turn's messages, formatting the prior turn's REPL output back into context via
  [`_pack_exec`](../catalog/training/src/rlm_train/env.md#_pack_exec) — the training-loop analog of
  [`format_iteration`](rlm-core-rlm.md) bounding a code result before it re-enters history.

## See also
- [`training-src-rlm_train-proxy`](training-src-rlm_train-proxy.md) — the sub-LLM proxy this environment starts.
- [`training-src-rlm_train-worker`](training-src-rlm_train-worker.md) — the sandboxed execution side.
- [`rlm-core-rlm`](rlm-core-rlm.md) — the inference-time counterpart this re-derives.
