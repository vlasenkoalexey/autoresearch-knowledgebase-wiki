---
title: 'Module: utils/mapping/map_stitcher.py'
type: catalog
provenance: extracted
module: utils/mapping/map_stitcher.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.map_stitcher`/
symbols:
  MapArea.location_name: MapArea#location_name.
  MapStitcher.load_from_file: MapStitcher#load_from_file().
  logger: logger.
  MapStitcher.map_areas: MapStitcher#map_areas.
  MapStitcher.load_from_checkpoint: MapStitcher#load_from_checkpoint().
  MapStitcher.update_map_area: MapStitcher#update_map_area().
  MapArea.map_data: MapArea#map_data.
  MapStitcher._detect_warp_connection: MapStitcher#_detect_warp_connection().
  MapStitcher.get_world_map_layout: MapStitcher#get_world_map_layout().
  MapStitcher.save_to_file: MapStitcher#save_to_file().
  MapStitcher.save_to_checkpoint: MapStitcher#save_to_checkpoint().
  MapStitcher.warp_connections: MapStitcher#warp_connections.
  MapStitcher.get_location_connections: MapStitcher#get_location_connections().
  WarpConnection.to_map_id: WarpConnection#to_map_id.
  WarpConnection.from_map_id: WarpConnection#from_map_id.
  MapArea.player_last_position: MapArea#player_last_position.
  WarpConnection.get_reverse_connection: WarpConnection#get_reverse_connection().
  MapStitcher.get_connected_areas: MapStitcher#get_connected_areas().
  MapStitcher.generate_world_map_grid: MapStitcher#generate_world_map_grid().
  MapStitcher.get_location_grid: MapStitcher#get_location_grid().
  MapStitcher._connection_exists: MapStitcher#_connection_exists().
  MapStitcher.generate_location_map_display: MapStitcher#generate_location_map_display().
  WarpConnection.from_position: WarpConnection#from_position.
  MapArea.overworld_coords: MapArea#overworld_coords.
  MapStitcher.get_stats: MapStitcher#get_stats().
  WarpConnection.to_position: WarpConnection#to_position.
  MapStitcher._merge_map_tiles: MapStitcher#_merge_map_tiles().
  MapStitcher.update_save_file: MapStitcher#update_save_file().
  MapStitcher.resolve_unknown_location_names: MapStitcher#resolve_unknown_location_names().
  MapStitcher.update_location_name: MapStitcher#update_location_name().
  WarpConnection.warp_type: WarpConnection#warp_type.
  MapStitcher.update_overworld_coordinates: MapStitcher#update_overworld_coordinates().
  MapStitcher.get_all_location_grids: MapStitcher#get_all_location_grids().
  MapStitcher._determine_warp_direction: MapStitcher#_determine_warp_direction().
  WarpConnection.direction: WarpConnection#direction.
  MapStitcher.get_player_position_for_location: MapStitcher#get_player_position_for_location().
  WarpConnection: WarpConnection#
  MapArea: MapArea#
  MapArea.visited_count: MapArea#visited_count.
  MapStitcher.cache_dir: MapStitcher#cache_dir.
  MapStitcher.save_file: MapStitcher#save_file.
  MapStitcher.last_map_id: MapStitcher#last_map_id.
  MapArea.map_id: MapArea#map_id.
  MapArea.warp_tiles: MapArea#warp_tiles.
  MapStitcher: MapStitcher#
  MapStitcher.last_position: MapStitcher#last_position.
  MapArea.boundaries: MapArea#boundaries.
  MapArea.last_seen: MapArea#last_seen.
  MapArea.get_map_bounds: MapArea#get_map_bounds().
  MapArea.first_seen: MapArea#first_seen.
  MapArea.has_warp_at: MapArea#has_warp_at().
  MapStitcher.get_map_id: MapStitcher#get_map_id().
  MapStitcher._tile_to_symbol: MapStitcher#_tile_to_symbol().
  MapStitcher.__init__: MapStitcher#__init__().
  MapStitcher._detect_warp_tiles: MapStitcher#_detect_warp_tiles().
  MapStitcher.format_world_map_display: MapStitcher#format_world_map_display().
  MapStitcher.pending_warps: MapStitcher#pending_warps.
  MapStitcher._trim_null_rows: MapStitcher#_trim_null_rows().
  MapStitcher.decode_map_id: MapStitcher#decode_map_id().
  MapStitcher._calculate_boundaries: MapStitcher#_calculate_boundaries().
  MapStitcher._infer_overworld_coordinates: MapStitcher#_infer_overworld_coordinates().
  MapStitcher._should_trim_edge: MapStitcher#_should_trim_edge().
  MapStitcher._is_explorable_edge: MapStitcher#_is_explorable_edge().
---
# Module: [`utils/mapping/map_stitcher.py`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py)

## Classes
### `MapArea`
- def: [`utils/mapping/map_stitcher.py:47`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L47)
- doc: Represents a single map area with its data
- signature: `class MapArea:`
- members:
  - `get_map_bounds(self)` — [`L60`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L60) — Return (min_x, min_y, max_x, max_y) for this map
  - `has_warp_at(self, x: int, y: int)` — [`L66`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L66) — Check if there's a warp at the given position
  - `boundaries` — [`L54`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L54)
  - `first_seen` — [`L56`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L56)
  - `last_seen` — [`L57`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L57)
  - `location_name` — [`L50`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L50) — documented in [utils-mapping-map_stitcher](../../../concepts/utils-mapping-map_stitcher.md)
  - `map_data` — [`L51`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L51)
  - `map_id` — [`L49`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L49)
  - `overworld_coords` — [`L58`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L58)
  - `player_last_position` — [`L52`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L52)
  - `visited_count` — [`L55`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L55)
  - `warp_tiles` — [`L53`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L53)
- used by: [`load_from_file`](map_stitcher.md#MapStitcher.load_from_file), [`map_areas`](map_stitcher.md#MapStitcher.map_areas), [`load_from_checkpoint`](map_stitcher.md#MapStitcher.load_from_checkpoint), [`update_map_area`](map_stitcher.md#MapStitcher.update_map_area), [`_detect_warp_connection`](map_stitcher.md#MapStitcher._detect_warp_connection), [`get_stitched_map_info`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.get_stitched_map_info), [`get_world_map_layout`](map_stitcher.md#MapStitcher.get_world_map_layout), [`save_to_file`](map_stitcher.md#MapStitcher.save_to_file), [`save_to_checkpoint`](map_stitcher.md#MapStitcher.save_to_checkpoint), [`_sync_warp_connections_to_state_formatter`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._sync_warp_connections_to_state_formatter), [`get_location_connections`](map_stitcher.md#MapStitcher.get_location_connections), [`_build_location_connections_from_map_areas`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._build_location_connections_from_map_areas), [`add_connected_areas`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.add_connected_areas), [`get_connected_areas`](map_stitcher.md#MapStitcher.get_connected_areas), [`generate_world_map_grid`](map_stitcher.md#MapStitcher.generate_world_map_grid), [`get_location_grid`](map_stitcher.md#MapStitcher.get_location_grid), [`generate_location_map_display`](map_stitcher.md#MapStitcher.generate_location_map_display), [`get_stats`](map_stitcher.md#MapStitcher.get_stats), [`_merge_map_tiles`](map_stitcher.md#MapStitcher._merge_map_tiles), [`resolve_unknown_location_names`](map_stitcher.md#MapStitcher.resolve_unknown_location_names), [`update_location_name`](map_stitcher.md#MapStitcher.update_location_name), [`get_all_location_grids`](map_stitcher.md#MapStitcher.get_all_location_grids), [`update_overworld_coordinates`](map_stitcher.md#MapStitcher.update_overworld_coordinates), [`_determine_warp_direction`](map_stitcher.md#MapStitcher._determine_warp_direction), [`get_player_position_for_location`](map_stitcher.md#MapStitcher.get_player_position_for_location)

### `MapStitcher`
- def: [`utils/mapping/map_stitcher.py:73`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L73)
- doc: Main class for managing map stitching and connections
- signature: `class MapStitcher:`
- members:
  - `_calculate_boundaries(self, map_data: List[List[Tuple]])` — [`L408`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L408) — Calculate walkable boundaries of the map
  - `_connection_exists(self, connection: WarpConnection)` — [`L498`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L498) — Check if a similar connection already exists
  - `_detect_warp_connection(self, from_map_id: int, to_map_id: int, from_pos: Optional[Tuple[int, int]], to_pos: Tuple[int, int], timestamp: float)` — [`L420`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L420) — Detect and record warp connections between maps
  - `_detect_warp_tiles(self, map_data: List[List[Tuple]])` — [`L370`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L370) — Detect tiles that can be warps (doors, stairs, exits)
  - `_determine_warp_direction(self, from_area: MapArea, to_area: MapArea, from_pos: Tuple[int, int], to_pos: Tuple[int, int])` — [`L466`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L466) — Determine the direction of movement for a warp
  - `_infer_overworld_coordinates(self, location_name: str, player_pos: Tuple[int, int])` — [`L507`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L507) — Infer overworld coordinates - should return None to keep coordinates unknown until discovered
  - `_is_explorable_edge(self, x: int, y: int, location_grid: Dict[Tuple[int, int], str])` — [`L1703`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1703) — Check if an unexplored coordinate is worth exploring (adjacent to walkable tiles).
  - `_merge_map_tiles(self, area: MapArea, new_tiles: List[List[Tuple]], player_pos: Tuple[int, int])` — [`L95`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L95) — Merge new tiles into existing map data, building up complete map over time.
  - `_should_trim_edge(self, tiles, is_row=True)` — [`L1159`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1159) — Check if an edge (row or column) should be trimmed.
  - `_tile_to_symbol(self, tile, location_name: str = None)` — [`L1603`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1603) — Convert a tile tuple to a simplified symbol for display.
  - `_trim_null_rows(self, map_data: List[List])` — [`L1170`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1170) — Trim rows that are entirely null/None from map data to reduce file size.
  - `decode_map_id(self, map_id: int)` — [`L221`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L221) — Convert map ID back to bank/number
  - `format_world_map_display(self, current_map_id: Optional[int] = None, max_width: int = 50)` — [`L1717`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1717) — Format world map for display in agent context
  - `generate_location_map_display(self, location_name: str, player_pos: Tuple[int, int] = None, npcs: List[Dict] = None, connections: List[Dict] = None)` — [`L1234`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1234) — Generate a detailed map display for a specific location.
  - `generate_world_map_grid(self, current_map_id: Optional[int] = None)` — [`L1083`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1083) — Generate a world map grid showing discovered areas and connections
  - `get_all_location_grids(self, simplified: bool = True)` — [`L790`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L790) — Get grids for all known locations.
  - `get_connected_areas(self, map_id: int)` — [`L559`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L559) — Get all areas connected to the given map ID
  - `get_location_connections(self, location_name=None)` — [`L621`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L621) — Get connections for a specific location or all locations.
  - `get_location_grid(self, location_name: str, simplified: bool = True)` — [`L676`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L676) — Get a simplified grid representation of a location for display.
  - `get_map_id(self, map_bank: int, map_number: int)` — [`L217`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L217) — Convert map bank/number to unique ID
  - `get_player_position_for_location(self, location_name: str)` — [`L604`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L604) — Get the last known player position for a specific location.
  - `get_stats(self)` — [`L1064`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1064) — Get statistics about the stitched world map
  - `get_world_map_layout(self)` — [`L569`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L569) — Generate a layout showing how all areas connect
  - `load_from_checkpoint(self, checkpoint_data: dict)` — [`L1803`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1803) — Load map stitching data from checkpoint data structure
  - `load_from_file(self)` — [`L851`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L851) — Load stitching data from JSON file — documented in [utils-mapping-map_stitcher](../../../concepts/utils-mapping-map_stitcher.md)
  - `resolve_unknown_location_names(self, memory_reader=None)` — [`L531`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L531) — Try to resolve 'Unknown' location names using the memory reader if available
  - `save_to_checkpoint(self, checkpoint_data: dict)` — [`L1760`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L1760) — Save map stitching data to checkpoint data structure
  - `save_to_file(self)` — [`L802`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L802) — Save stitching data to JSON file
  - `update_location_name(self, map_id: int, location_name: str)` — [`L519`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L519) — Update location name for an existing area
  - `update_map_area(self, map_bank: int, map_number: int, location_name: str, map_data: List[List[Tuple]], player_pos: Tuple[int, int], timestamp: float, overworld_coords: Optional[Tuple[int, int]] = None)` — [`L234`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L234) — Update or create a map area with new data
  - `update_overworld_coordinates(self, map_id: int, coords: Tuple[int, int])` — [`L513`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L513) — Update overworld coordinates for a discovered area
  - `update_save_file(self, new_save_file: str)` — [`L225`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L225) — Update the save file path and reload data
  - `cache_dir` — [`L79`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L79)
  - `last_map_id` — [`L89`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L89)
  - `last_position` — [`L90`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L90)
  - `map_areas` — [`L86`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L86)
  - `pending_warps` — [`L88`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L88)
  - `save_file` — [`L85`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L85)
  - `warp_connections` — [`L87`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L87)
- protocol/private: `__init__`[`L76`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L76)
- uses (calls/refs, reference-scoped): [`MetatileBehavior`](../../pokemon_env/enums.md#MetatileBehavior), [`location_name`](map_stitcher.md#MapArea.location_name), [`logger`](map_stitcher.md#logger), [`map_data`](map_stitcher.md#MapArea.map_data), [`get_cache_directory`](../data_persistence/run_data_manager.md#get_cache_directory), [`to_map_id`](map_stitcher.md#WarpConnection.to_map_id), [`from_map_id`](map_stitcher.md#WarpConnection.from_map_id), [`player_last_position`](map_stitcher.md#MapArea.player_last_position), [`get_reverse_connection`](map_stitcher.md#WarpConnection.get_reverse_connection), [`from_position`](map_stitcher.md#WarpConnection.from_position), [`overworld_coords`](map_stitcher.md#MapArea.overworld_coords), [`to_position`](map_stitcher.md#WarpConnection.to_position), [`warp_type`](map_stitcher.md#WarpConnection.warp_type), [`direction`](map_stitcher.md#WarpConnection.direction), [`MapArea`](map_stitcher.md#MapArea), [`MapLocation`](../../pokemon_env/enums.md#MapLocation), [`WarpConnection`](map_stitcher.md#WarpConnection), [`visited_count`](map_stitcher.md#MapArea.visited_count), [`map_id`](map_stitcher.md#MapArea.map_id), [`warp_tiles`](map_stitcher.md#MapArea.warp_tiles), [`boundaries`](map_stitcher.md#MapArea.boundaries), [`last_seen`](map_stitcher.md#MapArea.last_seen), [`get_map_bounds`](map_stitcher.md#MapArea.get_map_bounds), [`first_seen`](map_stitcher.md#MapArea.first_seen), [`has_warp_at`](map_stitcher.md#MapArea.has_warp_at)
- used by: [`get_comprehensive_state`](../../server/app.md#get_comprehensive_state), [`_player_house_entered`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._player_house_entered), [`get_stitched_map_info`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.get_stitched_map_info), [`read_map`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.read_map), [`_sync_warp_connections_to_state_formatter`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._sync_warp_connections_to_state_formatter), [`_build_location_connections_from_map_areas`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._build_location_connections_from_map_areas), [`_save_persistent_grids_for_state`](../../pokemon_env/emulator.md#EmeraldEmulator._save_persistent_grids_for_state), [`add_connected_areas`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.add_connected_areas), [`_last_stitcher_save`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._last_stitcher_save), [`get_instance`](map_stitcher_singleton.md#get_instance), [`update_map_stitcher_save_file`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.update_map_stitcher_save_file), [`save_callback`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader.save_callback), [`_get_map_stitcher_instance`](../state_formatter.md#_get_map_stitcher_instance)

### `WarpConnection`
- def: [`utils/mapping/map_stitcher.py:21`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L21)
- doc: Represents a connection between two map areas
- signature: `class WarpConnection:`
- members:
  - `get_reverse_connection(self)` — [`L30`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L30) — Get the reverse direction of this warp
  - `direction` — [`L28`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L28)
  - `from_map_id` — [`L23`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L23)
  - `from_position` — [`L25`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L25)
  - `to_map_id` — [`L24`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L24)
  - `to_position` — [`L26`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L26)
  - `warp_type` — [`L27`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L27)
- used by: [`load_from_file`](map_stitcher.md#MapStitcher.load_from_file), [`load_from_checkpoint`](map_stitcher.md#MapStitcher.load_from_checkpoint), [`_detect_warp_connection`](map_stitcher.md#MapStitcher._detect_warp_connection), [`get_world_map_layout`](map_stitcher.md#MapStitcher.get_world_map_layout), [`warp_connections`](map_stitcher.md#MapStitcher.warp_connections), [`_sync_warp_connections_to_state_formatter`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._sync_warp_connections_to_state_formatter), [`get_location_connections`](map_stitcher.md#MapStitcher.get_location_connections), [`_build_location_connections_from_map_areas`](../../pokemon_env/memory_reader.md#PokemonEmeraldReader._build_location_connections_from_map_areas), [`get_connected_areas`](map_stitcher.md#MapStitcher.get_connected_areas), [`generate_world_map_grid`](map_stitcher.md#MapStitcher.generate_world_map_grid), [`_connection_exists`](map_stitcher.md#MapStitcher._connection_exists), [`get_stats`](map_stitcher.md#MapStitcher.get_stats)

## Module values
- `logger` — [`L18`](../../../../../../raw/code/continual-harness/utils/mapping/map_stitcher.py#L18)

