---
title: 'Module: tests/test_snapshot_artifacts_limit.py'
type: catalog
provenance: extracted
module: tests/test_snapshot_artifacts_limit.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_snapshot_artifacts_limit`/Test
symbols:
  TestArtifactStorageWithLimit.test_store_artifacts_within_limit: ArtifactStorageWithLimit#test_store_artifacts_within_limit().
  TestArtifactStorageWithLimit.test_store_many_artifacts: ArtifactStorageWithLimit#test_store_many_artifacts().
  TestMaxSnapshotArtifactsConfig.test_custom_value_from_dict: MaxSnapshotArtifactsConfig#test_custom_value_from_dict().
  TestMaxSnapshotArtifactsConfig.test_unlimited_artifacts_with_none: MaxSnapshotArtifactsConfig#test_unlimited_artifacts_with_none().
  TestMaxSnapshotArtifactsConfig.test_zero_artifacts: MaxSnapshotArtifactsConfig#test_zero_artifacts().
  TestSnapshotCreation.test_config_accessible_from_database: SnapshotCreation#test_config_accessible_from_database().
  TestSnapshotCreation.test_unlimited_config_is_none: SnapshotCreation#test_unlimited_config_is_none().
  TestMaxSnapshotArtifactsConfig.test_default_value_is_100: MaxSnapshotArtifactsConfig#test_default_value_is_100().
  TestArtifactStorageWithLimit.test_artifacts_for_nonexistent_program_returns_empty: ArtifactStorageWithLimit#test_artifacts_for_nonexistent_program_returns_empty().
  TestArtifactStorageWithLimit.test_store_artifacts_for_nonexistent_program_logs_warning: ArtifactStorageWithLimit#test_store_artifacts_for_nonexistent_program_logs_warning().
  TestMaxSnapshotArtifactsConfig.test_database_config_default: MaxSnapshotArtifactsConfig#test_database_config_default().
  TestMaxSnapshotArtifactsConfig: MaxSnapshotArtifactsConfig#
  TestArtifactStorageWithLimit: ArtifactStorageWithLimit#
  TestSnapshotCreation: SnapshotCreation#
---
# Module: [`tests/test_snapshot_artifacts_limit.py`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py)

## Classes
### `TestArtifactStorageWithLimit`  ·  implements/extends TestCase
- def: [`tests/test_snapshot_artifacts_limit.py:59`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L59)
- doc: Tests for artifact storage respecting the limit
- signature: `class TestArtifactStorageWithLimit(unittest.TestCase):`
- members:
  - `test_artifacts_for_nonexistent_program_returns_empty(self)` — [`L105`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L105) — Test retrieving artifacts for non-existent program
  - `test_store_artifacts_for_nonexistent_program_logs_warning(self)` — [`L113`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L113) — Test that storing artifacts for non-existent program doesn't crash
  - `test_store_artifacts_within_limit(self)` — [`L62`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L62) — Test storing artifacts when within the limit
  - `test_store_many_artifacts(self)` — [`L83`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L83) — Test storing more artifacts than the limit
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`generation`](../openevolve/database.md#Program.generation), [`store_artifacts`](../openevolve/database.md#ProgramDatabase.store_artifacts), [`get_artifacts`](../openevolve/database.md#ProgramDatabase.get_artifacts), [`max_snapshot_artifacts`](../openevolve/config.md#DatabaseConfig.max_snapshot_artifacts)

### `TestMaxSnapshotArtifactsConfig`  ·  implements/extends TestCase
- def: [`tests/test_snapshot_artifacts_limit.py:12`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L12)
- doc: Tests for max_snapshot_artifacts configuration
- signature: `class TestMaxSnapshotArtifactsConfig(unittest.TestCase):`
- members:
  - `test_custom_value_from_dict(self)` — [`L25`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L25) — Test loading custom max_snapshot_artifacts from config dict
  - `test_database_config_default(self)` — [`L20`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L20) — Test DatabaseConfig default for max_snapshot_artifacts
  - `test_default_value_is_100(self)` — [`L15`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L15) — Test that max_snapshot_artifacts defaults to 100
  - `test_unlimited_artifacts_with_none(self)` — [`L36`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L36) — Test setting unlimited artifacts with None
  - `test_zero_artifacts(self)` — [`L47`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L47) — Test setting max_snapshot_artifacts to 0
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`from_dict`](../openevolve/config.md#Config.from_dict), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`max_snapshot_artifacts`](../openevolve/config.md#DatabaseConfig.max_snapshot_artifacts)

### `TestSnapshotCreation`  ·  implements/extends TestCase
- def: [`tests/test_snapshot_artifacts_limit.py:122`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L122)
- doc: Tests for snapshot creation with artifact limits
- signature: `class TestSnapshotCreation(unittest.TestCase):`
- members:
  - `test_config_accessible_from_database(self)` — [`L125`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L125) — Test that max_snapshot_artifacts is accessible from database config
  - `test_unlimited_config_is_none(self)` — [`L132`](../../../../../raw/code/openevolve/tests/test_snapshot_artifacts_limit.py#L132) — Test that unlimited artifacts config is None
- uses (calls/refs, reference-scoped): [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`config`](../openevolve/database.md#ProgramDatabase.config), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`max_snapshot_artifacts`](../openevolve/config.md#DatabaseConfig.max_snapshot_artifacts)

