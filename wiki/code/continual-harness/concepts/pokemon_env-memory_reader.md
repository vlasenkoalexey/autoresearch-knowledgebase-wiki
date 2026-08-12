---
title: PokemonEmeraldReader — reading game state from raw memory
type: concept
provenance: mixed
concept: pokemon_env-memory_reader
updated: 2026-08-12
status: fresh
---
# PokemonEmeraldReader — reading game state from raw memory

## Overview

`PokemonEmeraldReader` is how the agent perceives the game: [`get_comprehensive_state`](../catalog/pokemon_env/memory_reader.md#PokemonEmeraldReader.get_comprehensive_state) —
*"Get comprehensive game state with optional screenshot for OCR fallback"* — assembles location, party,
inventory, dialog, and battle info by reading raw emulator memory through address-offset accessors like
[`_read_u8`](../catalog/pokemon_env/memory_reader.md#PokemonEmeraldReader._read_u8), rather than any
higher-level game API. `addresses: MemoryAddresses` holds the offset table this all resolves against.

## Why it matters
This is the ground-truth observation layer every higher piece of the agent (objectives, subagents, the
Refiner's trajectory analysis) ultimately reads from — none of it is synthesized from screen pixels alone;
OCR is explicitly a *fallback*, not the primary channel.

## See also
- [`pokemon_env-emulator`](pokemon_env-emulator.md) — the emulator this reader attaches to.
