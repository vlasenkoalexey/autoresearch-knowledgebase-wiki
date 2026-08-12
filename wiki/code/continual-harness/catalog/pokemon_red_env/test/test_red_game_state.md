---
title: 'Module: pokemon_red_env/test/test_red_game_state.py'
type: catalog
provenance: extracted
module: pokemon_red_env/test/test_red_game_state.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.test.test_red_game_state`/
symbols:
  check: check().
  main: main().
  test_overworld_states: test_overworld_states().
  test_battle_states: test_battle_states().
  test_dialog_states: test_dialog_states().
  test_menu_states: test_menu_states().
  test_zip_states: test_zip_states().
  test_init_zip: test_init_zip().
  load_emu: load_emu().
  OUTPUT_DIR: OUTPUT_DIR.
  load_emu_from_zip: load_emu_from_zip().
  SEP: SEP.
  run_pipeline: run_pipeline().
  validate_common: validate_common().
  STATES_DIR: STATES_DIR.
  save_output: save_output().
  ROM_PATH: ROM_PATH.
  REPO_ROOT: REPO_ROOT.
  print_state_text: print_state_text().
  INIT_ZIP: INIT_ZIP.
  FAILED: FAILED.
  PASSED: PASSED.
  THIS_DIR: THIS_DIR.
  PARTY_REQUIRED_KEYS: PARTY_REQUIRED_KEYS.
---
# Module: [`pokemon_red_env/test/test_red_game_state.py`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py)

## Functions
- `check(label, condition, detail="")` — [`L41`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L41)
- `load_emu(state_path)` — [`L66`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L66) — Create RedEmulator, load a .state file, tick 1 frame.
- `load_emu_from_zip(zip_path)` — [`L75`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L75) — Extract checkpoint.state from a backup zip and load it.
- `main()` — [`L619`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L619)
- `print_state_text(state_text, max_lines=120, indent=" ")` — [`L51`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L51)
- `run_pipeline(emu)` — [`L89`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L89) — Run the full mcp_get_game_state pipeline.
- `save_output(name, result)` — [`L94`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L94) — Save state_text and raw_state JSON for inspection.
- `test_battle_states()` — [`L228`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L228)
- `test_dialog_states()` — [`L334`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L334)
- `test_init_zip()` — [`L569`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L569)
- `test_menu_states()` — [`L409`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L409)
- `test_overworld_states()` — [`L164`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L164)
- `test_zip_states()` — [`L472`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L472)
- `validate_common(result, label, min_party=1, allow_title=False)` — [`L119`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L119) — Structural assertions that apply to every state.

## Module values
- `FAILED` — [`L37`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L37)
- `INIT_ZIP` — [`L27`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L27)
- `OUTPUT_DIR` — [`L28`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L28)
- `PARTY_REQUIRED_KEYS` — [`L113`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L113)
- `PASSED` — [`L36`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L36)
- `REPO_ROOT` — [`L24`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L24)
- `ROM_PATH` — [`L25`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L25)
- `SEP` — [`L38`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L38)
- `STATES_DIR` — [`L26`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L26)
- `THIS_DIR` — [`L23`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_game_state.py#L23)

