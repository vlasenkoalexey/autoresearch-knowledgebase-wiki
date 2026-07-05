---
title: 'Module: tests/test_concurrent_island_access.py'
type: catalog
provenance: extracted
module: tests/test_concurrent_island_access.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_concurrent_island_access`/
symbols:
  TestConcurrentIslandAccess.database: TestConcurrentIslandAccess#database.
  TestConcurrentIslandAccess.config: TestConcurrentIslandAccess#config.
  TestConcurrentIslandAccess.sample_from_island: TestConcurrentIslandAccess#sample_from_island().
  TestConcurrentIslandAccess.test_proposed_fix_with_island_specific_sampling: TestConcurrentIslandAccess#test_proposed_fix_with_island_specific_sampling().
  TestConcurrentIslandAccess.sample_from_island_safe: TestConcurrentIslandAccess#sample_from_island_safe().
  TestConcurrentIslandAccess.safe_sample: TestConcurrentIslandAccess#safe_sample().
  result: result.
  TestConcurrentIslandAccess.test_sequential_island_access_works_correctly: TestConcurrentIslandAccess#test_sequential_island_access_works_correctly().
  suite: suite.
  TestConcurrentIslandAccess.tearDown: TestConcurrentIslandAccess#tearDown().
  TestConcurrentIslandAccess.test_concurrent_island_state_modification_causes_race_condition: TestConcurrentIslandAccess#test_concurrent_island_state_modification_causes_race_condition().
  TestConcurrentIslandAccess: TestConcurrentIslandAccess#
  TestConcurrentIslandAccess.temp_dir: TestConcurrentIslandAccess#temp_dir.
  runner: runner.
  TestConcurrentIslandAccess.setUp: TestConcurrentIslandAccess#setUp().
---
# Module: [`tests/test_concurrent_island_access.py`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py)

## Classes
### `TestConcurrentIslandAccess`  ·  implements/extends TestCase
- def: [`tests/test_concurrent_island_access.py:17`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L17)
- doc: Test concurrent access to island state in database
- signature: `class TestConcurrentIslandAccess(unittest.TestCase):`
- members:
  - `safe_sample(island_id)` — [`L199`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L199) — Use the safe sampling method
  - `sample_from_island(island_id)` — [`L59`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L59) — Simulate what _submit_iteration does
  - `sample_from_island_safe(island_id, num_inspirations=2)` — [`L159`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L159) — Safe sampling that doesn't modify current_island
  - `setUp(self)` — [`L20`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L20) — Set up test database with multiple islands
  - `tearDown(self)` — [`L45`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L45) — Clean up temp directory
  - `test_concurrent_island_state_modification_causes_race_condition(self)` — [`L50`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L50) — Test that concurrent modifications to current_island cause issues
  - `test_proposed_fix_with_island_specific_sampling(self)` — [`L153`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L153) — Test the proposed fix: using a method that doesn't modify shared state
  - `test_sequential_island_access_works_correctly(self)` — [`L124`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L124) — Test that sequential access works without issues using safe sampling
  - `config` — [`L22`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L22)
  - `database` — [`L30`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L30)
  - `temp_dir` — [`L27`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L27)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`sample_from_island`](../openevolve/database.md#ProgramDatabase.sample_from_island), [`current_island`](../openevolve/database.md#ProgramDatabase.current_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`sample`](../openevolve/database.md#ProgramDatabase.sample), [`population_size`](../openevolve/config.md#DatabaseConfig.population_size)
- used by: (1 test-only callers)

## Module values
- `result` — [`L250`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L250)
- `runner` — [`L249`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L249)
- `suite` — [`L246`](../../../../../raw/code/openevolve/tests/test_concurrent_island_access.py#L246)

