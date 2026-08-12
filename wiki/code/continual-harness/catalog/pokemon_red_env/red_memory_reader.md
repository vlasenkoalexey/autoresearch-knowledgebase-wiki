---
title: 'Module: pokemon_red_env/red_memory_reader.py'
type: catalog
provenance: extracted
module: pokemon_red_env/red_memory_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.red_memory_reader`/
symbols:
  RedMemoryReader.get_comprehensive_state: RedMemoryReader#get_comprehensive_state().
  RED_ADDR.RED_ADDR: RED_ADDR.RED_ADDR.
  RedMemoryReader._read_u8: RedMemoryReader#_read_u8().
  RedMemoryReader.read_battle_details: RedMemoryReader#read_battle_details().
  RedMemoryReader.read_party_pokemon: RedMemoryReader#read_party_pokemon().
  RedMemoryReader.test_memory_reading: RedMemoryReader#test_memory_reading().
  RedMemoryReader._read_bytes: RedMemoryReader#_read_bytes().
  RedMemoryReader.is_in_dialog: RedMemoryReader#is_in_dialog().
  RedMemoryReader.read_screen_text: RedMemoryReader#read_screen_text().
  RedMemoryReader._build_progress_context: RedMemoryReader#_build_progress_context().
  RedMemoryReader.map_reader: RedMemoryReader#map_reader.
  RedMemoryReader.read_money: RedMemoryReader#read_money().
  RedMemoryReader.read_location: RedMemoryReader#read_location().
  RedMemoryReader.read_badges: RedMemoryReader#read_badges().
  _load_json_mapping: _load_json_mapping().
  RedMemoryReader.read_items: RedMemoryReader#read_items().
  RedMemoryReader.read_player_name: RedMemoryReader#read_player_name().
  RedMemoryReader.is_in_battle: RedMemoryReader#is_in_battle().
  RedMemoryReader.get_game_state: RedMemoryReader#get_game_state().
  RedMemoryReader.read_coordinates: RedMemoryReader#read_coordinates().
  RedMemoryReader._read_u16_be: RedMemoryReader#_read_u16_be().
  RedMemoryReader._check_area_transition: RedMemoryReader#_check_area_transition().
  RedMemoryReader.read_party_size: RedMemoryReader#read_party_size().
  RedMemoryReader.read_item_count: RedMemoryReader#read_item_count().
  RedMemoryReader.read_pokedex_caught_count: RedMemoryReader#read_pokedex_caught_count().
  RedMemoryReader.read_pokedex_seen_count: RedMemoryReader#read_pokedex_seen_count().
  RedMemoryReader._decode_gen1_text: RedMemoryReader#_decode_gen1_text().
  _TYPE_NAMES._TYPE_NAMES: _TYPE_NAMES._TYPE_NAMES.
  RedMemoryReader._has_dialog_box_borders: RedMemoryReader#_has_dialog_box_borders().
  RedMemoryReader.is_on_title_screen: RedMemoryReader#is_on_title_screen().
  RedMemoryReader.read_direction: RedMemoryReader#read_direction().
  RedMemoryReader.reset_dialog_tracking: RedMemoryReader#reset_dialog_tracking().
  RedMemoryReader.read_map_around_player: RedMemoryReader#read_map_around_player().
  logger: logger.
  _SPECIES_NAMES._SPECIES_NAMES: _SPECIES_NAMES._SPECIES_NAMES.
  _MOVE_NAMES._MOVE_NAMES: _MOVE_NAMES._MOVE_NAMES.
  _CHARMAP._CHARMAP: _CHARMAP._CHARMAP.
  RedMemoryReader: RedMemoryReader#
  RedMemoryReader._last_map_id: RedMemoryReader#_last_map_id.
  RedMemoryReader.set_map_reader: RedMemoryReader#set_map_reader().
  RedMemoryReader.clear_dialogue_cache_on_button_press: RedMemoryReader#clear_dialogue_cache_on_button_press().
  RedMemoryReader.test_memory_access: RedMemoryReader#test_memory_access().
  _ITEM_NAMES._ITEM_NAMES: _ITEM_NAMES._ITEM_NAMES.
  _MAP_NAMES._MAP_NAMES: _MAP_NAMES._MAP_NAMES.
  RedMemoryReader._area_transition_detected: RedMemoryReader#_area_transition_detected.
  RedMemoryReader._dialog_detection_enabled: RedMemoryReader#_dialog_detection_enabled.
  RedMemoryReader._read_u16_le: RedMemoryReader#_read_u16_le().
  PARTY_SLOT_SIZE: PARTY_SLOT_SIZE.
  RedMemoryReader.pyboy: RedMemoryReader#pyboy.
  RedMemoryReader._dialog_cache: RedMemoryReader#_dialog_cache.
  RedMemoryReader._status_name: RedMemoryReader#_status_name().
  _DATA_DIR: _DATA_DIR.
  RedMemoryReader._dialog_cache_time: RedMemoryReader#_dialog_cache_time.
  RedMemoryReader._bcd_to_int: RedMemoryReader#_bcd_to_int().
  RedMemoryReader._BOX_BORDER_CHARS: RedMemoryReader#_BOX_BORDER_CHARS.
  RedMemoryReader.invalidate_map_cache: RedMemoryReader#invalidate_map_cache().
  RED_BADGE_NAMES.RED_BADGE_NAMES: RED_BADGE_NAMES.RED_BADGE_NAMES.
  RedMemoryReader.__init__: RedMemoryReader#__init__().
---
# Module: [`pokemon_red_env/red_memory_reader.py`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py)

## Classes
### `RedMemoryReader`
- def: [`pokemon_red_env/red_memory_reader.py:136`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L136)
- doc: Memory reader for Pokemon Red using PyBoy backend.
- signature: `class RedMemoryReader:`
- members:
  - `_bcd_to_int(raw: bytes)` — [`L185`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L185) — Decode big-endian BCD bytes to integer (e.g. b'\x01\x23\x45' → 12345).
  - `_build_progress_context(self, party: List[Dict], badges: List[str])` — [`L522`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L522) — Build progress_context dict mirroring EmeraldEmulator's shape.
  - `_check_area_transition(self)` — [`L735`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L735) — Detect if player moved to a different map.
  - `_decode_gen1_text(byte_array: bytes)` — [`L193`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L193) — Decode Gen 1 custom character encoding to a Python string.
  - `_has_dialog_box_borders(self)` — [`L341`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L341) — Scan the bottom 5 rows of the VRAM tilemap for dialog box borders.
  - `_read_u16_be(self, addr: int)` — [`L166`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L166) — Read 2-byte big-endian unsigned integer.
  - `_read_u16_le(self, addr: int)` — [`L172`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L172) — Read 2-byte little-endian unsigned integer.
  - `_status_name(byte: int)` — [`L210`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L210) — Convert status condition byte to human-readable string.
  - `clear_dialogue_cache_on_button_press(self)` — [`L759`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L759) — Called when 'A' is pressed to dismiss dialog; resets cache.
  - `get_comprehensive_state(self, screenshot=None)` — [`L577`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L577) — Return a state dict with the same four-key shape as EmeraldEmulator.
  - `get_game_state(self)` — [`L366`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L366) — Return game state string matching pyboy_runner: 'title', 'battle', 'dialog', or 'overworld'.
  - `invalidate_map_cache(self, **kwargs)` — [`L750`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L750) — No-op — processed_map data is static; no cache to invalidate.
  - `is_in_battle(self)` — [`L328`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L328)
  - `is_in_dialog(self)` — [`L331`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L331) — Two-signal dialog detection: text_progress register + VRAM border check.
  - `is_on_title_screen(self)` — [`L361`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L361) — Detect the title screen (title_check == 0x1F and title_map_id == 0x00).
  - `read_badges(self)` — [`L323`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L323) — Return list of earned badge names (bit 0 = Boulder Badge).
  - `read_battle_details(self)` — [`L445`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L445) — Return battle info dict aligned with Emerald's structure, or None if not in battle.
  - `read_coordinates(self)` — [`L238`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L238) — Return (x, y) tile coordinates.
  - `read_direction(self)` — [`L376`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L376) — Return player facing direction as a cardinal string.
  - `read_item_count(self)` — [`L381`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L381)
  - `read_items(self)` — [`L384`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L384) — Return list of {item_id, name, quantity} dicts from player's bag.
  - `read_location(self)` — [`L244`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L244) — Return the map name string for the current map ID.
  - `read_map_around_player(self, radius: int = 7)` — [`L725`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L725) — Delegate to map_reader.read_map_around_player(radius), or return [].
  - `read_money(self)` — [`L234`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L234)
  - `read_party_pokemon(self)` — [`L252`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L252) — Parse all party Pokemon from RAM. Returns a list of dicts.
  - `read_party_size(self)` — [`L249`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L249)
  - `read_player_name(self)` — [`L230`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L230)
  - `read_pokedex_caught_count(self)` — [`L401`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L401) — Count bits set in the 19-byte 'owned' Pokedex bitfield.
  - `read_pokedex_seen_count(self)` — [`L406`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L406) — Count bits set in the 19-byte 'seen' Pokedex bitfield.
  - `read_screen_text(self)` — [`L414`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L414) — Decode VRAM tilemap to readable dialog text.
  - `reset_dialog_tracking(self)` — [`L754`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L754) — Reset any cached dialog state.
  - `set_map_reader(self, map_reader)` — [`L721`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L721) — Attach a RedMapReader instance (called by RedEmulator.initialize()).
  - `test_memory_access(self)` — [`L788`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L788) — Alias for server /debug/memory endpoint compatibility.
  - `test_memory_reading(self)` — [`L767`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L767) — Read a handful of known Red addresses and return diagnostic info.
  - `map_reader` — [`L149`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L149)
  - `pyboy` — [`L144`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L144)
- protocol/private: `_BOX_BORDER_CHARS`[`L412`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L412), `__init__`[`L143`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L143), `_area_transition_detected`[`L152`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L152), `_dialog_cache`[`L146`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L146), `_dialog_cache_time`[`L147`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L147), `_dialog_detection_enabled`[`L154`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L154), `_last_map_id`[`L151`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L151), `_read_bytes`[`L178`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L178), `_read_u8`[`L160`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L160)
- uses (calls/refs, reference-scoped): [`RED_ADDR`](red_memory_reader.md#RED_ADDR.RED_ADDR), [`_TYPE_NAMES`](red_memory_reader.md#_TYPE_NAMES._TYPE_NAMES), [`logger`](red_memory_reader.md#logger), [`_CHARMAP`](red_memory_reader.md#_CHARMAP._CHARMAP), [`_MOVE_NAMES`](red_memory_reader.md#_MOVE_NAMES._MOVE_NAMES), [`_SPECIES_NAMES`](red_memory_reader.md#_SPECIES_NAMES._SPECIES_NAMES), [`_ITEM_NAMES`](red_memory_reader.md#_ITEM_NAMES._ITEM_NAMES), [`_MAP_NAMES`](red_memory_reader.md#_MAP_NAMES._MAP_NAMES), [`PARTY_SLOT_SIZE`](red_memory_reader.md#PARTY_SLOT_SIZE), [`RED_BADGE_NAMES`](red_memory_reader.md#RED_BADGE_NAMES.RED_BADGE_NAMES)
- used by: [`main`](../server/app.md#main), [`memory_reader`](red_emulator.md#RedEmulator.memory_reader), [`get_comprehensive_state`](../server/app.md#get_comprehensive_state), [`step_environment`](../server/app.md#step_environment), [`debug_memory`](../server/app.md#debug_memory), [`initialize`](red_emulator.md#RedEmulator.initialize), [`init_for_multiprocess`](../server/app.md#init_for_multiprocess), [`periodic_milestone_updater`](../server/app.md#periodic_milestone_updater), [`load_state`](red_emulator.md#RedEmulator.load_state), [`get_comprehensive_state`](red_emulator.md#RedEmulator.get_comprehensive_state), [`debug_memory_dump`](../server/app.md#debug_memory_dump), [`_update_dialog_state_cache`](red_emulator.md#RedEmulator._update_dialog_state_cache), [`run_frame_with_buttons`](red_emulator.md#RedEmulator.run_frame_with_buttons), [`get_termination_condition`](../server/app.md#get_termination_condition), [`get_map_location`](red_emulator.md#RedEmulator.get_map_location), [`get_party_pokemon`](red_emulator.md#RedEmulator.get_party_pokemon), [`get_money`](red_emulator.md#RedEmulator.get_money), [`get_player_position`](red_emulator.md#RedEmulator.get_player_position), [`test_memory_reading`](red_emulator.md#RedEmulator.test_memory_reading), [`get_whole_map`](red_emulator.md#RedEmulator.get_whole_map), [`get_map_tiles`](red_emulator.md#RedEmulator.get_map_tiles)  (1 test-only)

## Functions
- `_load_json_mapping(filename: str)` — [`L20`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L20) — Load a JSON file from the data directory; return {} on failure.

## Module values
- `PARTY_SLOT_SIZE` — [`L121`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L121)
- `RED_ADDR` — [`L52`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L52)
- `RED_BADGE_NAMES` — [`L126`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L126)
- `_CHARMAP` — [`L39`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L39)
- `_DATA_DIR` — [`L17`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L17)
- `_ITEM_NAMES` — [`L45`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L45)
- `_MAP_NAMES` — [`L48`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L48)
- `_MOVE_NAMES` — [`L36`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L36)
- `_SPECIES_NAMES` — [`L33`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L33)
- `_TYPE_NAMES` — [`L42`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L42)
- `logger` — [`L15`](../../../../../raw/code/continual-harness/pokemon_red_env/red_memory_reader.py#L15)

