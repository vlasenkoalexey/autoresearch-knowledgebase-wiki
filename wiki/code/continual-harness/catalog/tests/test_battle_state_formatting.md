---
title: 'Module: tests/test_battle_state_formatting.py'
type: catalog
provenance: extracted
module: tests/test_battle_state_formatting.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_battle_state_formatting`/test_
symbols:
  test_battle_mode_hides_map: battle_mode_hides_map().
  test_normal_mode_shows_everything: normal_mode_shows_everything().
  test_battle_mode_hides_dialogue: battle_mode_hides_dialogue().
  test_battle_party_information: battle_party_information().
  test_battle_mode_detection_variants: battle_mode_detection_variants().
  test_empty_battle_info: empty_battle_info().
---
# Module: [`tests/test_battle_state_formatting.py`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py)

## Functions
- `test_battle_mode_detection_variants()` — [`L153`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L153) — Test that both is_in_battle and in_battle keys trigger battle mode.
- `test_battle_mode_hides_dialogue()` — [`L51`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L51) — Test that battle mode doesn't show dialogue information.
- `test_battle_mode_hides_map()` — [`L11`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L11) — Test that battle mode doesn't show map information.
- `test_battle_party_information()` — [`L118`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L118) — Test that battle mode shows full party for switching decisions.
- `test_empty_battle_info()` — [`L184`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L184) — Test handling of battle mode with missing battle info.
- `test_normal_mode_shows_everything()` — [`L77`](../../../../../raw/code/continual-harness/tests/test_battle_state_formatting.py#L77) — Test that normal (non-battle) mode shows all information.

