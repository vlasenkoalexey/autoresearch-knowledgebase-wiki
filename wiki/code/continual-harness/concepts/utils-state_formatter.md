---
title: format_state_for_llm — the text rendering the model actually reads
type: concept
provenance: mixed
concept: utils-state_formatter
updated: 2026-08-12
status: fresh
---
# format_state_for_llm — the text rendering the model actually reads

## Overview

[`format_state_for_llm`](../catalog/utils/state_formatter.md#format_state_for_llm) — *"Format comprehensive
state data into a readable context for the VLM"* — is the final translation step between raw memory-reader
output ([`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) /
[`pokemon_red_env-red_memory_reader`](pokemon_red_env-red_memory_reader.md)) and the text the model actually
sees each turn, optionally including debug info, NPCs, and a movement preview.

## See also
- [`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) — the data source.
