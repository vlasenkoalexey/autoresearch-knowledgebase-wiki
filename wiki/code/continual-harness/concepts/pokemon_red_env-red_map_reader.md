---
title: RedMapReader — Gen 1 map data and NPC/sprite tracking
type: concept
provenance: mixed
concept: pokemon_red_env-red_map_reader
updated: 2026-08-12
status: fresh
---
# RedMapReader — Gen 1 map data and NPC/sprite tracking

## Overview

`RedMapReader.get_whole_map_data` — *"Return complete map data for /whole_map endpoint"* — reads tile
behaviors via [`pokemon_red_env-utils-red_metatile_behavior`](pokemon_red_env-utils-red_metatile_behavior.md)'s
`RedMetatileBehavior` enum and tracks NPC/sprite/obstacle state across calls (`_ensure_npc_cache`,
`_detect_cleared_obstacles`) — the Gen 1 counterpart to
[`utils-mapping-map_stitcher`](utils-mapping-map_stitcher.md)'s persistent world map.

## See also
- [`pokemon_red_env-utils-red_metatile_behavior`](pokemon_red_env-utils-red_metatile_behavior.md) — the tile vocabulary.
