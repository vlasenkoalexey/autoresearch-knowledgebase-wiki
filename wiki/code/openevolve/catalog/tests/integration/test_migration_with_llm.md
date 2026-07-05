---
title: 'Module: tests/integration/test_migration_with_llm.py'
type: catalog
provenance: extracted
module: tests/integration/test_migration_with_llm.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_migration_with_llm`/TestMigrationWithLLM#
symbols:
  TestMigrationWithLLM.test_migration_preserves_program_quality: test_migration_preserves_program_quality().
  TestMigrationWithLLM.test_island_migration_no_duplicates_real_evolution: test_island_migration_no_duplicates_real_evolution().
  TestMigrationWithLLM.test_single_island_no_migration: test_single_island_no_migration().
  TestMigrationWithLLM.test_per_island_map_elites_isolation: test_per_island_map_elites_isolation().
  TestMigrationWithLLM.test_migration_timing_logic: test_migration_timing_logic().
  TestMigrationWithLLM: ''
---
# Module: [`tests/integration/test_migration_with_llm.py`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py)

## Classes
### `TestMigrationWithLLM`
- def: [`tests/integration/test_migration_with_llm.py:10`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L10)
- doc: Test island migration with real LLM generation
- signature: `class TestMigrationWithLLM:`
- members:
  - `test_island_migration_no_duplicates_real_evolution(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L15`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L15) — Test that migration doesn't create duplicate chains with real evolution
  - `test_migration_preserves_program_quality(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L119`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L119) — Test that migration preserves program content and metrics — documented in [openevolve-controller](../../../concepts/openevolve-controller.md)
  - `test_migration_timing_logic(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L170`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L170) — Test that migration timing logic works correctly
  - `test_per_island_map_elites_isolation(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L76`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L76) — Test that per-island MAP-Elites works correctly with migration
  - `test_single_island_no_migration(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L215`](../../../../../../raw/code/openevolve/tests/integration/test_migration_with_llm.py#L215) — Test that single island setup doesn't attempt migration
- uses (calls/refs, reference-scoped): [`id`](../../openevolve/database.md#Program.id), [`metrics`](../../openevolve/database.md#Program.metrics), [`programs`](../../openevolve/database.md#ProgramDatabase.programs), [`run`](../../openevolve/controller.md#OpenEvolve.run), [`database`](../../openevolve/controller.md#OpenEvolve.database), [`metadata`](../../openevolve/database.md#Program.metadata), [`language`](../../openevolve/database.md#Program.language), [`island_feature_maps`](../../openevolve/database.md#ProgramDatabase.island_feature_maps), [`island_generations`](../../openevolve/database.md#ProgramDatabase.island_generations), [`OpenEvolve`](../../openevolve/controller.md#OpenEvolve), [`parent_id`](../../openevolve/database.md#Program.parent_id), [`get`](../../openevolve/database.md#ProgramDatabase.get), [`last_migration_generation`](../../openevolve/database.md#ProgramDatabase.last_migration_generation)

