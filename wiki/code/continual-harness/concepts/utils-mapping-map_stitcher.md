---
title: MapStitcher — building a persistent world map from local observations
type: concept
provenance: mixed
concept: utils-mapping-map_stitcher
updated: 2026-08-12
status: fresh
---
# MapStitcher — building a persistent world map from local observations

## Overview

`MapStitcher` assembles a persistent, cross-session world map out of the locally-visible
[`MapArea`](../catalog/utils/mapping/map_stitcher.md#MapArea.location_name) observations the agent
accumulates as it explores — [`load_from_file`](../catalog/utils/mapping/map_stitcher.md#MapStitcher.load_from_file)
(*"Load stitching data from JSON file"*) persists `map_areas`, warp connections, and player position
history to disk, so map knowledge survives the same context resets
[`retrodiction-methodology`](../../Retrodict/doc-concepts/retrodiction-methodology.md)-style logs are
built to survive in [Retrodict](../../../sources/retrodict.md) — an independently-arrived-at instance of
the same "persist structured world knowledge outside the model's own context" pattern.

## See also
- [`pokemon_env-memory_reader`](pokemon_env-memory_reader.md) — the raw observation source this stitches.
