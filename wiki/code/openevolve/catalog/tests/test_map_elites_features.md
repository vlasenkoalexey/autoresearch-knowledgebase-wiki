---
title: 'Module: tests/test_map_elites_features.py'
type: catalog
provenance: extracted
module: tests/test_map_elites_features.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_map_elites_features`/TestMapElitesFeatures#
symbols:
  TestMapElitesFeatures.test_custom_features_override_builtin: test_custom_features_override_builtin().
  TestMapElitesFeatures.test_per_dimension_bins: test_per_dimension_bins().
  TestMapElitesFeatures.test_feature_coordinates_with_new_defaults: test_feature_coordinates_with_new_defaults().
  TestMapElitesFeatures.db: db.
  TestMapElitesFeatures.test_missing_feature_dimension_error: test_missing_feature_dimension_error().
  TestMapElitesFeatures.test_diversity_reference_set_update: test_diversity_reference_set_update().
  TestMapElitesFeatures.test_diversity_cache_lru_eviction: test_diversity_cache_lru_eviction().
  TestMapElitesFeatures.test_diversity_caching: test_diversity_caching().
  TestMapElitesFeatures.test_feature_scaling_minmax: test_feature_scaling_minmax().
  TestMapElitesFeatures.test_feature_scaling_with_identical_values: test_feature_scaling_with_identical_values().
  TestMapElitesFeatures.setUp: setUp().
  TestMapElitesFeatures.test_feature_stats_update: test_feature_stats_update().
  TestMapElitesFeatures.test_default_feature_dimensions: test_default_feature_dimensions().
  TestMapElitesFeatures: ''
---
# Module: [`tests/test_map_elites_features.py`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py)

## Classes
### `TestMapElitesFeatures`  ·  implements/extends TestCase
- def: [`tests/test_map_elites_features.py:11`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L11)
- doc: Tests for MAP-Elites feature enhancements
- signature: `class TestMapElitesFeatures(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L14`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L14) — Set up test database with enhanced features
  - `test_custom_features_override_builtin(self)` — [`L271`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L271) — Test that custom complexity and diversity from evaluator override built-in calculations
  - `test_default_feature_dimensions(self)` — [`L148`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L148) — Test default feature dimensions are complexity and diversity
  - `test_diversity_cache_lru_eviction(self)` — [`L154`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L154) — Test LRU eviction in diversity cache
  - `test_diversity_caching(self)` — [`L22`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L22) — Test diversity score caching functionality
  - `test_diversity_reference_set_update(self)` — [`L53`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L53) — Test diversity reference set updates
  - `test_feature_coordinates_with_new_defaults(self)` — [`L209`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L209) — Test feature coordinate calculation with new default dimensions
  - `test_feature_scaling_minmax(self)` — [`L78`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L78) — Test min-max feature scaling
  - `test_feature_scaling_with_identical_values(self)` — [`L193`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L193) — Test feature scaling when all values are identical
  - `test_feature_stats_update(self)` — [`L101`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L101) — Test feature statistics are updated correctly
  - `test_missing_feature_dimension_error(self)` — [`L247`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L247) — Test that missing feature dimensions raise appropriate errors
  - `test_per_dimension_bins(self)` — [`L118`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L118) — Test per-dimension bin configuration
  - `db` — [`L20`](../../../../../raw/code/openevolve/tests/test_map_elites_features.py#L20)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`language`](../openevolve/database.md#Program.language), [`config`](../openevolve/database.md#ProgramDatabase.config), [`feature_stats`](../openevolve/database.md#ProgramDatabase.feature_stats), [`_calculate_feature_coords`](../openevolve/database.md#ProgramDatabase._calculate_feature_coords), [`feature_dimensions`](../openevolve/config.md#DatabaseConfig.feature_dimensions), [`feature_bins`](../openevolve/database.md#ProgramDatabase.feature_bins), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`feature_bins_per_dim`](../openevolve/database.md#ProgramDatabase.feature_bins_per_dim), [`_get_cached_diversity`](../openevolve/database.md#ProgramDatabase._get_cached_diversity), [`_scale_feature_value`](../openevolve/database.md#ProgramDatabase._scale_feature_value), [`_update_diversity_reference_set`](../openevolve/database.md#ProgramDatabase._update_diversity_reference_set), [`diversity_cache`](../openevolve/database.md#ProgramDatabase.diversity_cache), [`feature_bins`](../openevolve/config.md#DatabaseConfig.feature_bins), [`_update_feature_stats`](../openevolve/database.md#ProgramDatabase._update_feature_stats), [`diversity_reference_set`](../openevolve/database.md#ProgramDatabase.diversity_reference_set), [`diversity_reference_size`](../openevolve/database.md#ProgramDatabase.diversity_reference_size), [`diversity_cache_size`](../openevolve/database.md#ProgramDatabase.diversity_cache_size)

