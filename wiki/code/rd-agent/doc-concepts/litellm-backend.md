---
title: LiteLLM multi-provider backend
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# LiteLLM multi-provider backend

## Definition
R&D-Agent talks to LLMs through **[LiteLLM](https://github.com/BerriAI/litellm)** as its default backend, giving one configuration surface for many providers — OpenAI, Azure OpenAI, DeepSeek, SiliconFlow-hosted embeddings, and any other LiteLLM-supported model. The README configures it purely through environment variables in a `.env` file: `CHAT_MODEL` and `EMBEDDING_MODEL` name the models (e.g. `gpt-4o`, `deepseek/deepseek-chat`, `litellm_proxy/BAAI/bge-m3`), with per-provider API base/key vars. The demos require three abilities from the configured models: ChatCompletion, json_mode, and embedding query.

## In rd-agent (grounded)
The `.env` keys bind to settings on [`LLMSettings`](../catalog/rdagent/oai/llm_conf.md#LLMSettings) (the [`LLM_SETTINGS`](../catalog/rdagent/oai/llm_conf.md#LLM_SETTINGS) singleton, module `rdagent/oai/llm_conf.py`): `CHAT_MODEL` → [`chat_model`](../catalog/rdagent/oai/llm_conf.md#LLMSettings.chat_model), `EMBEDDING_MODEL` → [`embedding_model`](../catalog/rdagent/oai/llm_conf.md#LLMSettings.embedding_model), plus caps and retries like [`chat_max_tokens`](../catalog/rdagent/oai/llm_conf.md#LLMSettings.chat_max_tokens) and [`max_retry`](../catalog/rdagent/oai/llm_conf.md#LLMSettings.max_retry); a per-role [`chat_model_map`](../catalog/rdagent/oai/llm_conf.md#LLMSettings.chat_model_map) enables the "o3(R)+GPT-4.1(D)" split the README's MLE-bench result relies on. Calls route through the [`APIBackend`](../catalog/rdagent/oai/backend/base.md#APIBackend) façade (module `rdagent/oai/backend/base.py`): [`build_messages_and_create_chat_completion`](../catalog/rdagent/oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion) for chat and [`create_embedding`](../catalog/rdagent/oai/backend/base.md#APIBackend.create_embedding) for embeddings, with SQLite-backed chat/embedding caches ([`use_chat_cache`](../catalog/rdagent/oai/backend/base.md#APIBackend.use_chat_cache), [`use_embedding_cache`](../catalog/rdagent/oai/backend/base.md#APIBackend.use_embedding_cache)) for reproducibility and cost control. The README's `REASONING_THINK_RM=True` toggle for `<think>`-tag models corresponds to the reasoning-model handling on the backend.

## Why it matters / when it applies
Provider-agnostic configuration is what lets the README quote a quant result "at a cost under $10" and mix a strong reasoning model for Research with a cheaper model for Development. Because chat and embedding models are configured independently, users pair, say, DeepSeek chat with a SiliconFlow embedding model (DeepSeek has no embedding model) — a case the README calls out explicitly. The `litellm_proxy/` prefix requirement for embeddings and the separate-API-base option are the two configuration gotchas the doc warns about.

## Connections
- Code concepts: [oai/backend/base (APIBackend)](../concepts/rdagent-oai-backend-base.md) — the request/cache/parse pipeline; [oai/llm_conf (LLMSettings)](../concepts/rdagent-oai-llm_conf.md) — the settings surface.
- Module catalogs: [oai/backend/base](../catalog/rdagent/oai/backend/base.md), [oai/llm_conf](../catalog/rdagent/oai/llm_conf.md).
- Related doc-concepts: [research-development-framework](research-development-framework.md), [rdagent-cli](rdagent-cli.md).

## Source
Extracted from `README.md` (kept in place).
