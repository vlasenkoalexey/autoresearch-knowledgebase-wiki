---
title: EmeraldEmulator — the emulator wrapper and milestone tracking
type: concept
provenance: mixed
concept: pokemon_env-emulator
updated: 2026-08-12
status: fresh
---
# EmeraldEmulator — the emulator wrapper and milestone tracking

## Overview

`EmeraldEmulator` wraps the underlying GBA emulator and owns
[`milestone_tracker`](../catalog/pokemon_env/emulator.md#EmeraldEmulator.milestone_tracker) — a
`MilestoneTracker` recording game-progress milestones as they're reached — alongside
[`load_state`](../catalog/pokemon_env/emulator.md#EmeraldEmulator.load_state) for save-state resumption,
the emulator-level counterpart to [Retrodict](../../../sources/retrodict.md)'s log-replay resume mechanism.

## See also
- [`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) — attaches to this emulator to read state.
