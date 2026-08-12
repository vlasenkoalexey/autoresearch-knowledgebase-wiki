---
title: 'Module: pokemon_red_env/utils/red_metatile_behavior.py'
type: catalog
provenance: extracted
module: pokemon_red_env/utils/red_metatile_behavior.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.utils.red_metatile_behavior`/
symbols:
  RedMetatileBehavior: RedMetatileBehavior#
  BEHAVIOR_COLLISION.BEHAVIOR_COLLISION: BEHAVIOR_COLLISION.BEHAVIOR_COLLISION.
  HIDDEN_SYMBOL_TO_BEHAVIOR.HIDDEN_SYMBOL_TO_BEHAVIOR: HIDDEN_SYMBOL_TO_BEHAVIOR.HIDDEN_SYMBOL_TO_BEHAVIOR.
  RedMetatileBehavior.IMPASSABLE: RedMetatileBehavior#IMPASSABLE.
  RedMetatileBehavior.NORMAL: RedMetatileBehavior#NORMAL.
  RedMetatileBehavior.LADDER: RedMetatileBehavior#LADDER.
  RedMetatileBehavior.BOOKSHELF: RedMetatileBehavior#BOOKSHELF.
  RedMetatileBehavior.TALL_GRASS: RedMetatileBehavior#TALL_GRASS.
  RedMetatileBehavior.DEEP_WATER: RedMetatileBehavior#DEEP_WATER.
  RedMetatileBehavior.JUMP_EAST: RedMetatileBehavior#JUMP_EAST.
  RedMetatileBehavior.JUMP_WEST: RedMetatileBehavior#JUMP_WEST.
  RedMetatileBehavior.JUMP_NORTH: RedMetatileBehavior#JUMP_NORTH.
  RedMetatileBehavior.JUMP_SOUTH: RedMetatileBehavior#JUMP_SOUTH.
  RedMetatileBehavior.COUNTER: RedMetatileBehavior#COUNTER.
  RedMetatileBehavior.PC: RedMetatileBehavior#PC.
  RedMetatileBehavior.TELEVISION: RedMetatileBehavior#TELEVISION.
  RedMetatileBehavior.TRASH_CAN: RedMetatileBehavior#TRASH_CAN.
  RedMetatileBehavior.BLUEPRINT: RedMetatileBehavior#BLUEPRINT.
  RedMetatileBehavior.NON_ANIMATED_DOOR: RedMetatileBehavior#NON_ANIMATED_DOOR.
  RedMetatileBehavior.CRACKED_FLOOR_HOLE: RedMetatileBehavior#CRACKED_FLOOR_HOLE.
  RedMetatileBehavior.QUESTIONNAIRE: RedMetatileBehavior#QUESTIONNAIRE.
  RedMetatileBehavior.WARP_CARPET: RedMetatileBehavior#WARP_CARPET.
  RedMetatileBehavior.WARP_PAD: RedMetatileBehavior#WARP_PAD.
  RedMetatileBehavior.CUT_TREE: RedMetatileBehavior#CUT_TREE.
  RedMetatileBehavior.SPINNER: RedMetatileBehavior#SPINNER.
  RedMetatileBehavior.POKE_BALL: RedMetatileBehavior#POKE_BALL.
---
# Module: [`pokemon_red_env/utils/red_metatile_behavior.py`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py)

## Classes
### `RedMetatileBehavior`  ·  implements/extends IntEnum
- def: [`pokemon_red_env/utils/red_metatile_behavior.py:28`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L28) — documented in [pokemon_red_env-utils-red_metatile_behavior](../../../concepts/pokemon_red_env-utils-red_metatile_behavior.md)
- doc: Gen 1 (pokered) tile behavior codes for processed_map JSON raw_tile field.
- signature: `class RedMetatileBehavior(IntEnum):`
- members:
  - `BLUEPRINT` — [`L58`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L58)
  - `BOOKSHELF` — [`L56`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L56)
  - `COUNTER` — [`L52`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L52)
  - `CRACKED_FLOOR_HOLE` — [`L51`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L51)
  - `CUT_TREE` — [`L74`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L74)
  - `DEEP_WATER` — [`L44`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L44)
  - `IMPASSABLE` — [`L71`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L71)
  - `JUMP_EAST` — [`L45`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L45)
  - `JUMP_NORTH` — [`L47`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L47)
  - `JUMP_SOUTH` — [`L48`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L48)
  - `JUMP_WEST` — [`L46`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L46)
  - `LADDER` — [`L50`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L50)
  - `NON_ANIMATED_DOOR` — [`L49`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L49)
  - `NORMAL` — [`L42`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L42)
  - `PC` — [`L53`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L53)
  - `POKE_BALL` — [`L67`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L67)
  - `QUESTIONNAIRE` — [`L55`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L55)
  - `SPINNER` — [`L65`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L65)
  - `TALL_GRASS` — [`L43`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L43)
  - `TELEVISION` — [`L54`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L54)
  - `TRASH_CAN` — [`L57`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L57)
  - `WARP_CARPET` — [`L61`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L61)
  - `WARP_PAD` — [`L63`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L63)
- used by: [`main`](map_preprocess.md#main), [`BEHAVIOR_COLLISION`](red_metatile_behavior.md#BEHAVIOR_COLLISION.BEHAVIOR_COLLISION), [`_GRID_SYMBOL_TO_BEHAVIOR`](map_preprocess.md#_GRID_SYMBOL_TO_BEHAVIOR._GRID_SYMBOL_TO_BEHAVIOR), [`get_whole_map_data`](../red_map_reader.md#RedMapReader.get_whole_map_data), [`HIDDEN_SYMBOL_TO_BEHAVIOR`](red_metatile_behavior.md#HIDDEN_SYMBOL_TO_BEHAVIOR.HIDDEN_SYMBOL_TO_BEHAVIOR), [`_can_move_to`](../../utils/mapping/pathfinding.md#Pathfinder._can_move_to), [`_get_behavior_enum`](../../utils/mapping/map_formatter.md#_get_behavior_enum)

## Module values
- `BEHAVIOR_COLLISION` — [`L81`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L81)
- `HIDDEN_SYMBOL_TO_BEHAVIOR` — [`L114`](../../../../../../raw/code/continual-harness/pokemon_red_env/utils/red_metatile_behavior.py#L114)

