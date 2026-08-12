---
title: 'Module: server/app.py'
type: catalog
provenance: extracted
module: server/app.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `server.app`/
symbols:
  env: env.
  logger: logger.
  direct_objectives_manager: direct_objectives_manager.
  mcp_complete_direct_objective: mcp_complete_direct_objective().
  main: main().
  mcp_get_game_state: mcp_get_game_state().
  get_comprehensive_state: get_comprehensive_state().
  take_action: take_action().
  app: app.
  step_environment: step_environment().
  signal_handler: signal_handler().
  game_loop: game_loop().
  _update_objectives_cache: _update_objectives_cache().
  setup_environment: setup_environment().
  latest_metrics: latest_metrics.
  debug_memory: debug_memory().
  mcp_get_progress_summary: mcp_get_progress_summary().
  init_for_multiprocess: init_for_multiprocess().
  periodic_milestone_updater: periodic_milestone_updater().
  get_screenshot: get_screenshot().
  get_whole_map: get_whole_map().
  _build_story_planning_objective: _build_story_planning_objective().
  agent_step_count: agent_step_count.
  get_metrics: get_metrics().
  recent_button_presses: recent_button_presses.
  init_video_recording: init_video_recording().
  get_agent_thinking: get_agent_thinking().
  update_agent_step: update_agent_step().
  mcp_press_buttons: mcp_press_buttons().
  mcp_navigate_to: mcp_navigate_to().
  mcp_replan_objectives: mcp_replan_objectives().
  current_obs: current_obs.
  test_milestone_operations: test_milestone_operations().
  mcp_get_map_data: mcp_get_map_data().
  direct_objectives_sequence: direct_objectives_sequence.
  stream_agent_thinking.event_stream: stream_agent_thinking().event_stream().
  action_queue: action_queue.
  get_status: get_status().
  debug_memory_dump: debug_memory_dump().
  reset_milestones: reset_milestones().
  save_checkpoint: save_checkpoint().
  sync_llm_metrics: sync_llm_metrics().
  load_checkpoint: load_checkpoint().
  current_action: current_action.
  step_lock: step_lock.
  game_type: game_type.
  get_latest_frame: get_latest_frame().
  websocket_frames: websocket_frames().
  get_milestones: get_milestones().
  debug_milestones: debug_milestones().
  mcp_get_full_objective_sequence: mcp_get_full_objective_sequence().
  save_state_endpoint: save_state_endpoint().
  load_state_endpoint: load_state_endpoint().
  current_run_dir: current_run_dir.
  video_writer: video_writer.
  ActionRequest.buttons: ActionRequest#buttons.
  get_config: get_config().
  get_queue_status: get_queue_status().
  get_llm_logs: get_llm_logs().
  mcp_add_memory: mcp_add_memory().
  mcp_process_memory: mcp_process_memory().
  mcp_process_skill: mcp_process_skill().
  mcp_process_subagent: mcp_process_subagent().
  save_agent_history: save_agent_history().
  running: running.
  _state_cache: _state_cache.
  ConnectionManager.connect: ConnectionManager#connect().
  ConnectionManager.disconnect: ConnectionManager#disconnect().
  update_frame_cache: update_frame_cache().
  record_frame: record_frame().
  checkpoint_loading_enabled: checkpoint_loading_enabled.
  step_count: step_count.
  fps: fps.
  debug_memory_comprehensive: debug_memory_comprehensive().
  get_termination_condition: get_termination_condition().
  reset_metrics: reset_metrics().
  action_frames_remaining: action_frames_remaining.
  video_recording: video_recording.
  obs_lock: obs_lock.
  state_update_running: state_update_running.
  ConnectionManager.send_latest_frame: ConnectionManager#send_latest_frame().
  cleanup_video_recording: cleanup_video_recording().
  direct_objectives_start_index: direct_objectives_start_index.
  video_filename: video_filename.
  reset_game: reset_game().
  stream_agent_thinking: stream_agent_thinking().
  mcp_search_memory: mcp_search_memory().
  mcp_get_memory_summary: mcp_get_memory_summary().
  mcp_get_memory_overview: mcp_get_memory_overview().
  mcp_get_skill_overview: mcp_get_skill_overview().
  mcp_get_subagent_overview: mcp_get_subagent_overview().
  mcp_get_walkthrough: mcp_get_walkthrough().
  mcp_save_memory: mcp_save_memory().
  mcp_save_map: mcp_save_map().
  mcp_load_map: mcp_load_map().
  release_frames_remaining: release_frames_remaining.
  DEFAULT_SPEED: DEFAULT_SPEED.
  frame_manager: frame_manager.
  anticheat_tracker: anticheat_tracker.
  direct_objectives_battling_start_index: direct_objectives_battling_start_index.
  SPEED_PRESETS: SPEED_PRESETS.
  ConnectionManager.last_sent_frame_count: ConnectionManager#last_sent_frame_count.
  state_update_thread: state_update_thread.
  video_frame_skip: video_frame_skip.
  ConnectionManager.active_connections: ConnectionManager#active_connections.
  save_screenshot: save_screenshot().
  test_stream: test_stream().
  mcp_lookup_pokemon_info: mcp_lookup_pokemon_info().
  stop_server: stop_server().
  _provider_family_for_llm_log_entry: _provider_family_for_llm_log_entry().
  _require_state_api_key: _require_state_api_key().
  last_action_time: last_action_time.
  last_fps_log: last_fps_log.
  frame_count_since_log: frame_count_since_log.
  current_action_release_delay: current_action_release_delay.
  frame_cache_counter: frame_cache_counter.
  ConnectionManager.latest_frame: ConnectionManager#latest_frame.
  ActionRequest.source: ActionRequest#source.
  run_fastapi_server: run_fastapi_server().
  _build_porymap_visual_map_15x15: _build_porymap_visual_map_15x15().
  _coerce_replan_edits_to_list: _coerce_replan_edits_to_list().
  step_counter: step_counter.
  video_frame_counter: video_frame_counter.
  ActionRequest: ActionRequest#
  ActionRequest.metadata: ActionRequest#metadata.
  _update_objectives_cache.get_recent_for_category: _update_objectives_cache().get_recent_for_category().
  ACTION_HOLD_FRAMES: ACTION_HOLD_FRAMES.
  ACTION_RELEASE_DELAY: ACTION_RELEASE_DELAY.
  get_stream: get_stream().
  get_health: get_health().
  get_frame_from_cache: get_frame_from_cache().
  get_recent_actions: get_recent_actions().
  mcp_list_wiki_sources: mcp_list_wiki_sources().
  _format_interaction_type_for_ui: _format_interaction_type_for_ui().
  ENABLE_MAP_STITCHER: ENABLE_MAP_STITCHER.
  ConnectionManager.lock: ConnectionManager#lock.
  ActionRequest.speed: ActionRequest#speed.
  _is_simplest_scaffold: _is_simplest_scaffold().
  playwright_recording: playwright_recording.
  _state_cache_ttl: _state_cache_ttl.
  memory_lock: memory_lock.
  ConnectionManager: ConnectionManager#
  ActionRequest.hold_frames: ActionRequest#hold_frames.
  ActionRequest.release_frames: ActionRequest#release_frames.
  GameStateResponse: GameStateResponse#
  GameStateResponse.screenshot_base64: GameStateResponse#screenshot_base64.
  GameStateResponse.step_number: GameStateResponse#step_number.
  GameStateResponse.resolution: GameStateResponse#resolution.
  GameStateResponse.status: GameStateResponse#status.
  ComprehensiveStateResponse: ComprehensiveStateResponse#
  ComprehensiveStateResponse.visual: ComprehensiveStateResponse#visual.
  ComprehensiveStateResponse.player: ComprehensiveStateResponse#player.
  ComprehensiveStateResponse.game: ComprehensiveStateResponse#game.
  ComprehensiveStateResponse.milestones: ComprehensiveStateResponse#milestones.
  ComprehensiveStateResponse.location_connections: ComprehensiveStateResponse#location_connections.
  ComprehensiveStateResponse.step_number: ComprehensiveStateResponse#step_number.
  ComprehensiveStateResponse.status: ComprehensiveStateResponse#status.
  ComprehensiveStateResponse.action_queue_length: ComprehensiveStateResponse#action_queue_length.
  handle_input: handle_input().
  update_display: update_display().
  _build_porymap_visual_map_15x15._slice_row: _build_porymap_visual_map_15x15()._slice_row().
  test_stream.simple_stream: test_stream().simple_stream().
  debug_state_enabled: debug_state_enabled.
  _debug_state_counter: _debug_state_counter.
  _debug_state_log: _debug_state_log.
  playwright_thread: playwright_thread.
  playwright_video_path: playwright_video_path.
  FRAME_CACHE_FILE: FRAME_CACHE_FILE.
  frame_cache_skip_frames: frame_cache_skip_frames.
  ConnectionManager.__init__: ConnectionManager#__init__().
  draw_info_overlay: draw_info_overlay().
