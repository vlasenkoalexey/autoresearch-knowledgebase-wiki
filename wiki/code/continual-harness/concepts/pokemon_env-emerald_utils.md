---
title: emerald_utils — raw-memory-to-Pokemon-object parsing
type: concept
provenance: mixed
concept: pokemon_env-emerald_utils
updated: 2026-08-12
status: fresh
---
# emerald_utils — raw-memory-to-Pokemon-object parsing

## Overview

[`parse_pokemon`](../catalog/pokemon_env/emerald_utils.md#parse_pokemon) turns raw save-block bytes into a
structured `PokemonData` (species, level, HP, moves, status, types) — the decode step
[`pokemon_env-memory_reader`](pokemon_env-memory_reader.md)'s battle/party reads depend on.

## See also
- [`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) — the caller.
- [`pokemon_env-enums`](pokemon_env-enums.md) — `PokemonType`, used to decode parsed types.
