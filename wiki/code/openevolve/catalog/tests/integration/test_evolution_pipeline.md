---
title: 'Module: tests/integration/test_evolution_pipeline.py'
type: catalog
provenance: extracted
module: tests/integration/test_evolution_pipeline.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_evolution_pipeline`/TestEvolutionPipeline#
symbols:
  TestEvolutionPipeline.test_best_program_tracking: test_best_program_tracking().
  TestEvolutionPipeline.test_full_evolution_loop: test_full_evolution_loop().
  TestEvolutionPipeline.test_island_feature_maps_populated: test_island_feature_maps_populated().
  TestEvolutionPipeline.test_evolution_with_small_model_succeeds: test_evolution_with_small_model_succeeds().
  TestEvolutionPipeline: ''
---
# Module: [`tests/integration/test_evolution_pipeline.py`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py)

## Classes
### `TestEvolutionPipeline`
- def: [`tests/integration/test_evolution_pipeline.py:10`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py#L10)
- doc: Test complete evolution with real LLM generation
- signature: `class TestEvolutionPipeline:`
- members:
  - `test_best_program_tracking(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L142`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py#L142) — Test that best program tracking works correctly
  - `test_evolution_with_small_model_succeeds(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L105`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py#L105) — Test that evolution works with small local model (may not be perfect but should not crash)
  - `test_full_evolution_loop(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L15`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py#L15) — Test complete evolution with real LLM
  - `test_island_feature_maps_populated(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L67`](../../../../../../raw/code/openevolve/tests/integration/test_evolution_pipeline.py#L67) — Test that island feature maps are properly populated during evolution
- uses (calls/refs, reference-scoped): [`id`](../../openevolve/database.md#Program.id), [`programs`](../../openevolve/database.md#ProgramDatabase.programs), [`run`](../../openevolve/controller.md#OpenEvolve.run), [`database`](../../openevolve/controller.md#OpenEvolve.database), [`metadata`](../../openevolve/database.md#Program.metadata), [`island_feature_maps`](../../openevolve/database.md#ProgramDatabase.island_feature_maps), [`best_program_id`](../../openevolve/database.md#ProgramDatabase.best_program_id), [`OpenEvolve`](../../openevolve/controller.md#OpenEvolve), [`get_best_program`](../../openevolve/database.md#ProgramDatabase.get_best_program), [`get`](../../openevolve/database.md#ProgramDatabase.get), [`iteration_found`](../../openevolve/database.md#Program.iteration_found)