---
# Module: [`server/app.py`](../../../../../raw/code/continual-harness/server/app.py)

## Classes
### `ActionRequest`  ·  implements/extends BaseModel
- def: [`server/app.py:415`](../../../../../raw/code/continual-harness/server/app.py#L415)
- signature: `class ActionRequest(BaseModel):`
- members:
  - `buttons` — [`L416`](../../../../../raw/code/continual-harness/server/app.py#L416)
  - `hold_frames` — [`L420`](../../../../../raw/code/continual-harness/server/app.py#L420)
  - `metadata` — [`L423`](../../../../../raw/code/continual-harness/server/app.py#L423)
  - `release_frames` — [`L421`](../../../../../raw/code/continual-harness/server/app.py#L421)
  - `source` — [`L422`](../../../../../raw/code/continual-harness/server/app.py#L422)
  - `speed` — [`L419`](../../../../../raw/code/continual-harness/server/app.py#L419)
- used by: [`take_action`](app.md#take_action), [`mcp_navigate_to`](app.md#mcp_navigate_to), [`mcp_press_buttons`](app.md#mcp_press_buttons)

### `ComprehensiveStateResponse`  ·  implements/extends BaseModel
- def: [`server/app.py:433`](../../../../../raw/code/continual-harness/server/app.py#L433)
- signature: `class ComprehensiveStateResponse(BaseModel):`
- members:
  - `action_queue_length` — [`L442`](../../../../../raw/code/continual-harness/server/app.py#L442)
  - `game` — [`L436`](../../../../../raw/code/continual-harness/server/app.py#L436)
  - `location_connections` — [`L439`](../../../../../raw/code/continual-harness/server/app.py#L439)
  - `milestones` — [`L438`](../../../../../raw/code/continual-harness/server/app.py#L438)
  - `player` — [`L435`](../../../../../raw/code/continual-harness/server/app.py#L435)
  - `status` — [`L441`](../../../../../raw/code/continual-harness/server/app.py#L441)
  - `step_number` — [`L440`](../../../../../raw/code/continual-harness/server/app.py#L440)
  - `visual` — [`L434`](../../../../../raw/code/continual-harness/server/app.py#L434)
- used by: [`get_comprehensive_state`](app.md#get_comprehensive_state)

### `ConnectionManager`
- def: [`server/app.py:206`](../../../../../raw/code/continual-harness/server/app.py#L206)
- doc: Manages WebSocket connections for real-time frame streaming
- signature: `class ConnectionManager:`
- members:
  - `connect(self, websocket: WebSocket)` — [`L215`](../../../../../raw/code/continual-harness/server/app.py#L215)
  - `disconnect(self, websocket: WebSocket)` — [`L222`](../../../../../raw/code/continual-harness/server/app.py#L222)
  - `send_latest_frame(self, websocket: WebSocket)` — [`L231`](../../../../../raw/code/continual-harness/server/app.py#L231) — Send latest frame to a specific connection if new frame available
  - `active_connections` — [`L210`](../../../../../raw/code/continual-harness/server/app.py#L210)
  - `last_sent_frame_count` — [`L213`](../../../../../raw/code/continual-harness/server/app.py#L213)
  - `latest_frame` — [`L212`](../../../../../raw/code/continual-harness/server/app.py#L212)
  - `lock` — [`L211`](../../../../../raw/code/continual-harness/server/app.py#L211)
- protocol/private: `__init__`[`L209`](../../../../../raw/code/continual-harness/server/app.py#L209)
- uses (calls/refs, reference-scoped): [`logger`](app.md#logger)
- used by: [`websocket_frames`](app.md#websocket_frames), [`update_frame_cache`](app.md#update_frame_cache), [`frame_manager`](app.md#frame_manager)

### `GameStateResponse`  ·  implements/extends BaseModel
- def: [`server/app.py:426`](../../../../../raw/code/continual-harness/server/app.py#L426)
- signature: `class GameStateResponse(BaseModel):`
- members:
  - `resolution` — [`L429`](../../../../../raw/code/continual-harness/server/app.py#L429)
  - `screenshot_base64` — [`L427`](../../../../../raw/code/continual-harness/server/app.py#L427)
  - `status` — [`L430`](../../../../../raw/code/continual-harness/server/app.py#L430)
  - `step_number` — [`L428`](../../../../../raw/code/continual-harness/server/app.py#L428)
- used by: [`get_screenshot`](app.md#get_screenshot)

## Functions
- `_build_porymap_visual_map_15x15(state: Dict[str, Any], player_coords: Tuple[int, int])` — [`L1323`](../../../../../raw/code/continual-harness/server/app.py#L1323) — Set ``state['map']['visual_map']`` from elevation-filtered ``porymap.grid`` (15x15 around player).
- `_build_story_planning_objective()` — [`L78`](../../../../../raw/code/continual-harness/server/app.py#L78) — Create scaffold-aware planning guidance when story objectives run out.
- `_coerce_replan_edits_to_list(edits: Any)` — [`L4059`](../../../../../raw/code/continual-harness/server/app.py#L4059) — Normalize ``edits`` from JSON / odd client encodings into ``list[dict]``.
- `_format_interaction_type_for_ui(interaction_type: str)` — [`L117`](../../../../../raw/code/continual-harness/server/app.py#L117) — Normalize orchestrator labels for UI readability.
- `_is_simplest_scaffold()` — [`L73`](../../../../../raw/code/continual-harness/server/app.py#L73) — Return True when the run is using the simplest scaffold.
- `_provider_family_for_llm_log_entry(entry: dict)` — [`L137`](../../../../../raw/code/continual-harness/server/app.py#L137) — UI color bucket from raw log line (handles OpenRouter via model slug).
- `_require_state_api_key(request: Request)` — [`L4328`](../../../../../raw/code/continual-harness/server/app.py#L4328) — When POKEMON_STATE_API_KEY is set (e.g. by run_cli), require X-Internal-API-Key header.
- `_slice_row(row: Any, sx: int, ex: int)` — [`L1342`](../../../../../raw/code/continual-harness/server/app.py#L1342)
- `_update_objectives_cache()` — [`L2512`](../../../../../raw/code/continual-harness/server/app.py#L2512) — Write current objectives state to fast-access cache file
- `cleanup_video_recording()` — [`L380`](../../../../../raw/code/continual-harness/server/app.py#L380) — Clean up video recording resources
- `debug_memory()` — [`L1876`](../../../../../raw/code/continual-harness/server/app.py#L1876) — Debug memory reading (basic version)
- `debug_memory_comprehensive()` — [`L1939`](../../../../../raw/code/continual-harness/server/app.py#L1939) — Comprehensive memory reading test with detailed diagnostics
- `debug_memory_dump(start: int = 33554432, length: int = 4096)` — [`L1955`](../../../../../raw/code/continual-harness/server/app.py#L1955) — Dump raw memory from the emulator
- `debug_milestones()` — [`L2694`](../../../../../raw/code/continual-harness/server/app.py#L2694) — Debug milestone tracking system
- `draw_info_overlay()` — [`L736`](../../../../../raw/code/continual-harness/server/app.py#L736) — Draw info overlay - server runs headless, no overlay needed
- `event_stream()` — [`L2014`](../../../../../raw/code/continual-harness/server/app.py#L2014) — Generate server-sent events for agent thinking
- `game_loop(manual_mode=False)` — [`L769`](../../../../../raw/code/continual-harness/server/app.py#L769) — Main game loop - runs in main thread, always headless
- `get_agent_thinking()` — [`L2147`](../../../../../raw/code/continual-harness/server/app.py#L2147) — Get current agent thinking status and recent LLM interactions
- `get_comprehensive_state()` — [`L1381`](../../../../../raw/code/continual-harness/server/app.py#L1381) — Get comprehensive game state including visual and memory data
- `get_config()` — [`L938`](../../../../../raw/code/continual-harness/server/app.py#L938) — Return server configuration (game type, resolution) for dynamic UI
- `get_frame_from_cache()` — [`L1050`](../../../../../raw/code/continual-harness/server/app.py#L1050) — DISABLED - Use WebSocket /ws/frames for real-time streaming instead
- `get_health()` — [`L948`](../../../../../raw/code/continual-harness/server/app.py#L948) — Health check endpoint for server monitoring
- `get_latest_frame()` — [`L1013`](../../../../../raw/code/continual-harness/server/app.py#L1013) — Get latest game frame in same format as single-process mode
- `get_llm_logs()` — [`L2480`](../../../../../raw/code/continual-harness/server/app.py#L2480) — Get recent LLM log entries
- `get_metrics()` — [`L2231`](../../../../../raw/code/continual-harness/server/app.py#L2231) — Get cumulative metrics for the run
- `get_milestones()` — [`L2632`](../../../../../raw/code/continual-harness/server/app.py#L2632) — Get current milestones achieved based on persistent tracking
- `get_queue_status()` — [`L1303`](../../../../../raw/code/continual-harness/server/app.py#L1303) — Get action queue status
- `get_recent_actions()` — [`L2684`](../../../../../raw/code/continual-harness/server/app.py#L2684) — Get recently pressed buttons
- `get_recent_for_category(category, sequence, index)` — [`L2531`](../../../../../raw/code/continual-harness/server/app.py#L2531)
- `get_screenshot()` — [`L975`](../../../../../raw/code/continual-harness/server/app.py#L975) — Get current screenshot
- `get_status()` — [`L954`](../../../../../raw/code/continual-harness/server/app.py#L954) — Get server status
- `get_stream()` — [`L926`](../../../../../raw/code/continual-harness/server/app.py#L926) — Serve the stream.html interface
- `get_termination_condition(condition_type: str = "gym_badge_count", threshold: int = 1)` — [`L2290`](../../../../../raw/code/continual-harness/server/app.py#L2290) — Check if a termination condition is met based on ground-truth memory data.
- `get_whole_map()` — [`L1744`](../../../../../raw/code/continual-harness/server/app.py#L1744) — Get complete map data including full grid, raw tiles, and elevation info for debugging
- `handle_input(manual_mode=False)` — [`L627`](../../../../../raw/code/continual-harness/server/app.py#L627) — Handle input - server runs headless, no input handling needed
- `init_for_multiprocess()` — [`L4923`](../../../../../raw/code/continual-harness/server/app.py#L4923) — Initialize emulator when server is imported for multiprocess mode
- `init_video_recording(record_enabled=False)` — [`L262`](../../../../../raw/code/continual-harness/server/app.py#L262) — Initialize video recording if enabled
- `load_checkpoint()` — [`L4591`](../../../../../raw/code/continual-harness/server/app.py#L4591) — Load checkpoint state - called by client on startup if --load-checkpoint flag is used
- `load_state_endpoint(request: Request)` — [`L4367`](../../../../../raw/code/continual-harness/server/app.py#L4367) — Load an emulator state from a file
- `main()` — [`L4628`](../../../../../raw/code/continual-harness/server/app.py#L4628) — Main function
- `mcp_add_memory(request: dict)` — [`L3599`](../../../../../raw/code/continual-harness/server/app.py#L3599) — MCP Tool: Add entry to long-term memory (persistent across runs)
- `mcp_complete_direct_objective(request: dict)` — [`L3218`](../../../../../raw/code/continual-harness/server/app.py#L3218) — MCP Tool: Complete current direct objective — documented in [server-app](../../concepts/server-app.md)
- `mcp_get_full_objective_sequence()` — [`L4109`](../../../../../raw/code/continual-harness/server/app.py#L4109) — MCP Tool: Return the complete objective state across all categories (used by subagent_plan_objectives).
- `mcp_get_game_state()` — [`L2822`](../../../../../raw/code/continual-harness/server/app.py#L2822) — MCP Tool: Get current game state
- `mcp_get_map_data()` — [`L2982`](../../../../../raw/code/continual-harness/server/app.py#L2982) — MCP Tool: Get structured map data for skill code.
- `mcp_get_memory_overview(request: dict)` — [`L3662`](../../../../../raw/code/continual-harness/server/app.py#L3662) — MCP Tool: Get long-term memory tree overview (compact [id] title tree).
- `mcp_get_memory_summary(request: dict)` — [`L3650`](../../../../../raw/code/continual-harness/server/app.py#L3650) — MCP Tool: Get long-term memory summary (persistent across runs)
- `mcp_get_progress_summary(request: dict)` — [`L4131`](../../../../../raw/code/continual-harness/server/app.py#L4131) — MCP Tool: Get comprehensive progress summary.
- `mcp_get_skill_overview(request: dict)` — [`L3700`](../../../../../raw/code/continual-harness/server/app.py#L3700) — MCP Tool: Get skill library tree overview (compact [id] name tree).
- `mcp_get_subagent_overview(request: dict)` — [`L3738`](../../../../../raw/code/continual-harness/server/app.py#L3738) — MCP Tool: Get subagent registry tree overview (compact [id] name tree).
- `mcp_get_walkthrough(request: dict)` — [`L3931`](../../../../../raw/code/continual-harness/server/app.py#L3931) — MCP Tool: Get Pokemon Emerald walkthrough part
- `mcp_list_wiki_sources()` — [`L3891`](../../../../../raw/code/continual-harness/server/app.py#L3891) — MCP Tool: List available wiki sources
- `mcp_load_map(request: dict)` — [`L4267`](../../../../../raw/code/continual-harness/server/app.py#L4267) — MCP Tool: Load agent's previously saved mental map of a location (SLAM)
- `mcp_lookup_pokemon_info(request: dict)` — [`L3776`](../../../../../raw/code/continual-harness/server/app.py#L3776) — MCP Tool: Lookup Pokemon info from wikis
- `mcp_navigate_to(request: dict)` — [`L3546`](../../../../../raw/code/continual-harness/server/app.py#L3546) — MCP Tool: Navigate to coordinates using pathfinding
- `mcp_press_buttons(request: dict)` — [`L3117`](../../../../../raw/code/continual-harness/server/app.py#L3117) — MCP Tool: Press GBA buttons
- `mcp_process_memory(request: dict)` — [`L3674`](../../../../../raw/code/continual-harness/server/app.py#L3674) — MCP Tool: Unified CRUD for long-term memory (read/add/update/delete).
- `mcp_process_skill(request: dict)` — [`L3712`](../../../../../raw/code/continual-harness/server/app.py#L3712) — MCP Tool: Unified CRUD for skill library (read/add/update/delete).
- `mcp_process_subagent(request: dict)` — [`L3750`](../../../../../raw/code/continual-harness/server/app.py#L3750) — MCP Tool: Unified CRUD for subagent registry (read/add/update/delete).
- `mcp_replan_objectives(request: dict)` — [`L4065`](../../../../../raw/code/continual-harness/server/app.py#L4065) — MCP Tool: Apply index-based edits to a single objective category (used by subagent_plan_objectives).
- `mcp_save_map(request: dict)` — [`L4224`](../../../../../raw/code/continual-harness/server/app.py#L4224) — MCP Tool: Save agent's mental map of a location to file (SLAM)
- `mcp_save_memory(request: dict)` — [`L4023`](../../../../../raw/code/continual-harness/server/app.py#L4023) — MCP Tool: Save facts to persistent memory (saved to run directory)
- `mcp_search_memory(request: dict)` — [`L3632`](../../../../../raw/code/continual-harness/server/app.py#L3632) — MCP Tool: Search long-term memory (persistent across runs)
- `periodic_milestone_updater()` — [`L445`](../../../../../raw/code/continual-harness/server/app.py#L445) — Lightweight background thread that only updates milestones occasionally
- `record_frame(screenshot)` — [`L345`](../../../../../raw/code/continual-harness/server/app.py#L345) — Record frame to video if recording is enabled with frame skipping
- `reset_game()` — [`L757`](../../../../../raw/code/continual-harness/server/app.py#L757) — Reset the game and all milestones
- `reset_metrics()` — [`L2353`](../../../../../raw/code/continual-harness/server/app.py#L2353) — Reset all metrics to zero for fresh start
- `reset_milestones()` — [`L2742`](../../../../../raw/code/continual-harness/server/app.py#L2742) — Reset all milestones (for testing)
- `run_fastapi_server(port)` — [`L911`](../../../../../raw/code/continual-harness/server/app.py#L911) — Run FastAPI server in background thread
- `save_agent_history()` — [`L4568`](../../../../../raw/code/continual-harness/server/app.py#L4568) — Save agent history to checkpoint_llm.txt (called by client after each step)
- `save_checkpoint(request_data: dict = None)` — [`L4393`](../../../../../raw/code/continual-harness/server/app.py#L4393) — Save checkpoint - called by client when step count reaches checkpoint interval
- `save_screenshot()` — [`L742`](../../../../../raw/code/continual-harness/server/app.py#L742) — Save current screenshot
- `save_state_endpoint(request: Request)` — [`L4343`](../../../../../raw/code/continual-harness/server/app.py#L4343) — Save the current emulator state to a file
- `setup_environment(skip_initial_state=False)` — [`L578`](../../../../../raw/code/continual-harness/server/app.py#L578) — Initialize the emulator
- `signal_handler(signum, frame)` — [`L490`](../../../../../raw/code/continual-harness/server/app.py#L490) — Handle shutdown signals gracefully
- `simple_stream()` — [`L1998`](../../../../../raw/code/continual-harness/server/app.py#L1998)
- `step_environment(actions_pressed)` — [`L633`](../../../../../raw/code/continual-harness/server/app.py#L633) — Take a step in the environment with optimized locking for better performance
- `stop_server()` — [`L4321`](../../../../../raw/code/continual-harness/server/app.py#L4321) — Stop the server
- `stream_agent_thinking()` — [`L2008`](../../../../../raw/code/continual-harness/server/app.py#L2008) — Stream agent thinking in real-time using Server-Sent Events
- `sync_llm_metrics(request: Request)` — [`L4428`](../../../../../raw/code/continual-harness/server/app.py#L4428) — Sync LLM cumulative metrics from client to server
- `take_action(request: ActionRequest)` — [`L1088`](../../../../../raw/code/continual-harness/server/app.py#L1088) — Take an action
- `test_milestone_operations()` — [`L2760`](../../../../../raw/code/continual-harness/server/app.py#L2760) — Test milestone loading and saving operations
- `test_stream()` — [`L1993`](../../../../../raw/code/continual-harness/server/app.py#L1993) — Simple test stream to verify SSE works
- `update_agent_step(request: Request = None)` — [`L2379`](../../../../../raw/code/continual-harness/server/app.py#L2379) — Update the agent step count and metrics
- `update_display(manual_mode=False)` — [`L730`](../../../../../raw/code/continual-harness/server/app.py#L730) — Update display - server runs headless, no display update needed
- `update_frame_cache(screenshot)` — [`L302`](../../../../../raw/code/continual-harness/server/app.py#L302) — Update frame cache for WebSocket streaming - NO FILE I/O!
- `websocket_frames(websocket: WebSocket)` — [`L1059`](../../../../../raw/code/continual-harness/server/app.py#L1059) — WebSocket endpoint for real-time frame streaming

## Module values
- `ACTION_HOLD_FRAMES` — [`L166`](../../../../../raw/code/continual-harness/server/app.py#L166)
- `ACTION_RELEASE_DELAY` — [`L167`](../../../../../raw/code/continual-harness/server/app.py#L167)
- `DEFAULT_SPEED` — [`L163`](../../../../../raw/code/continual-harness/server/app.py#L163)
- `ENABLE_MAP_STITCHER` — [`L191`](../../../../../raw/code/continual-harness/server/app.py#L191)
- `FRAME_CACHE_FILE` — [`L185`](../../../../../raw/code/continual-harness/server/app.py#L185)
- `SPEED_PRESETS` — [`L158`](../../../../../raw/code/continual-harness/server/app.py#L158)
- `_debug_state_counter` — [`L67`](../../../../../raw/code/continual-harness/server/app.py#L67)
- `_debug_state_log` — [`L68`](../../../../../raw/code/continual-harness/server/app.py#L68)
- `_state_cache` — [`L194`](../../../../../raw/code/continual-harness/server/app.py#L194)
- `_state_cache_ttl` — [`L195`](../../../../../raw/code/continual-harness/server/app.py#L195)
- `action_frames_remaining` — [`L152`](../../../../../raw/code/continual-harness/server/app.py#L152)
- `action_queue` — [`L150`](../../../../../raw/code/continual-harness/server/app.py#L150)
- `agent_step_count` — [`L65`](../../../../../raw/code/continual-harness/server/app.py#L65)
- `anticheat_tracker` — [`L55`](../../../../../raw/code/continual-harness/server/app.py#L55)
- `app` — [`L398`](../../../../../raw/code/continual-harness/server/app.py#L398)
- `checkpoint_loading_enabled` — [`L2349`](../../../../../raw/code/continual-harness/server/app.py#L2349)
- `current_action` — [`L151`](../../../../../raw/code/continual-harness/server/app.py#L151)
- `current_action_release_delay` — [`L154`](../../../../../raw/code/continual-harness/server/app.py#L154)
- `current_obs` — [`L69`](../../../../../raw/code/continual-harness/server/app.py#L69)
- `current_run_dir` — [`L64`](../../../../../raw/code/continual-harness/server/app.py#L64)
- `debug_state_enabled` — [`L66`](../../../../../raw/code/continual-harness/server/app.py#L66)
- `direct_objectives_battling_start_index` — [`L62`](../../../../../raw/code/continual-harness/server/app.py#L62)
- `direct_objectives_manager` — [`L63`](../../../../../raw/code/continual-harness/server/app.py#L63)
- `direct_objectives_sequence` — [`L60`](../../../../../raw/code/continual-harness/server/app.py#L60)
- `direct_objectives_start_index` — [`L61`](../../../../../raw/code/continual-harness/server/app.py#L61)
- `env` — [`L54`](../../../../../raw/code/continual-harness/server/app.py#L54)
- `fps` — [`L70`](../../../../../raw/code/continual-harness/server/app.py#L70)
- `frame_cache_counter` — [`L186`](../../../../../raw/code/continual-harness/server/app.py#L186)
- `frame_cache_skip_frames` — [`L187`](../../../../../raw/code/continual-harness/server/app.py#L187)
- `frame_count_since_log` — [`L149`](../../../../../raw/code/continual-harness/server/app.py#L149)
- `frame_manager` — [`L252`](../../../../../raw/code/continual-harness/server/app.py#L252)
- `game_type` — [`L51`](../../../../../raw/code/continual-harness/server/app.py#L51)
- `last_action_time` — [`L57`](../../../../../raw/code/continual-harness/server/app.py#L57)
- `last_fps_log` — [`L148`](../../../../../raw/code/continual-harness/server/app.py#L148)
- `latest_metrics` — [`L2277`](../../../../../raw/code/continual-harness/server/app.py#L2277)
- `logger` — [`L48`](../../../../../raw/code/continual-harness/server/app.py#L48)
- `memory_lock` — [`L202`](../../../../../raw/code/continual-harness/server/app.py#L202)
- `obs_lock` — [`L200`](../../../../../raw/code/continual-harness/server/app.py#L200)
- `playwright_recording` — [`L177`](../../../../../raw/code/continual-harness/server/app.py#L177)
- `playwright_thread` — [`L178`](../../../../../raw/code/continual-harness/server/app.py#L178)
- `playwright_video_path` — [`L179`](../../../../../raw/code/continual-harness/server/app.py#L179)
- `recent_button_presses` — [`L2680`](../../../../../raw/code/continual-harness/server/app.py#L2680)
- `release_frames_remaining` — [`L153`](../../../../../raw/code/continual-harness/server/app.py#L153)
- `running` — [`L58`](../../../../../raw/code/continual-harness/server/app.py#L58)
- `state_update_running` — [`L256`](../../../../../raw/code/continual-harness/server/app.py#L256)
- `state_update_thread` — [`L255`](../../../../../raw/code/continual-harness/server/app.py#L255)
- `step_count` — [`L59`](../../../../../raw/code/continual-harness/server/app.py#L59)
- `step_counter` — [`L56`](../../../../../raw/code/continual-harness/server/app.py#L56)
- `step_lock` — [`L201`](../../../../../raw/code/continual-harness/server/app.py#L201)
- `video_filename` — [`L172`](../../../../../raw/code/continual-harness/server/app.py#L172)
- `video_frame_counter` — [`L173`](../../../../../raw/code/continual-harness/server/app.py#L173)
- `video_frame_skip` — [`L174`](../../../../../raw/code/continual-harness/server/app.py#L174)
- `video_recording` — [`L171`](../../../../../raw/code/continual-harness/server/app.py#L171)
- `video_writer` — [`L170`](../../../../../raw/code/continual-harness/server/app.py#L170)

