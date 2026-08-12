---
title: 'Module: pokemon_red_env/test/test_red_state_formatter.py'
type: catalog
provenance: extracted
module: pokemon_red_env/test/test_red_state_formatter.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.test.test_red_state_formatter`/
symbols:
  check: check().
  main: main().
  test_format_map_info_visual_map_fallback: test_format_map_info_visual_map_fallback().
  test_with_real_states: test_with_real_states().
  make_red_full_state: make_red_full_state().
  test_format_map_info_no_crash: test_format_map_info_no_crash().
  test_format_map_info_has_location: test_format_map_info_has_location().
  test_format_map_info_full_map: test_format_map_info_full_map().
  test_format_map_info_no_visual_map: test_format_map_info_no_visual_map().
  SEP: SEP.
  test_format_map_info_has_player_position: test_format_map_info_has_player_position().
  test_format_map_info_title_sequence: test_format_map_info_title_sequence().
  test_format_state_for_llm_no_crash: test_format_state_for_llm_no_crash().
  test_format_state_for_llm_visual_map_fallback: test_format_state_for_llm_visual_map_fallback().
  test_format_state_for_llm_battle_state: test_format_state_for_llm_battle_state().
  test_format_state_for_llm_dialog_state: test_format_state_for_llm_dialog_state().
  test_format_state_for_llm_no_map_at_all: test_format_state_for_llm_no_map_at_all().
  test_format_state_for_llm_contains_key_info: test_format_state_for_llm_contains_key_info().
  test_format_state_for_llm_contains_full_map: test_format_state_for_llm_contains_full_map().
  test_format_state_for_llm_gen1_party_fields: test_format_state_for_llm_gen1_party_fields().
  make_red_map_info: make_red_map_info().
  REPO: REPO.
  make_red_player_data: make_red_player_data().
  test_format_map_info_empty_map: test_format_map_info_empty_map().
  print_formatted_map: print_formatted_map().
  print_formatted_state: print_formatted_state().
  FAILED: FAILED.
  PASSED: PASSED.
  SAMPLE_VISUAL_MAP: SAMPLE_VISUAL_MAP.
  CELL_SYMBOLS: CELL_SYMBOLS.
---
# Module: [`pokemon_red_env/test/test_red_state_formatter.py`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py)

## Functions
- `check(label, condition, detail="")` — [`L32`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L32)
- `main()` — [`L617`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L617)
- `make_red_full_state(visual_map=None, map_source=None, location="OaksLab", game_state="overworld", include_whole_map=False)` — [`L182`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L182)
- `make_red_map_info(visual_map=None, map_source=None, include_whole_map=False, location="OaksLab", player_x=5, player_y=6)` — [`L75`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L75) — Create a Red-style map dict (no porymap, tiles are 4-tuples).
- `make_red_player_data(location="OaksLab", x=5, y=6)` — [`L166`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L166)
- `print_formatted_map(result, indent=" ")` — [`L42`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L42) — Pretty-print the list returned by _format_map_info.
- `print_formatted_state(result, indent=" ", max_lines=80)` — [`L53`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L53) — Pretty-print the string returned by format_state_for_llm.
- `test_format_map_info_empty_map()` — [`L367`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L367) — Empty/None map_info returns empty list.
- `test_format_map_info_full_map()` — [`L272`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L272) — When red_whole_map is present, full map with warps/objects is rendered.
- `test_format_map_info_has_location()` — [`L240`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L240) — Output includes location name from player_data.
- `test_format_map_info_has_player_position()` — [`L257`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L257) — Output includes player coordinates.
- `test_format_map_info_no_crash()` — [`L220`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L220) — _format_map_info must not crash on Red state data (no porymap).
- `test_format_map_info_no_visual_map()` — [`L328`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L328) — When neither porymap nor visual_map is present, output has location but no map.
- `test_format_map_info_title_sequence()` — [`L349`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L349) — TITLE_SEQUENCE location returns early with message.
- `test_format_map_info_visual_map_fallback()` — [`L304`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L304) — When only visual_map is present (no red_whole_map), the fallback renders it.
- `test_format_state_for_llm_battle_state()` — [`L436`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L436) — Works with battle state (has battle_info).
- `test_format_state_for_llm_contains_full_map()` — [`L411`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L411) — When red_whole_map is present, full map shows up in the formatted output.
- `test_format_state_for_llm_contains_key_info()` — [`L398`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L398) — Output text includes player name, location, party info.
- `test_format_state_for_llm_dialog_state()` — [`L464`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L464) — Works when dialog_text is present.
- `test_format_state_for_llm_gen1_party_fields()` — [`L485`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L485) — Gen 1 party fields (attack, defense, speed, special) don't cause errors.
- `test_format_state_for_llm_no_crash()` — [`L381`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L381) — format_state_for_llm must not crash on full Red state with whole_map.
- `test_format_state_for_llm_no_map_at_all()` — [`L503`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L503) — Works when map section has only tiles and no visual_map.
- `test_format_state_for_llm_visual_map_fallback()` — [`L424`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L424) — When only visual_map is present (no red_whole_map), fallback works.
- `test_with_real_states()` — [`L523`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L523) — Load real Red state JSONs and run format_state_for_llm on them.

## Module values
- `CELL_SYMBOLS` — [`L69`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L69)
- `FAILED` — [`L26`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L26)
- `PASSED` — [`L25`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L25)
- `REPO` — [`L20`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L20)
- `SAMPLE_VISUAL_MAP` — [`L151`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L151)
- `SEP` — [`L29`](../../../../../../raw/code/continual-harness/pokemon_red_env/test/test_red_state_formatter.py#L29)

