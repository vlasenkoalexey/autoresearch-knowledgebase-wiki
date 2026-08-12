---
title: RedMemoryReader — the Gen 1 memory reader, unified state shape
type: concept
provenance: mixed
concept: pokemon_red_env-red_memory_reader
updated: 2026-08-12
status: fresh
---
# RedMemoryReader — the Gen 1 memory reader, unified state shape

## Overview

`RedMemoryReader.get_comprehensive_state` — *"Return a state dict with the same four-key shape as
EmeraldEmulator"* — is deliberately shaped to match
[`pokemon_env-memory_reader`](pokemon_env-memory_reader.md)'s Emerald reader's output contract, so
downstream consumers ([`utils-state_formatter`](utils-state_formatter.md),
[`agents-PokeAgent`](agents-PokeAgent.md)) don't need to branch on which game generation is running.

## See also
- [`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) — the Emerald counterpart this matches.
