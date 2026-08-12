---
title: 'Module: utils/mapping/ascii_map_loader.py'
type: catalog
provenance: extracted
module: utils/mapping/ascii_map_loader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.mapping.ascii_map_loader`/
symbols:
  ascii_to_metatiles: ascii_to_metatiles().
  get_effective_map_name: get_effective_map_name().
  get_override: get_override().
  CONDITIONAL_SELECTORS.CONDITIONAL_SELECTORS: CONDITIONAL_SELECTORS.CONDITIONAL_SELECTORS.
  _select_petalburg_gym: _select_petalburg_gym().
  has_override: has_override().
  MAP_OVERRIDES.MAP_OVERRIDES: MAP_OVERRIDES.MAP_OVERRIDES.
  logger: logger.
---
# Module: [`utils/mapping/ascii_map_loader.py`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py)

## Functions
- `_select_petalburg_gym(badge_count: int = 0, **kwargs)` — [`L426`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L426) — Return lobby variant if < 4 badges, else None for default.
- `ascii_to_metatiles(ascii_map: str, map_name: str = "")` — [`L463`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L463) — Convert ASCII map to metatile format for pathfinding.
- `get_effective_map_name(map_name: str, badge_count: int = 0, **kwargs)` — [`L444`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L444) — Get the effective map name after applying conditional selection.
- `get_override(map_name: str)` — [`L453`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L453) — Get override data for a map, if any exists.
- `has_override(map_name: str)` — [`L458`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L458) — Check if any override exists for the map.

## Module values
- `CONDITIONAL_SELECTORS` — [`L435`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L435)
- `MAP_OVERRIDES` — [`L30`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L30)
- `logger` — [`L19`](../../../../../../raw/code/continual-harness/utils/mapping/ascii_map_loader.py#L19)

