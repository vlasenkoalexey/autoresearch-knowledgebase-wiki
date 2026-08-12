---
title: 'Module: pokemon_env/utils.py'
type: catalog
provenance: extracted
module: pokemon_env/utils.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_env.utils`/
symbols:
  is_passable_behavior: is_passable_behavior().
  get_type_effectiveness: get_type_effectiveness().
  is_encounter_behavior: is_encounter_behavior().
  is_surfable_behavior: is_surfable_behavior().
  get_pokemon_type_names: get_pokemon_type_names().
  format_time: format_time().
  format_money: format_money().
---
# Module: [`pokemon_env/utils.py`](../../../../../raw/code/continual-harness/pokemon_env/utils.py)

## Functions
- `format_money(amount: int)` — [`L271`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L271) — Format money amount with commas
- `format_time(hours: int, minutes: int, seconds: int)` — [`L256`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L256) — Format game time in a human-readable format
- `get_pokemon_type_names(type1: PokemonType, type2: Optional[PokemonType] = None)` — [`L284`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L284) — Get formatted type names for a Pokemon
- `get_type_effectiveness(attacking_type: PokemonType, defending_type: PokemonType)` — [`L91`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L91) — Calculate type effectiveness between two Pokemon types
- `is_encounter_behavior(behavior: MetatileBehavior)` — [`L46`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L46) — Check if a metatile behavior can trigger wild Pokemon encounters
- `is_passable_behavior(behavior: MetatileBehavior)` — [`L9`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L9) — Check if a metatile behavior allows the player to walk on it
- `is_surfable_behavior(behavior: MetatileBehavior)` — [`L69`](../../../../../raw/code/continual-harness/pokemon_env/utils.py#L69) — Check if a metatile behavior allows surfing

