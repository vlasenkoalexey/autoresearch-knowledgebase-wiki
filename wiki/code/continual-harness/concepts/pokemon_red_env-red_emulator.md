---
title: RedEmulator — the Pokémon Red/Blue counterpart emulator
type: concept
provenance: mixed
concept: pokemon_red_env-red_emulator
updated: 2026-08-12
status: fresh
---
# RedEmulator — the Pokémon Red/Blue counterpart emulator

## Overview

`RedEmulator` is the Game Boy (Red/Blue, Gen 1) sibling of
[`pokemon_env-emulator`](pokemon_env-emulator.md)'s Emerald (GBA, Gen 3) wrapper — same shape
(`memory_reader`, `milestone_tracker`, `initialize`), separate implementation, reflecting the two
generations' different memory layouts. This is the mechanism behind the repo's own `--game red`/`--game
emerald` selector (see [context-reset-and-playbook](../../Retrodict/doc-concepts/context-reset-and-playbook.md)-adjacent
per-game infrastructure split noted in this silo's source page).

## See also
- [`pokemon_env-emulator`](pokemon_env-emulator.md) — the Emerald counterpart.
