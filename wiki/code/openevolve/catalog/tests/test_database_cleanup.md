---
title: 'Module: tests/test_database_cleanup.py'
type: catalog
provenance: extracted
module: tests/test_database_cleanup.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_database_cleanup`/TestArtifactCleanup#
symbols:
  TestArtifactCleanup.test_artifact_cleanup: test_artifact_cleanup().
  TestArtifactCleanup.db_path: db_path.
  TestArtifactCleanup.tearDown: tearDown().
  TestArtifactCleanup.temp_dir: temp_dir.
  TestArtifactCleanup: ''
  TestArtifactCleanup.setUp: setUp().
---
# Module: [`tests/test_database_cleanup.py`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py)

## Classes
### `TestArtifactCleanup`  ·  implements/extends TestCase
- def: [`tests/test_database_cleanup.py:13`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L13)
- signature: `class TestArtifactCleanup(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L15`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L15)
  - `tearDown(self)` — [`L20`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L20)
  - `test_artifact_cleanup(self)` — [`L23`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L23)
  - `db_path` — [`L17`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L17)
  - `temp_dir` — [`L16`](../../../../../raw/code/openevolve/tests/test_database_cleanup.py#L16)
- uses (calls/refs, reference-scoped): [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`save`](../openevolve/database.md#ProgramDatabase.save), [`DatabaseConfig`](../openevolve/config.md#DatabaseConfig), [`db_path`](../openevolve/config.md#DatabaseConfig.db_path), [`artifact_retention_days`](../openevolve/config.md#DatabaseConfig.artifact_retention_days), [`cleanup_old_artifacts`](../openevolve/config.md#DatabaseConfig.cleanup_old_artifacts)

