---
title: 'Module: tests/test_fps_adjustment_pytest.py'
type: catalog
provenance: extracted
module: tests/test_fps_adjustment_pytest.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_fps_adjustment_pytest`/
symbols:
  test_fps_adjustment: test_fps_adjustment().
  ServerManager.server_process: ServerManager#server_process.
  ServerManager.start_server: ServerManager#start_server().
  ServerManager.stop_server: ServerManager#stop_server().
  TEST_CASES: TEST_CASES.
  ServerManager: ServerManager#
  check_fps: check_fps().
  ServerManager.__init__: ServerManager#__init__().
  check_environment: check_environment().
  test_fps_adjustment_summary: test_fps_adjustment_summary().
---
# Module: [`tests/test_fps_adjustment_pytest.py`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py)

## Classes
### `ServerManager`
- def: [`tests/test_fps_adjustment_pytest.py:48`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L48)
- doc: Manages server startup and shutdown for tests
- signature: `class ServerManager:`
- members:
  - `start_server(self, state_file)` — [`L54`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L54) — Start the server with a specific state file
  - `stop_server(self)` — [`L83`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L83) — Stop the server cleanly
  - `server_process` — [`L52`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L52)
- protocol/private: `__init__`[`L51`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L51)
- used by: (1 test-only callers)

## Functions
- `check_environment()` — [`L136`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L136) — Check that we're in the right environment before running tests
- `check_fps(expected_fps, test_name)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L105) — Check if the current FPS matches the expected value
- `test_fps_adjustment(test_case)` — [`L155`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L155) — Test FPS adjustment for a specific state
- `test_fps_adjustment_summary()` — [`L194`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L194) — Test summary - this will run after all individual tests

## Module values
- `TEST_CASES` — [`L25`](../../../../../raw/code/continual-harness/tests/test_fps_adjustment_pytest.py#L25)

