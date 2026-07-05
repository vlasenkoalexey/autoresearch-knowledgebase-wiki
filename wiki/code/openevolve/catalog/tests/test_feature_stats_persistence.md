---
title: 'Module: tests/test_feature_stats_persistence.py'
type: catalog
provenance: extracted
module: tests/test_feature_stats_persistence.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_feature_stats_persistence`/TestFeatureStatsPersistence#
symbols:
  TestFeatureStatsPersistence.test_feature_stats_preservation_during_load: test_feature_stats_preservation_during_load().
  TestFeatureStatsPersistence.test_feature_stats_saved_and_loaded: test_feature_stats_saved_and_loaded().
  TestFeatureStatsPersistence.config: config.
  TestFeatureStatsPersistence.test_empty_feature_stats_handling: test_empty_feature_stats_handling().
  TestFeatureStatsPersistence.test_backward_compatibility_missing_feature_stats: test_backward_compatibility_missing_feature_stats().
  TestFeatureStatsPersistence.test_feature_stats_serialization_edge_cases: test_feature_stats_serialization_edge_cases().
  TestFeatureStatsPersistence.test_feature_stats_with_numpy_types: test_feature_stats_with_numpy_types().
  TestFeatureStatsPersistence.test_dir: test_dir.
  TestFeatureStatsPersistence.test_malformed_feature_stats_handling: test_malformed_feature_stats_handling().
  TestFeatureStatsPersistence.tearDown: tearDown().
  TestFeatureStatsPersistence: ''
  TestFeatureStatsPersistence.setUp: setUp().
---
# Module: [`tests/test_feature_stats_persistence.py`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py)

## Classes
### `TestFeatureStatsPersistence`  ·  implements/extends TestCase
- def: [`tests/test_feature_stats_persistence.py:16`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L16)
- doc: Test feature_stats are correctly saved and loaded in checkpoints
- signature: `class TestFeatureStatsPersistence(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L19`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L19) — Set up test environment
  - `tearDown(self)` — [`L28`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L28) — Clean up test environment
  - `test_backward_compatibility_missing_feature_stats(self)` — [`L93`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L93) — Test loading checkpoints that don't have feature_stats (backward compatibility)
  - `test_empty_feature_stats_handling(self)` — [`L80`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L80) — Test handling of empty feature_stats
  - `test_feature_stats_preservation_during_load(self)` — [`L159`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L159) — Test that feature_stats ranges are preserved when loading from checkpoint
  - `test_feature_stats_saved_and_loaded(self)` — [`L32`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L32) — Test that feature_stats are correctly saved and loaded from checkpoints
  - `test_feature_stats_serialization_edge_cases(self)` — [`L122`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L122) — Test feature_stats serialization handles edge cases correctly
  - `test_feature_stats_with_numpy_types(self)` — [`L230`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L230) — Test that numpy types are correctly handled in serialization
  - `test_malformed_feature_stats_handling(self)` — [`L257`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L257) — Test handling of malformed feature_stats during deserialization
  - `config` — [`L22`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L22)
  - `test_dir` — [`L21`](../../../../../raw/code/openevolve/tests/test_feature_stats_persistence.py#L21)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`load`](../openevolve/database.md#ProgramDatabase.load), [`save`](../openevolve/database.md#ProgramDatabase.save), [`feature_stats`](../openevolve/database.md#ProgramDatabase.feature_stats), [`_calculate_feature_coords`](../openevolve/database.md#ProgramDatabase._calculate_feature_coords), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`feature_dimensions`](../openevolve/config.md#DatabaseConfig.feature_dimensions), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path), [`feature_bins`](../openevolve/config.md#DatabaseConfig.feature_bins), [`_deserialize_feature_stats`](../openevolve/database.md#ProgramDatabase._deserialize_feature_stats), [`_serialize_feature_stats`](../openevolve/database.md#ProgramDatabase._serialize_feature_stats)

