---
title: 'Module: tests/test_grid_stability.py'
type: catalog
provenance: extracted
module: tests/test_grid_stability.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_grid_stability`/TestGridStability#
symbols:
  TestGridStability.test_feature_ranges_preserved_across_checkpoints: test_feature_ranges_preserved_across_checkpoints().
  TestGridStability.test_grid_expansion_behavior: test_grid_expansion_behavior().
  TestGridStability.test_feature_stats_consistency_across_cycles: test_feature_stats_consistency_across_cycles().
  TestGridStability.test_feature_stats_accumulation: test_feature_stats_accumulation().
  TestGridStability.test_dir: test_dir.
  TestGridStability.tearDown: tearDown().
  TestGridStability: ''
  TestGridStability.setUp: setUp().
---
# Module: [`tests/test_grid_stability.py`](../../../../../raw/code/openevolve/tests/test_grid_stability.py)

## Classes
### `TestGridStability`  ·  implements/extends TestCase
- def: [`tests/test_grid_stability.py:14`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L14)
- doc: Integration tests for MAP-Elites grid stability when resuming from checkpoints
- signature: `class TestGridStability(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L17`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L17) — Set up test environment
  - `tearDown(self)` — [`L21`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L21) — Clean up test environment
  - `test_feature_ranges_preserved_across_checkpoints(self)` — [`L25`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L25) — Test that feature ranges are preserved across checkpoint save/load cycles — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `test_feature_stats_accumulation(self)` — [`L238`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L238) — Test that feature_stats accumulate correctly across checkpoint cycles
  - `test_feature_stats_consistency_across_cycles(self)` — [`L170`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L170) — Test that feature_stats remain consistent across multiple save/load cycles
  - `test_grid_expansion_behavior(self)` — [`L112`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L112) — Test that grid expands correctly when new programs exceed existing ranges
  - `test_dir` — [`L19`](../../../../../raw/code/openevolve/tests/test_grid_stability.py#L19)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`load`](../openevolve/database.md#ProgramDatabase.load), [`save`](../openevolve/database.md#ProgramDatabase.save), [`feature_stats`](../openevolve/database.md#ProgramDatabase.feature_stats), [`_calculate_feature_coords`](../openevolve/database.md#ProgramDatabase._calculate_feature_coords), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`feature_dimensions`](../openevolve/config.md#DatabaseConfig.feature_dimensions), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path), [`feature_bins`](../openevolve/config.md#DatabaseConfig.feature_bins)

