---
title: 'Module: pokemon_red_env/red_emulator.py'
type: catalog
provenance: extracted
module: pokemon_red_env/red_emulator.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.red_emulator`/
symbols:
  RedEmulator.memory_reader: RedEmulator#memory_reader.
  RedEmulator.milestone_tracker: RedEmulator#milestone_tracker.
  RedEmulator.initialize: RedEmulator#initialize().
  emu: emu.
  RedEmulator.load_state: RedEmulator#load_state().
  RedEmulator.get_comprehensive_state: RedEmulator#get_comprehensive_state().
  RedEmulator.pyboy: RedEmulator#pyboy.
  state: state.
  logger: logger.
  RedEmulator.stop: RedEmulator#stop().
  RedEmulator.check_and_update_milestones: RedEmulator#check_and_update_milestones().
  RedEmulator.press_buttons: RedEmulator#press_buttons().
  RedEmulator._update_dialog_state_cache: RedEmulator#_update_dialog_state_cache().
  RedEmulator.get_info: RedEmulator#get_info().
  RedEmulator.get_screenshot: RedEmulator#get_screenshot().
  RedEmulator.run_frame_with_buttons: RedEmulator#run_frame_with_buttons().
  state_bytes: state_bytes.
  RedEmulator._last_milestone_update: RedEmulator#_last_milestone_update.
  RedEmulator: RedEmulator#
  RedEmulator.save_state: RedEmulator#save_state().
  img: img.
  info: info.
  RedEmulator._frame_capture_loop: RedEmulator#_frame_capture_loop().
  result: result.
  RedEmulator.tick: RedEmulator#tick().
  RedEmulator.get_map_location: RedEmulator#get_map_location().
  RedEmulator.get_party_pokemon: RedEmulator#get_party_pokemon().
  RedEmulator.press_key: RedEmulator#press_key().
  RedEmulator.get_player_position: RedEmulator#get_player_position().
  RedEmulator.get_money: RedEmulator#get_money().
  RedEmulator._check_red_milestone: RedEmulator#_check_red_milestone().
  RedEmulator.get_milestones: RedEmulator#get_milestones().
  img2: img2.
  v: v.
  RedEmulator.start_frame_capture: RedEmulator#start_frame_capture().
  RedEmulator.test_memory_reading: RedEmulator#test_memory_reading().
  RedEmulator.get_whole_map: RedEmulator#get_whole_map().
  diag: diag.
  RedEmulator.get_current_fps: RedEmulator#get_current_fps().
  ROM_PATH: ROM_PATH.
  RedEmulator.rom_path: RedEmulator#rom_path.
  RedEmulator.width: RedEmulator#width.
  RedEmulator.height: RedEmulator#height.
  RedEmulator.frame_thread: RedEmulator#frame_thread.
  RedEmulator._cached_dialog_state: RedEmulator#_cached_dialog_state.
  RedEmulator.get_map_tiles: RedEmulator#get_map_tiles().
  RedEmulator.get_location: RedEmulator#get_location().
  RedEmulator.KEY_MAP: RedEmulator#KEY_MAP.
  RedEmulator._get_cache_dir: RedEmulator#_get_cache_dir().
  RedEmulator.get_coordinates: RedEmulator#get_coordinates().
  RedEmulator.running: RedEmulator#running.
  RedEmulator.frame_queue: RedEmulator#frame_queue.
  RedEmulator.get_latest_frame: RedEmulator#get_latest_frame().
  RedEmulator.process_input: RedEmulator#process_input().
  RedEmulator.headless: RedEmulator#headless.
  RedEmulator.sound: RedEmulator#sound.
  RedEmulator._last_dialog_check_time: RedEmulator#_last_dialog_check_time.
  RED_MILESTONES_ORDER: RED_MILESTONES_ORDER.
  RedEmulator.current_frame: RedEmulator#current_frame.
  RedEmulator._dialog_check_interval: RedEmulator#_dialog_check_interval.
  RedEmulator._current_state_file: RedEmulator#_current_state_file.
  RedEmulator._cached_state_time: RedEmulator#_cached_state_time.
  RedEmulator._cached_state: RedEmulator#_cached_state.
  k: k.
  RedEmulator.__init__: RedEmulator#__init__().
  RedEmulator.cache_dir: RedEmulator#cache_dir.
  RedEmulator._save_persistent_grids_for_state: RedEmulator#_save_persistent_grids_for_state().
  RedEmulator._load_persistent_grids_for_state: RedEmulator#_load_persistent_grids_for_state().
  RedEmulator._copy_state_files_to_cache: RedEmulator#_copy_state_files_to_cache().
---
# Module: [`pokemon_red_env/red_emulator.py`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py)

## Classes
### `RedEmulator`
- def: [`pokemon_red_env/red_emulator.py:94`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L94)
- doc: Emulator wrapper for Pokemon Red using PyBoy, matching EmeraldEmulator interface.
- signature: `class RedEmulator:`
- members:
  - `_check_red_milestone(self, milestone_id: str, game_state: Dict[str, Any])` — [`L499`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L499) — Return True if the given milestone's condition is satisfied.
  - `_copy_state_files_to_cache(self, state_filename: str)` — [`L339`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L339) — Stub — Red map file cache not needed.
  - `_load_persistent_grids_for_state(self, state_filename: str)` — [`L335`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L335) — Stub — Red map persistence not needed (processed_map is static).
  - `_save_persistent_grids_for_state(self, state_filename: str)` — [`L331`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L331) — Stub — Red map persistence not needed (processed_map is static).
  - `_update_dialog_state_cache(self)` — [`L236`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L236) — Periodically refresh _cached_dialog_state from the memory reader.
  - `check_and_update_milestones(self, game_state: Dict[str, Any], agent_step_count: int = None)` — [`L486`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L486) — Check current game state and mark Red-specific milestones.
  - `get_comprehensive_state(self, screenshot=None)` — [`L448`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L448) — Return full game state dict (same four-key shape as EmeraldEmulator).
  - `get_coordinates(self)` — [`L409`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L409) — Alias for get_player_position() — used by server's periodic_milestone_updater.
  - `get_current_fps(self, base_fps: int = 30)` — [`L278`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L278) — Return base_fps x 4 when a dialog box is active.
  - `get_info(self)` — [`L706`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L706)
  - `get_latest_frame(self)` — [`L297`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L297) — Return the current frame as a numpy array.
  - `get_location(self)` — [`L413`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L413) — Alias for get_map_location() — used by server's periodic_milestone_updater.
  - `get_map_location(self)` — [`L399`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L399) — Return current map location name.
  - `get_map_tiles(self, radius: int = 7)` — [`L433`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L433)
  - `get_milestones(self, agent_step_count: int = None)` — [`L638`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L638) — Return milestone progress dict.
  - `get_money(self)` — [`L417`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L417)
  - `get_party_pokemon(self)` — [`L425`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L425)
  - `get_player_position(self)` — [`L389`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L389) — Return {"x": int, "y": int} or None.
  - `get_screenshot(self)` — [`L286`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L286) — Return the current frame as a PIL Image (RGB).
  - `get_whole_map(self)` — [`L438`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L438) — Get complete map data for current location (for /whole_map endpoint).
  - `initialize(self)` — [`L158`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L158) — Load ROM, set up PyBoy, and attach RedMemoryReader.
  - `load_state(self, path: Optional[str] = None, state_bytes: Optional[bytes] = None)` — [`L365`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L365) — Load emulator state from file or bytes.
  - `press_buttons(self, buttons: List[str], hold_frames: int = 10, release_frames: int = 10)` — [`L261`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L261) — Press a sequence of buttons, each held for *hold_frames*.
  - `press_key(self, key: str, frames: int = 2)` — [`L250`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L250) — Hold a single key for *frames* frames then release.
  - `process_input(self, input_data: Dict[str, Any])` — [`L715`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L715) — Handle JSON-style input payload (same as EmeraldEmulator).
  - `run_frame_with_buttons(self, buttons: List[str])` — [`L208`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L208) — Press buttons for one frame then release — matches EmeraldEmulator.
  - `save_state(self, path: Optional[str] = None)` — [`L347`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L347) — Save emulator state. Returns bytes; also writes to *path* if given.
  - `start_frame_capture(self, fps: int = 30)` — [`L302`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L302) — Start background thread that captures frames at *fps*.
  - `stop(self)` — [`L188`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L188) — Stop emulator and clean up.
  - `test_memory_reading(self)` — [`L733`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L733) — Diagnostic: delegate to RedMemoryReader.test_memory_reading().
  - `tick(self, frames: int = 1)` — [`L202`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L202) — Advance emulator by *frames* frames.
  - `KEY_MAP` — [`L129`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L129)
  - `cache_dir` — [`L116`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L116)
  - `current_frame` — [`L108`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L108)
  - `frame_queue` — [`L107`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L107)
  - `frame_thread` — [`L109`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L109)
  - `headless` — [`L99`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L99)
  - `height` — [`L104`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L104)
  - `memory_reader` — [`L112`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L112)
  - `milestone_tracker` — [`L117`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L117)
  - `pyboy` — [`L102`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L102)
  - `rom_path` — [`L98`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L98)
  - `running` — [`L105`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L105)
  - `sound` — [`L100`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L100)
  - `width` — [`L103`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L103)
- protocol/private: `__init__`[`L97`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L97), `_cached_dialog_state`[`L122`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L122), `_cached_state`[`L478`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L478), `_cached_state_time`[`L479`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L479), `_current_state_file`[`L126`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L126), `_dialog_check_interval`[`L124`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L124), `_frame_capture_loop`[`L310`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L310), `_get_cache_dir`[`L145`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L145), `_last_dialog_check_time`[`L123`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L123), `_last_milestone_update`[`L646`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L646)
- uses (calls/refs, reference-scoped): [`get_comprehensive_state`](red_memory_reader.md#RedMemoryReader.get_comprehensive_state), [`milestones`](red_milestone_tracker.md#RedMilestoneTracker.milestones), [`get_cache_directory`](../utils/data_persistence/run_data_manager.md#get_cache_directory), [`filename`](red_milestone_tracker.md#RedMilestoneTracker.filename), [`read_party_pokemon`](red_memory_reader.md#RedMemoryReader.read_party_pokemon), [`mark_completed`](red_milestone_tracker.md#RedMilestoneTracker.mark_completed), [`test_memory_reading`](red_memory_reader.md#RedMemoryReader.test_memory_reading), [`logger`](red_emulator.md#logger), [`load_milestones_for_state`](red_milestone_tracker.md#RedMilestoneTracker.load_milestones_for_state), [`is_in_dialog`](red_memory_reader.md#RedMemoryReader.is_in_dialog), [`save_milestones_for_state`](red_milestone_tracker.md#RedMilestoneTracker.save_milestones_for_state), [`map_reader`](red_memory_reader.md#RedMemoryReader.map_reader), [`read_location`](red_memory_reader.md#RedMemoryReader.read_location), [`read_money`](red_memory_reader.md#RedMemoryReader.read_money), [`read_coordinates`](red_memory_reader.md#RedMemoryReader.read_coordinates), [`is_completed`](red_milestone_tracker.md#RedMilestoneTracker.is_completed), [`reset_dialog_tracking`](red_memory_reader.md#RedMemoryReader.reset_dialog_tracking), [`read_map_around_player`](red_memory_reader.md#RedMemoryReader.read_map_around_player), [`RedMemoryReader`](red_memory_reader.md#RedMemoryReader), [`clear_dialogue_cache_on_button_press`](red_memory_reader.md#RedMemoryReader.clear_dialogue_cache_on_button_press), [`set_map_reader`](red_memory_reader.md#RedMemoryReader.set_map_reader), [`RedMapReader`](red_map_reader.md#RedMapReader), [`RedMilestoneTracker`](red_milestone_tracker.md#RedMilestoneTracker), [`RED_MILESTONES_ORDER`](red_emulator.md#RED_MILESTONES_ORDER)
- used by: [`main`](../server/app.md#main), [`get_comprehensive_state`](../server/app.md#get_comprehensive_state), [`take_action`](../server/app.md#take_action), [`step_environment`](../server/app.md#step_environment), [`signal_handler`](../server/app.md#signal_handler), [`game_loop`](../server/app.md#game_loop), [`setup_environment`](../server/app.md#setup_environment), [`debug_memory`](../server/app.md#debug_memory), [`mcp_get_progress_summary`](../server/app.md#mcp_get_progress_summary), [`init_for_multiprocess`](../server/app.md#init_for_multiprocess), [`periodic_milestone_updater`](../server/app.md#periodic_milestone_updater), [`emu`](red_emulator.md#emu), [`get_whole_map`](../server/app.md#get_whole_map), [`state`](red_emulator.md#state), [`test_milestone_operations`](../server/app.md#test_milestone_operations), [`debug_memory_dump`](../server/app.md#debug_memory_dump), [`get_status`](../server/app.md#get_status), [`load_checkpoint`](../server/app.md#load_checkpoint), [`reset_milestones`](../server/app.md#reset_milestones), [`save_checkpoint`](../server/app.md#save_checkpoint), [`debug_milestones`](../server/app.md#debug_milestones), [`get_latest_frame`](../server/app.md#get_latest_frame), [`get_milestones`](../server/app.md#get_milestones), [`load_state_endpoint`](../server/app.md#load_state_endpoint), [`save_state_endpoint`](../server/app.md#save_state_endpoint), [`state_bytes`](red_emulator.md#state_bytes), [`get_config`](../server/app.md#get_config), [`img`](red_emulator.md#img), [`info`](red_emulator.md#info), [`result`](red_emulator.md#result), [`debug_memory_comprehensive`](../server/app.md#debug_memory_comprehensive), [`get_termination_condition`](../server/app.md#get_termination_condition), [`img2`](red_emulator.md#img2), [`diag`](red_emulator.md#diag)  (11 test-only)

## Module values
- `RED_MILESTONES_ORDER` — [`L29`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L29)
- `ROM_PATH` — [`L746`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L746)
- `diag` — [`L789`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L789)
- `emu` — [`L752`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L752)
- `img` — [`L763`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L763)
- `img2` — [`L803`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L803)
- `info` — [`L796`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L796)
- `k` — [`L790`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L790)
- `logger` — [`L24`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L24)
- `result` — [`L771`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L771)
- `state` — [`L809`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L809)
- `state_bytes` — [`L781`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L781)
- `v` — [`L790`](../../../../../raw/code/continual-harness/pokemon_red_env/red_emulator.py#L790)

