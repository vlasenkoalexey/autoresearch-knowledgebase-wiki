---
title: 'Module: tests/test_server_map_validation.py'
type: catalog
provenance: extracted
module: tests/test_server_map_validation.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_server_map_validation`/
symbols:
  ServerMapTester.start_server: ServerMapTester#start_server().
  ServerMapTester.server_process: ServerMapTester#server_process.
  ServerMapTester.stop_server: ServerMapTester#stop_server().
  save_reference_map: save_reference_map().
  server_tester: server_tester().
  ServerMapTester.server_url: ServerMapTester#server_url.
  ServerMapTester.get_map_data: ServerMapTester#get_map_data().
  ServerMapTester.execute_actions: ServerMapTester#execute_actions().
  TestServerMapValidation.test_house_state_map: TestServerMapValidation#test_house_state_map().
  TestServerMapValidation.test_upstairs_state_map: TestServerMapValidation#test_upstairs_state_map().
  TestServerMapValidation.test_house_to_outside_transition: TestServerMapValidation#test_house_to_outside_transition().
  TestServerMapValidation.test_regression_against_references: TestServerMapValidation#test_regression_against_references().
  ServerMapTester: ServerMapTester#
  ServerMapTester.port: ServerMapTester#port.
  compare_with_reference: compare_with_reference().
  ServerMapTester.__init__: ServerMapTester#__init__().
  TestServerMapValidation: TestServerMapValidation#
---
# Module: [`tests/test_server_map_validation.py`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py)

## Classes
### `ServerMapTester`
- def: [`tests/test_server_map_validation.py:17`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L17)
- doc: Helper class for testing server-based map reading
- signature: `class ServerMapTester:`
- members:
  - `execute_actions(self, actions)` — [`L81`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L81) — Execute a sequence of actions
  - `get_map_data(self)` — [`L66`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L66) — Get current map data from server
  - `start_server(self, state_file)` — [`L25`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L25) — Start server with a specific state file
  - `stop_server(self)` — [`L55`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L55) — Stop the server process
  - `port` — [`L21`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L21)
  - `server_process` — [`L23`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L23)
  - `server_url` — [`L22`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L22)
- protocol/private: `__init__`[`L20`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L20)
- used by: (1 test-only callers)

### `TestServerMapValidation`
- def: [`tests/test_server_map_validation.py:165`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L165)
- doc: Test server-based map reading for different scenarios
- signature: `class TestServerMapValidation:`
- members:
  - `test_house_state_map(self, server_tester)` — [`L168`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L168) — Test map reading from house state
  - `test_house_to_outside_transition(self, server_tester)` — [`L224`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L224) — Test area transition from house to outside
  - `test_regression_against_references(self, server_tester)` — [`L265`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L265) — Test current maps against saved references
  - `test_upstairs_state_map(self, server_tester)` — [`L186`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L186) — Test map reading from upstairs state
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `compare_with_reference(current_map, reference_file)` — [`L125`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L125) — Compare current map with saved reference
- `save_reference_map(location_name, map_data, reference_dir)` — [`L101`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L101) — Save map data as reference for future comparisons
- `server_tester()` — [`L94`](../../../../../raw/code/continual-harness/tests/test_server_map_validation.py#L94) — Pytest fixture providing a server tester instance

