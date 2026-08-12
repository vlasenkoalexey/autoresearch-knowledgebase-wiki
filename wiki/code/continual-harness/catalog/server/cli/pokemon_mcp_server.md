---
title: 'Module: server/cli/pokemon_mcp_server.py'
type: catalog
provenance: extracted
module: server/cli/pokemon_mcp_server.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `server.cli.pokemon_mcp_server`/
symbols:
  _post: _post().
  _run_combined_transport: _run_combined_transport().
  transport_mode: transport_mode.
  logger: logger.
  mcp: mcp.
  get_game_state: get_game_state().
  _MCP_PORT: _MCP_PORT.
  press_buttons: press_buttons().
  lookup_pokemon_info: lookup_pokemon_info().
  list_wiki_sources: list_wiki_sources().
  get_walkthrough: get_walkthrough().
  get_progress_summary: get_progress_summary().
  _MCP_HOST: _MCP_HOST.
  _TIMEOUT_SHORT: _TIMEOUT_SHORT.
  _TIMEOUT_MEDIUM: _TIMEOUT_MEDIUM.
  navigate_to: navigate_to().
  complete_direct_objective: complete_direct_objective().
  reflect: reflect().
  SERVER_URL: SERVER_URL.
---
# Module: [`server/cli/pokemon_mcp_server.py`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py)

## Functions
- `_post(path: str, body: dict | None = None, timeout: int = _TIMEOUT_MEDIUM)` — [`L59`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L59) — POST to the game server and return the JSON response (or an error dict).
- `_run_combined_transport()` — [`L353`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L353) — Run both SSE and Streamable HTTP for containerized CLI agents.
- `complete_direct_objective(objective_id: str, completion_notes: str = "", category: str = "")` — [`L288`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L288) — Mark the current direct objective as completed.
- `get_game_state()` — [`L75`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L75) — Get the current game state including player position, party, map, items, and screenshot.
- `get_progress_summary()` — [`L314`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L314) — Get comprehensive progress summary including milestones, completed objectives, and memory.
- `get_walkthrough(part: int)` — [`L244`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L244) — Get the official Bulbapedia walkthrough for Pokemon Emerald.
- `list_wiki_sources()` — [`L232`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L232) — List available Pokemon wiki sources and what they're good for.
- `lookup_pokemon_info(topic: str, source: str = "bulbapedia")` — [`L211`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L211) — Look up information about Pokemon Emerald from trusted wiki sources.
- `navigate_to(x: int, y: int, variance: str = "none", reason: str = "", consider_npcs: bool = True, blocked_coords: Optional[List[List[int]]] = None)` — [`L176`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L176) — Automatically pathfind and move to a specific coordinate on the current map using A* algorithm.
- `press_buttons(buttons: List[str], speed: str = "normal", hold_frames: Optional[int] = None, release_frames: Optional[int] = None, reasoning: str = "", source: str = "", metadata: Optional[Dict[str, Any]] = None)` — [`L105`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L105) — Press buttons on the Game Boy Advance emulator with optional speed control.
- `reflect(situation: str = "Agent requested reflection")` — [`L330`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L330) — Return context data for self-reflection on current progress.

## Module values
- `SERVER_URL` — [`L46`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L46)
- `_MCP_HOST` — [`L51`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L51)
- `_MCP_PORT` — [`L50`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L50)
- `_TIMEOUT_MEDIUM` — [`L56`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L56)
- `_TIMEOUT_SHORT` — [`L55`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L55)
- `logger` — [`L43`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L43)
- `mcp` — [`L53`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L53)
- `transport_mode` — [`L387`](../../../../../../raw/code/continual-harness/server/cli/pokemon_mcp_server.py#L387)

