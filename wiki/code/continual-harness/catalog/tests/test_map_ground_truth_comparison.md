---
title: 'Module: tests/test_map_ground_truth_comparison.py'
type: catalog
provenance: extracted
module: tests/test_map_ground_truth_comparison.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_map_ground_truth_comparison`/TestMapGroundTruthComparison#
symbols:
  TestMapGroundTruthComparison.test_direct_emulator_outside_map: test_direct_emulator_outside_map().
  TestMapGroundTruthComparison.test_direct_emulator_house_map: test_direct_emulator_house_map().
  TestMapGroundTruthComparison.save_map_output: save_map_output().
  TestMapGroundTruthComparison.compare_with_ground_truth: compare_with_ground_truth().
  TestMapGroundTruthComparison.extract_traversability_map: extract_traversability_map().
  TestMapGroundTruthComparison.test_server_house_map: test_server_house_map().
  TestMapGroundTruthComparison.test_server_outside_map: test_server_outside_map().
  TestMapGroundTruthComparison.test_cross_comparison_house: test_cross_comparison_house().
  TestMapGroundTruthComparison.test_cross_comparison_outside: test_cross_comparison_outside().
  TestMapGroundTruthComparison.format_map_for_comparison: format_map_for_comparison().
  TestMapGroundTruthComparison: ''
  TestMapGroundTruthComparison.output_dir: output_dir().
  TestMapGroundTruthComparison.ground_truth_dir: ground_truth_dir().
---
# Module: [`tests/test_map_ground_truth_comparison.py`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py)

## Classes
### `TestMapGroundTruthComparison`
- def: [`tests/test_map_ground_truth_comparison.py:16`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L16)
- doc: Test suite for comparing map outputs to ground truth
- signature: `class TestMapGroundTruthComparison:`
- members:
  - `compare_with_ground_truth(self, output_content, ground_truth_file)` — [`L101`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L101) — Compare output with ground truth file
  - `extract_traversability_map(content)` — [`L110`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L110)
  - `format_map_for_comparison(self, tiles, title, location, position)` — [`L31`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L31) — Format map tiles for comparison with ground truth format
  - `ground_truth_dir(self)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L27) — Path to ground truth files
  - `output_dir(self)` — [`L20`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L20) — Create output directory for test results
  - `save_map_output(self, tiles, output_file, title, location, position)` — [`L91`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L91) — Save map output to file
  - `test_cross_comparison_house(self, output_dir)` — [`L394`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L394) — Test that direct emulator and server produce identical house maps
  - `test_cross_comparison_outside(self, output_dir)` — [`L429`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L429) — Test that direct emulator and server produce identical outside maps
  - `test_direct_emulator_house_map(self, output_dir, ground_truth_dir)` — [`L150`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L150) — Test direct emulator house map against ground truth
  - `test_direct_emulator_outside_map(self, output_dir, ground_truth_dir)` — [`L187`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L187) — Test direct emulator outside map against ground truth
  - `test_server_house_map(self, output_dir, ground_truth_dir)` — [`L232`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L232) — Test server house map against ground truth
  - `test_server_outside_map(self, output_dir, ground_truth_dir)` — [`L290`](../../../../../raw/code/continual-harness/tests/test_map_ground_truth_comparison.py#L290) — Test server outside map against ground truth
- uses (calls/refs, reference-scoped): [`get_comprehensive_state`](../pokemon_env/memory_reader.md#PokemonEmeraldReader.get_comprehensive_state), [`load_state`](../pokemon_env/emulator.md#EmeraldEmulator.load_state), [`memory_reader`](../pokemon_env/emulator.md#EmeraldEmulator.memory_reader), [`initialize`](../pokemon_env/emulator.md#EmeraldEmulator.initialize), [`EmeraldEmulator`](../pokemon_env/emulator.md#EmeraldEmulator), [`press_buttons`](../pokemon_env/emulator.md#EmeraldEmulator.press_buttons), [`stop`](../pokemon_env/emulator.md#EmeraldEmulator.stop)

