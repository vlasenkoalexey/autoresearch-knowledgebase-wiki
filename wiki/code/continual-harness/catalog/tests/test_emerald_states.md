---
title: 'Module: tests/test_emerald_states.py'
type: catalog
provenance: extracted
module: tests/test_emerald_states.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_emerald_states`/
symbols:
  run_state: run_state().
  main: main().
  REPO_ROOT: REPO_ROOT.
  STATE_DIRS: STATE_DIRS.
  ROM_PATH: ROM_PATH.
  _json_safe: _json_safe().
  OUTPUT_DIR: OUTPUT_DIR.
  collect_states: collect_states().
  THIS_DIR: THIS_DIR.
---
# Module: [`tests/test_emerald_states.py`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py)

## Functions
- `_json_safe(obj)` — [`L40`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L40) — Recursively convert non-serialisable objects to JSON-safe equivalents.
- `collect_states()` — [`L142`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L142) — Return sorted list of pathlib.Path for all .state files in STATE_DIRS.
- `main()` — [`L151`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L151)
- `run_state(state_path: pathlib.Path, rom_path: pathlib.Path, out_dir: pathlib.Path)` — [`L69`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L69)

## Module values
- `OUTPUT_DIR` — [`L29`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L29)
- `REPO_ROOT` — [`L27`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L27)
- `ROM_PATH` — [`L28`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L28)
- `STATE_DIRS` — [`L31`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L31)
- `THIS_DIR` — [`L26`](../../../../../raw/code/continual-harness/tests/test_emerald_states.py#L26)

