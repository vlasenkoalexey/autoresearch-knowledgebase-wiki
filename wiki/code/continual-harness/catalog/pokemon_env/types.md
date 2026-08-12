---
title: 'Module: pokemon_env/types.py'
type: catalog
provenance: extracted
module: pokemon_env/types.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_env.types`/PokemonData#
symbols:
  PokemonData.status_name: status_name().
  PokemonData.status: status.
  PokemonData.current_hp: current_hp.
  PokemonData.max_hp: max_hp.
  PokemonData.type1: type1.
  PokemonData.type2: type2.
  PokemonData.species_name: species_name.
  PokemonData.level: level.
  PokemonData.is_asleep: is_asleep().
  PokemonData: ''
  PokemonData.moves: moves.
  PokemonData.move_pp: move_pp.
  PokemonData.nickname: nickname.
  PokemonData.species_id: species_id.
  PokemonData.trainer_id: trainer_id.
  PokemonData.experience: experience.
  PokemonData.is_egg: is_egg.
---
# Module: [`pokemon_env/types.py`](../../../../../raw/code/continual-harness/pokemon_env/types.py)

## Classes
### `PokemonData`
- def: [`pokemon_env/types.py:6`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L6)
- doc: Complete Pokemon data structure for Emerald
- signature: `class PokemonData:`
- members:
  - `is_asleep(self)` — [`L24`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L24) — Check if the Pokémon is asleep
  - `status_name(self)` — [`L29`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L29) — Return a human-readable status name
  - `current_hp` — [`L10`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L10)
  - `experience` — [`L20`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L20)
  - `is_egg` — [`L21`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L21)
  - `level` — [`L12`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L12)
  - `max_hp` — [`L11`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L11)
  - `move_pp` — [`L17`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L17)
  - `moves` — [`L16`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L16)
  - `nickname` — [`L19`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L19)
  - `species_id` — [`L8`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L8)
  - `species_name` — [`L9`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L9)
  - `status` — [`L13`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L13)
  - `trainer_id` — [`L18`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L18)
  - `type1` — [`L14`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L14)
  - `type2` — [`L15`](../../../../../raw/code/continual-harness/pokemon_env/types.py#L15)
- uses (calls/refs, reference-scoped): [`PokemonType`](enums.md#PokemonType), [`StatusCondition`](enums.md#StatusCondition), [`BURN`](enums.md#StatusCondition.BURN), [`FREEZE`](enums.md#StatusCondition.FREEZE), [`PARALYSIS`](enums.md#StatusCondition.PARALYSIS), [`POISON`](enums.md#StatusCondition.POISON), [`is_asleep`](enums.md#StatusCondition.is_asleep)
- used by: [`get_comprehensive_state`](memory_reader.md#PokemonEmeraldReader.get_comprehensive_state), [`read_comprehensive_battle_info`](memory_reader.md#PokemonEmeraldReader.read_comprehensive_battle_info), [`parse_pokemon`](emerald_utils.md#parse_pokemon), [`read_party_pokemon`](memory_reader.md#PokemonEmeraldReader.read_party_pokemon), [`get_party_pokemon`](emulator.md#EmeraldEmulator.get_party_pokemon), [`_scan_for_opponent_pokemon`](memory_reader.md#PokemonEmeraldReader._scan_for_opponent_pokemon), [`get_game_progress_context`](memory_reader.md#PokemonEmeraldReader.get_game_progress_context)

