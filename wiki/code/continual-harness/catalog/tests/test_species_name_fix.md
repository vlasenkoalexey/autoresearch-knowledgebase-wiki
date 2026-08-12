---
title: 'Module: tests/test_species_name_fix.py'
type: catalog
provenance: extracted
module: tests/test_species_name_fix.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_species_name_fix`/test_
symbols:
  test_torchic_state_with_emulator: torchic_state_with_emulator().
  test_rom_species_mapping: rom_species_mapping().
  test_pokemon_species_enum_mismatch: pokemon_species_enum_mismatch().
  test_existing_usage_in_memory_reader: existing_usage_in_memory_reader().
---
# Module: [`tests/test_species_name_fix.py`](../../../../../raw/code/continual-harness/tests/test_species_name_fix.py)

## Functions
- `test_existing_usage_in_memory_reader()` — [`L51`](../../../../../raw/code/continual-harness/tests/test_species_name_fix.py#L51) — Point to existing logic that uses species_id to derive species name.
- `test_pokemon_species_enum_mismatch()` — [`L27`](../../../../../raw/code/continual-harness/tests/test_species_name_fix.py#L27) — Verify PokemonSpecies enum uses different numbering (Hoenn Dex order).
- `test_rom_species_mapping()` — [`L15`](../../../../../raw/code/continual-harness/tests/test_species_name_fix.py#L15) — Verify ROM species IDs map to correct names (emerald_utils single source).
- `test_torchic_state_with_emulator()` — [`L62`](../../../../../raw/code/continual-harness/tests/test_species_name_fix.py#L62) — Load torchic.state and verify species_id, nickname, and fix logic.

