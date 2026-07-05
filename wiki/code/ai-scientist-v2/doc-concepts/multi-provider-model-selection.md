---
title: Multi-provider model selection & per-stage model flags
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Multi-provider model selection & per-stage model flags

## Definition
AI Scientist-v2 is provider-agnostic and lets the operator assign *different* models to *different
pipeline stages*. The README documents three backends — OpenAI (via `OPENAI_API_KEY`), Gemini (routed
through the OpenAI-compatible API using `GEMINI_API_KEY`), and Claude via AWS Bedrock (`pip install
anthropic[bedrock]` plus `AWS_ACCESS_KEY_ID` / `AWS_SECRET_ACCESS_KEY` / `AWS_REGION_NAME`). Model choice
is per phase: ideation takes `--model`, and the experiment launcher takes `--model_writeup`,
`--model_citation`, `--model_review`, and `--model_agg_plots`, while the experimentation phase itself is
configured in `bfts_config.yaml` (default `claude-3-5-sonnet`).

## In ai-scientist-v2 (grounded)
All provider dispatch is centralized in
[`ai_scientist/llm.py`](../catalog/ai_scientist/llm.md). The `--model` strings the README passes must be
members of [`AVAILABLE_LLMS`](../catalog/ai_scientist/llm.md#AVAILABLE_LLMS); a model name is turned into a
concrete provider client by [`create_client`](../catalog/ai_scientist/llm.md#create_client), which is where
the OpenAI / Gemini-over-OpenAI-API / Claude-over-Bedrock branching lives. Once a client exists, all stages
call the same façade —
[`get_response_from_llm`](../catalog/ai_scientist/llm.md#get_response_from_llm) (and the batched
[`get_batch_responses_from_llm`](../catalog/ai_scientist/llm.md#get_batch_responses_from_llm)), which in
turn dispatch to [`make_llm_call`](../catalog/ai_scientist/llm.md#make_llm_call); token budgeting is bounded
by [`MAX_NUM_TOKENS`](../catalog/ai_scientist/llm.md#MAX_NUM_TOKENS). On the entry side, the ideation
model string is bound to
[`client_model`](../catalog/ai_scientist/perform_ideation_temp_free.md#client_model) in
[`ai_scientist/perform_ideation_temp_free.py`](../catalog/ai_scientist/perform_ideation_temp_free.md), and
the four `--model_*` experiment flags are declared in
[`parse_arguments`](../catalog/launch_scientist_bfts.md#parse_arguments) in
[`launch_scientist_bfts.py`](../catalog/launch_scientist_bfts.md).

The per-stage YAML model field (e.g. the experimentation model, the writeup/aggregation stages) is carried
on `StageConfig` — the config catalog exposes fields such as `StageConfig.model` — but the exact
CLI-flag-to-field wiring for `--model_writeup`/`--model_citation`/`--model_review`/`--model_agg_plots` is
resolved inside the launcher rather than a single named symbol; treat the flags as launcher arguments that
select which model each downstream stage instantiates via `create_client`.

## Why it matters / when it applies
Per-stage model selection is a direct cost/quality lever: the README recommends powerful models
(Claude 3.5 Sonnet) for the expensive experimentation phase but cheaper models (e.g. GPT-4o for
`model_citation`) for writeup-adjacent stages to cut cost. It also means an operator can mix providers in a
single run — e.g. a Claude experimentation model via Bedrock with OpenAI writeup/review models — as long as
the corresponding API keys are set. Provider setup (keys, Bedrock packages, region) is the precondition; the
flags are the routing.

## Connections
- Code concepts: [ai_scientist-llm](../concepts/ai_scientist-llm.md) — the LLM client/dispatch layer.
- Module catalogs: [ai_scientist/llm](../catalog/ai_scientist/llm.md),
  [ai_scientist/perform_ideation_temp_free](../catalog/ai_scientist/perform_ideation_temp_free.md),
  [launch_scientist_bfts](../catalog/launch_scientist_bfts.md).
- Related doc-concepts: [two-stage-operator-workflow](two-stage-operator-workflow.md),
  [bfts-tree-search-configuration](bfts-tree-search-configuration.md).

## Source
Extracted from `README.md` (kept in place).
