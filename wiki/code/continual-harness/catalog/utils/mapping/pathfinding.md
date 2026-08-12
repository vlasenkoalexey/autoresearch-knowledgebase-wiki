---
title: 'Module: utils/mapping/pathfinding.py'
type: catalog
provenance: extracted
module: utils/mapping/pathfinding.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.pathfinding`/
symbols:
  logger: logger.
  Pathfinder.find_path: Pathfinder#find_path().
  Pathfinder._astar: Pathfinder#_astar().
  Pathfinder._get_neighbors: Pathfinder#_get_neighbors().
  Pathfinder._reconstruct_path: Pathfinder#_reconstruct_path().
  Node.x: Node#x.
  Node.y: Node#y.
  Pathfinder._generate_variance_candidates: Pathfinder#_generate_variance_candidates().
  Pathfinder._can_move_to: Pathfinder#_can_move_to().
  Node.__post_init__: Node#__post_init__().
  Node.__lt__: Node#__lt__().
  Pathfinder: Pathfinder#
  Node: Node#
  Node.parent: Node#parent.
  Node.g_cost: Node#g_cost.
  Node.h_cost: Node#h_cost.
  Node.__eq__: Node#__eq__().
  Node.__hash__: Node#__hash__().
  find_path: find_path().
  Pathfinder._get_blocked_positions: Pathfinder#_get_blocked_positions().
  Node.f_cost: Node#f_cost.
  Pathfinder._path_to_buttons: Pathfinder#_path_to_buttons().
  Pathfinder._find_nearest_reachable: Pathfinder#_find_nearest_reachable().
  Pathfinder._enumerate_prefix_paths: Pathfinder#_enumerate_prefix_paths().
  Pathfinder._build_tile_connectivity: Pathfinder#_build_tile_connectivity().
  Pathfinder._is_tile_blocked: Pathfinder#_is_tile_blocked().
  Pathfinder.tile_connectivity: Pathfinder#tile_connectivity.
  Pathfinder._extract_map_data: Pathfinder#_extract_map_data().
  Pathfinder._heuristic: Pathfinder#_heuristic().
  VARIANCE_TO_STEPS: VARIANCE_TO_STEPS.
  GRASS_TILE_COST_MULTIPLIER: GRASS_TILE_COST_MULTIPLIER.
  Pathfinder.allow_diagonal: Pathfinder#allow_diagonal.
  Pathfinder._get_warp_positions: Pathfinder#_get_warp_positions().
  Pathfinder.__init__: Pathfinder#__init__().
  Pathfinder.collision_map: Pathfinder#collision_map.
  Pathfinder._get_npc_positions: Pathfinder#_get_npc_positions().
  Pathfinder._simple_path: Pathfinder#_simple_path().
---
# Module: [`utils/mapping/pathfinding.py`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py)

## Classes
### `Node`
- def: [`utils/mapping/pathfinding.py:36`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L36)
- doc: Represents a position in the pathfinding grid.
- signature: `class Node:`
- members:
  - `__lt__(self, other)` — [`L49`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L49) — Comparison for heapq tie-breaking.
  - `f_cost` — [`L43`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L43)
  - `g_cost` — [`L41`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L41)
  - `h_cost` — [`L42`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L42)
  - `parent` — [`L44`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L44)
  - `x` — [`L39`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L39)
  - `y` — [`L40`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L40)
- protocol/private: `__eq__`[`L64`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L64), `__hash__`[`L67`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L67), `__post_init__`[`L46`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L46)
- used by: [`find_path`](pathfinding.md#Pathfinder.find_path), [`_astar`](pathfinding.md#Pathfinder._astar), [`_get_neighbors`](pathfinding.md#Pathfinder._get_neighbors), [`_reconstruct_path`](pathfinding.md#Pathfinder._reconstruct_path)

### `Pathfinder`
- def: [`utils/mapping/pathfinding.py:71`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L71)
- doc: A* pathfinding implementation for Pokemon Emerald navigation.
- signature: `class Pathfinder:`
- members:
  - `__init__(self, collision_map: Optional[Dict] = None, allow_diagonal: bool = False)` — [`L78`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L78) — Initialize the pathfinder.
  - `_astar(self, start: Tuple[int, int], goal: Tuple[int, int], blocked: Set[Tuple[int, int]], map_data: Dict, max_distance: int)` — [`L1165`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1165) — A* pathfinding algorithm implementation.
  - `_build_tile_connectivity(self, map_data: Dict)` — [`L380`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L380) — Build a connectivity map showing which directions are valid from each tile.
  - `_can_move_to(self, from_pos: Tuple[int, int], to_pos: Tuple[int, int], map_data: Dict)` — [`L824`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L824) — Check if movement from from_pos to to_pos is valid.
  - `_enumerate_prefix_paths(self, start: Tuple[int, int], blocked: Set[Tuple[int, int]], map_data: Dict, steps_required: int, max_prefixes: int = 256)` — [`L1483`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1483) — Enumerate walkable position sequences originating from start with a fixed number of steps.
  - `_extract_map_data(self, game_state: Dict)` — [`L349`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L349) — Extract map data from game state. ONLY returns porymap data - no fallbacks.
  - `_find_nearest_reachable(self, start: Tuple[int, int], goal: Tuple[int, int], blocked: Set[Tuple[int, int]], map_data: Dict, max_distance: int = 10)` — [`L1309`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1309) — Find the nearest reachable position to the goal.
  - `_generate_variance_candidates(self, start: Tuple[int, int], goal: Tuple[int, int], blocked: Set[Tuple[int, int]], map_data: Dict, max_distance: int, variance_steps: int, base_path_buttons: List[str], max_variants: int = 8)` — [`L1408`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1408) — Generate alternative button sequences that reach the goal but differ in their initial moves.
  - `_get_blocked_positions(self, game_state: Dict, map_data: Dict, start_pos: Optional[Tuple[int, int]] = None, goal_pos: Optional[Tuple[int, int]] = None, consider_npcs: bool = False)` — [`L414`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L414) — Get all blocked positions on the current map.
  - `_get_neighbors(self, node: Node, blocked: Set[Tuple[int, int]])` — [`L1260`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1260) — Get valid neighbor positions for a node using connectivity map.
  - `_get_npc_positions(self, game_state: Dict)` — [`L768`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L768) — Get positions of all NPCs on the current map.
  - `_get_warp_positions(self, game_state: Dict, map_data: Dict)` — [`L786`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L786) — Get positions of warps (doors, stairs, transitions) which are always walkable.
  - `_heuristic(self, pos1: Tuple[int, int], pos2: Tuple[int, int])` — [`L1295`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1295) — Calculate heuristic distance (Manhattan distance for grid movement).
  - `_is_tile_blocked(self, tile)` — [`L751`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L751) — Check if a tile is blocked based on its properties.
  - `_path_to_buttons(self, path: List[Tuple[int, int]])` — [`L1529`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1529) — Convert a path of positions to button commands.
  - `_reconstruct_path(self, node: Node)` — [`L1299`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1299) — Reconstruct the path from start to goal.
  - `_simple_path(self, start: Tuple[int, int], goal: Tuple[int, int])` — [`L1553`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1553) — Simple straight-line path when no map data is available.
  - `find_path(self, start: Tuple[int, int], goal: Tuple[int, int], game_state: Dict, max_distance: int = 150, variance: Optional[str] = None, consider_npcs: bool = False, allow_partial: bool = True, blocked_coords: Optional[List[Tuple[int, int]]] = None)` — [`L90`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L90) — Find a path from start to goal using A* algorithm.
  - `allow_diagonal` — [`L87`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L87)
  - `collision_map` — [`L86`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L86)
  - `tile_connectivity` — [`L88`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L88)
- uses (calls/refs, reference-scoped): [`MetatileBehavior`](../../pokemon_env/enums.md#MetatileBehavior), [`RedMetatileBehavior`](../../pokemon_red_env/utils/red_metatile_behavior.md#RedMetatileBehavior), [`logger`](pathfinding.md#logger), [`x`](pathfinding.md#Node.x), [`y`](pathfinding.md#Node.y), [`is_tile_walkable`](map_formatter.md#is_tile_walkable), [`Node`](pathfinding.md#Node), [`parent`](pathfinding.md#Node.parent), [`g_cost`](pathfinding.md#Node.g_cost), [`h_cost`](pathfinding.md#Node.h_cost), [`f_cost`](pathfinding.md#Node.f_cost), [`GRASS_TILE_COST_MULTIPLIER`](pathfinding.md#GRASS_TILE_COST_MULTIPLIER), [`VARIANCE_TO_STEPS`](pathfinding.md#VARIANCE_TO_STEPS)
- used by: [`navigate_to_direct`](../../server/game_tools.md#navigate_to_direct), [`find_path`](pathfinding.md#find_path), [`pathfinder`](../../server/game_tools.md#pathfinder)  (2 test-only)

## Functions
- `find_path(start: Tuple[int, int], goal: Tuple[int, int], game_state: Dict, max_distance: int = 150, variance: Optional[str] = None, consider_npcs: bool = False, allow_partial: bool = True)` — [`L1576`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L1576) — Find a path from start to goal position.

## Module values
- `GRASS_TILE_COST_MULTIPLIER` — [`L32`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L32)
- `VARIANCE_TO_STEPS` — [`L24`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L24)
- `logger` — [`L21`](../../../../../../raw/code/continual-harness/utils/mapping/pathfinding.py#L21)

