---
title: 'Module: tests/test_torchic_state.py'
type: catalog
provenance: extracted
module: tests/test_torchic_state.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_torchic_state`/
symbols:
  test_torchic_state_loading: test_torchic_state_loading().
  test_torchic_milestones: test_torchic_milestones().
  test_torchic_state_summary: test_torchic_state_summary().
  ServerManager.server_process: ServerManager#server_process.
  ServerManager.start_server: ServerManager#start_server().
  ServerManager.stop_server: ServerManager#stop_server().
  ServerManager: ServerManager#
  ServerManager.__init__: ServerManager#__init__().
  check_environment: check_environment().
---
# Module: [`tests/test_torchic_state.py`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py)

## Classes
### `ServerManager`
- def: [`tests/test_torchic_state.py:18`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L18)
- doc: Manages server startup and shutdown for tests
- signature: `class ServerManager:`
- members:
  - `start_server(self, state_file)` — [`L24`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L24) — Start the server with a specific state file
  - `stop_server(self)` — [`L53`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L53) — Stop the server cleanly
  - `server_process` — [`L22`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L22)
- protocol/private: `__init__`[`L21`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L21)
- used by: (3 test-only callers)

## Functions
- `check_environment()` — [`L76`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L76) — Check that required files exist
- `test_torchic_milestones()` — [`L140`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L140) — Test that milestones are correctly detected for torchic state
- `test_torchic_state_loading()` — [`L84`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L84) — Test that the torchic state loads correctly
- `test_torchic_state_summary()` — [`L202`](../../../../../raw/code/continual-harness/tests/test_torchic_state.py#L202) — Test that the torchic state provides a comprehensive summary

