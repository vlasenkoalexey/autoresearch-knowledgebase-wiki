---
title: LLMLogger — the global model-call ledger
type: concept
provenance: mixed
concept: utils-data_persistence-llm_logger
updated: 2026-08-12
status: fresh
---
# LLMLogger — the global model-call ledger

## Overview

[`LLMLogger`](../catalog/utils/data_persistence/llm_logger.md#LLMLogger) — *"Logger for all LLM
interactions"* — is a single global instance ([`get_llm_logger`](../catalog/utils/data_persistence/llm_logger.md#get_llm_logger),
*"Get the global LLM logger instance"*) accumulating [`cumulative_metrics`](../catalog/utils/data_persistence/llm_logger.md#LLMLogger.cumulative_metrics)
across every call any [`utils-agent_infrastructure-vlm_backends`](utils-agent_infrastructure-vlm_backends.md)
backend makes — the single point every model interaction in the process passes through, regardless of which
loop or evolution pass triggered it.

## See also
- [`utils-agent_infrastructure-vlm_backends`](utils-agent_infrastructure-vlm_backends.md) — the caller.
