---
title: 'Module: tests/test_island_parent_consistency.py'
type: catalog
provenance: extracted
module: tests/test_island_parent_consistency.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_island_parent_consistency`/TestIslandParentConsistency#
symbols:
  TestIslandParentConsistency.test_parent_child_island_consistency: test_parent_child_island_consistency().
  TestIslandParentConsistency.test_multiple_generations_island_drift: test_multiple_generations_island_drift().
  TestIslandParentConsistency.test_explicit_migration_override: test_explicit_migration_override().
  TestIslandParentConsistency: ''
---
# Module: [`tests/test_island_parent_consistency.py`](../../../../../raw/code/openevolve/tests/test_island_parent_consistency.py)

## Classes
### `TestIslandParentConsistency`  ·  implements/extends TestCase
- def: [`tests/test_island_parent_consistency.py:10`](../../../../../raw/code/openevolve/tests/test_island_parent_consistency.py#L10)
- doc: Test that parent-child relationships respect island boundaries
- signature: `class TestIslandParentConsistency(unittest.TestCase):`
- members:
  - `test_explicit_migration_override(self)` — [`L132`](../../../../../raw/code/openevolve/tests/test_island_parent_consistency.py#L132) — Test that explicit target_island overrides parent island inheritance
  - `test_multiple_generations_island_drift(self)` — [`L66`](../../../../../raw/code/openevolve/tests/test_island_parent_consistency.py#L66) — Test that children inherit their parent's island at time of creation
  - `test_parent_child_island_consistency(self)` — [`L13`](../../../../../raw/code/openevolve/tests/test_island_parent_consistency.py#L13) — Test that children are added to the same island as their parents — documented in [openevolve-database](../../concepts/openevolve-database.md)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`islands`](../openevolve/database.md#ProgramDatabase.islands), [`metadata`](../openevolve/database.md#Program.metadata), [`current_island`](../openevolve/database.md#ProgramDatabase.current_island), [`num_islands`](../openevolve/config.md#DatabaseConfig.num_islands), [`parent_id`](../openevolve/database.md#Program.parent_id), [`iteration_found`](../openevolve/database.md#Program.iteration_found), [`next_island`](../openevolve/database.md#ProgramDatabase.next_island)

