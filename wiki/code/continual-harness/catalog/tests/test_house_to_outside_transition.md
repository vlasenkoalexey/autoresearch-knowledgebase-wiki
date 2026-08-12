---
title: 'Module: tests/test_house_to_outside_transition.py'
type: catalog
provenance: extracted
module: tests/test_house_to_outside_transition.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_house_to_outside_transition`/
symbols:
  TestHouseToOutsideTransition.server_process: TestHouseToOutsideTransition#server_process.
  SERVER_URL: SERVER_URL.
  TestHouseToOutsideTransition.test_initial_house_map: TestHouseToOutsideTransition#test_initial_house_map().
  TestHouseToOutsideTransition.test_walk_outside_transition: TestHouseToOutsideTransition#test_walk_outside_transition().
  TestHouseToOutsideTransition._format_server_map_data: TestHouseToOutsideTransition#_format_server_map_data().
  TestHouseToOutsideTransition._validate_outside_map: TestHouseToOutsideTransition#_validate_outside_map().
  SERVER_PORT: SERVER_PORT.
  TestHouseToOutsideTransition.setup_class: TestHouseToOutsideTransition#setup_class().
  TestHouseToOutsideTransition.teardown_class: TestHouseToOutsideTransition#teardown_class().
  TestHouseToOutsideTransition._maps_are_similar: TestHouseToOutsideTransition#_maps_are_similar().
  TestHouseToOutsideTransition: TestHouseToOutsideTransition#
---
# Module: [`tests/test_house_to_outside_transition.py`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py)

## Classes
### `TestHouseToOutsideTransition`
- def: [`tests/test_house_to_outside_transition.py:22`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L22)
- signature: `class TestHouseToOutsideTransition:`
- members:
  - `_format_server_map_data(self, server_tiles, title="Map Data")` — [`L181`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L181) — Convert server tile format to the same format as test_memory_map.py
  - `_maps_are_similar(self, actual, expected)` — [`L208`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L208) — Check if two maps are similar (allowing for minor differences)
  - `_validate_outside_map(self, map_tiles, location_name)` — [`L229`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L229) — Validate that outside map looks reasonable
  - `setup_class(cls)` — [`L25`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L25) — Start server with house.state before running tests
  - `teardown_class(cls)` — [`L65`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L65) — Stop server after all tests
  - `test_initial_house_map(self)` — [`L73`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L73) — Test that the initial house map matches the expected ground truth
  - `test_walk_outside_transition(self)` — [`L112`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L112) — Test walking outside from house and verify map is correct
  - `server_process` — [`L38`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L38)
- uses (calls/refs, reference-scoped): [`MetatileBehavior`](../pokemon_env/enums.md#MetatileBehavior)  (3 test-only)

## Module values
- `SERVER_PORT` — [`L19`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L19)
- `SERVER_URL` — [`L20`](../../../../../raw/code/continual-harness/tests/test_house_to_outside_transition.py#L20)

