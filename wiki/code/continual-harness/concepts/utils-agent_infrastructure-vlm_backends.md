---
title: VLM backends — the model-call layer every loop shares
type: concept
provenance: mixed
concept: utils-agent_infrastructure-vlm_backends
updated: 2026-08-12
status: fresh
---
# VLM backends — the model-call layer every loop shares

## Overview

`OpenRouterBackend.get_query`/`get_text_query` — *"Process image(s) and text. Returns adapter if tools,
else string"* / *"Process text-only prompt. Returns adapter if tools, else string"* — is the actual model
call underneath [`agents-PokeAgent`](agents-PokeAgent.md)'s planner/battler loops and
[`HarnessEvolver`](agents-utils-harness_evolver.md)'s VLM-analysis passes alike; every call routes through
`log_llm_interaction`/`log_llm_error` into the shared logger.

## See also
- [`utils-data_persistence-llm_logger`](utils-data_persistence-llm_logger.md) — where every call here is recorded.
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — a caller of this backend for evolution analysis.
