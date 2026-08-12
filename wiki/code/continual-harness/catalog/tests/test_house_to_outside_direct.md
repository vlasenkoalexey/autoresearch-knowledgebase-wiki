---
title: 'Module: tests/test_house_to_outside_direct.py'
type: catalog
provenance: extracted
module: tests/test_house_to_outside_direct.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_house_to_outside_direct`/TestHouseToOutsideDirectTransition#
symbols:
  TestHouseToOutsideDirectTransition.emulator: emulator().
  TestHouseToOutsideDirectTransition.test_walk_and_map_transition: test_walk_and_map_transition().
  TestHouseToOutsideDirectTransition._test_outside_map: _test_outside_map().
  TestHouseToOutsideDirectTransition.test_house_map_baseline: test_house_map_baseline().
  TestHouseToOutsideDirectTransition._validate_map_structure: _validate_map_structure().
  TestHouseToOutsideDirectTransition._analyze_map_for_exits: _analyze_map_for_exits().
  TestHouseToOutsideDirectTransition: ''
---
# Module: [`tests/test_house_to_outside_direct.py`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py)

## Classes
### `TestHouseToOutsideDirectTransition`
- def: [`tests/test_house_to_outside_direct.py:13`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L13)
- signature: `class TestHouseToOutsideDirectTransition:`
- members:
  - `_analyze_map_for_exits(self, map_data, player_pos)` — [`L133`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L133) — Analyze house map to find potential exits
  - `_test_outside_map(self, emulator, location, position)` — [`L107`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L107) — Test the outside map after successful transition
  - `_validate_map_structure(self, map_data, location_name, area_type)` — [`L159`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L159) — Validate map structure
  - `emulator(self)` — [`L16`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L16) — Create and initialize emulator
  - `test_house_map_baseline(self, emulator)` — [`L28`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L28) — Test that house map reads correctly as baseline
  - `test_walk_and_map_transition(self, emulator)` — [`L54`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_direct.py#L54) — Test walking outside and check if map transitions work
- uses (calls/refs, reference-scoped): [`MetatileBehavior`](../pokemon_env/enums.md#MetatileBehavior), [`initialize`](../pokemon_env/emulator.md#EmeraldEmulator.initialize), [`EmeraldEmulator`](../pokemon_env/emulator.md#EmeraldEmulator), [`stop`](../pokemon_env/emulator.md#EmeraldEmulator.stop)  (1 test-only)

