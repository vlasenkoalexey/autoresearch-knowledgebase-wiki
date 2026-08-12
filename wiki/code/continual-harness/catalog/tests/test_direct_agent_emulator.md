---
title: 'Module: tests/test_direct_agent_emulator.py'
type: catalog
provenance: extracted
module: tests/test_direct_agent_emulator.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_direct_agent_emulator`/TestDirectAgentEmulator#
symbols:
  TestDirectAgentEmulator.test_direct_emulator_house_to_outside: test_direct_emulator_house_to_outside().
  TestDirectAgentEmulator.test_direct_agent_simulation: test_direct_agent_simulation().
  TestDirectAgentEmulator.save_map_output: save_map_output().
  TestDirectAgentEmulator.analyze_map_corruption: analyze_map_corruption().
  TestDirectAgentEmulator.format_map_for_comparison: format_map_for_comparison().
  TestDirectAgentEmulator: ''
  TestDirectAgentEmulator.output_dir: output_dir().
---
# Module: [`tests/test_direct_agent_emulator.py`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py)

## Classes
### `TestDirectAgentEmulator`
- def: [`tests/test_direct_agent_emulator.py:13`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L13)
- doc: Test agent functionality by running emulator directly
- signature: `class TestDirectAgentEmulator:`
- members:
  - `analyze_map_corruption(self, tiles)` — [`L198`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L198) — Analyze map for corruption (IM tiles)
  - `format_map_for_comparison(self, tiles, title, location, position)` — [`L23`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L23) — Format map tiles for comparison
  - `output_dir(self)` — [`L17`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L17) — Create output directory for test results
  - `save_map_output(self, tiles, output_file, title, location, position)` — [`L82`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L82) — Save map output to file
  - `test_direct_agent_simulation(self, output_dir)` — [`L225`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L225) — Test simulating agent decision-making with direct emulator access
  - `test_direct_emulator_house_to_outside(self, output_dir)` — [`L92`](../../../../../raw/code/continual-harness/tests/test_direct_agent_emulator.py#L92) — Test direct emulator movement from house to outside
- uses (calls/refs, reference-scoped): [`load_state`](../pokemon_env/emulator.md#EmeraldEmulator.load_state), [`initialize`](../pokemon_env/emulator.md#EmeraldEmulator.initialize), [`get_comprehensive_state`](../pokemon_env/emulator.md#EmeraldEmulator.get_comprehensive_state), [`EmeraldEmulator`](../pokemon_env/emulator.md#EmeraldEmulator), [`press_buttons`](../pokemon_env/emulator.md#EmeraldEmulator.press_buttons), [`stop`](../pokemon_env/emulator.md#EmeraldEmulator.stop)

