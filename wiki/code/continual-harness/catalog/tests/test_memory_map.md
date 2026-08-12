---
title: 'Module: tests/test_memory_map.py'
type: catalog
provenance: extracted
module: tests/test_memory_map.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_memory_map`/
symbols:
  test_door_behavior: test_door_behavior().
  test_upstairs_state_map_reading: test_upstairs_state_map_reading().
  test_simple_test_state_map_reading: test_simple_test_state_map_reading().
  TEST_STATES_DIR: TEST_STATES_DIR.
  test_house_state_map_reading: test_house_state_map_reading().
  test_truck_state_map_reading: test_truck_state_map_reading().
  format_map_data: format_map_data().
  print_map_data: print_map_data().
  emulator: emulator().
  test_map_data_validation: test_map_data_validation().
  test_map_reading_area_transitions: test_map_reading_area_transitions().
---
# Module: [`tests/test_memory_map.py`](../../../../../raw/code/continual-harness/tests/test_memory_map.py)

## Functions
- `emulator()` — [`L116`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L116) — Create and initialize an emulator instance
- `format_map_data(map_data, title="Map Data")` — [`L10`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L10) — Format the map data into a string using the agent's format
- `print_map_data(map_data, title="Map Data")` — [`L93`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L93) — Pretty print the map data and return the formatted string
- `test_door_behavior(emulator)` — [`L217`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L217) — Test that doors are properly identified and not marked as blocked
- `test_house_state_map_reading(emulator)` — [`L131`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L131) — Test map reading functionality in the house state
- `test_map_data_validation(emulator)` — [`L247`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L247) — Test validation of map data structure and content
- `test_map_reading_area_transitions(emulator)` — [`L401`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L401) — Test that map reading handles area transitions and new saves correctly
- `test_simple_test_state_map_reading(emulator)` — [`L446`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L446) — Test map reading functionality in the simple_test state (rival's bedroom)
- `test_truck_state_map_reading(emulator)` — [`L174`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L174) — Test map reading functionality in the truck state (game start)
- `test_upstairs_state_map_reading(emulator)` — [`L280`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L280) — Test map reading functionality in the upstairs state

## Module values
- `TEST_STATES_DIR` — [`L113`](../../../../../raw/code/continual-harness/tests/test_memory_map.py#L113)

