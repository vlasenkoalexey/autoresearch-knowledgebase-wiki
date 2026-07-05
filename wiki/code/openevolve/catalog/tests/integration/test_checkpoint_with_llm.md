---
title: 'Module: tests/integration/test_checkpoint_with_llm.py'
type: catalog
provenance: extracted
module: tests/integration/test_checkpoint_with_llm.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.integration.test_checkpoint_with_llm`/TestCheckpointWithLLM#
symbols:
  TestCheckpointWithLLM.test_checkpoint_intervals_with_real_llm: test_checkpoint_intervals_with_real_llm().
  TestCheckpointWithLLM.test_final_checkpoint_creation: test_final_checkpoint_creation().
  TestCheckpointWithLLM.test_checkpoint_resume_functionality: test_checkpoint_resume_functionality().
  TestCheckpointWithLLM.test_checkpoint_with_best_program_save: test_checkpoint_with_best_program_save().
  TestCheckpointWithLLM: ''
---
# Module: [`tests/integration/test_checkpoint_with_llm.py`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py)

## Classes
### `TestCheckpointWithLLM`
- def: [`tests/integration/test_checkpoint_with_llm.py:10`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py#L10)
- doc: Test checkpoints with real LLM generation
- signature: `class TestCheckpointWithLLM:`
- members:
  - `test_checkpoint_intervals_with_real_llm(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L15`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py#L15) — Test checkpoints occur at correct intervals with real evolution
  - `test_checkpoint_resume_functionality(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L58`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py#L58) — Test checkpoint save and resume with real LLM
  - `test_checkpoint_with_best_program_save(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L135`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py#L135) — Test that checkpoints include best program information
  - `test_final_checkpoint_creation(self, optillm_server, evolution_config, test_program_file, test_evaluator_file, evolution_output_dir)` — [`L101`](../../../../../../raw/code/openevolve/tests/integration/test_checkpoint_with_llm.py#L101) — Test that final checkpoint is created regardless of interval
- uses (calls/refs, reference-scoped): [`programs`](../../openevolve/database.md#ProgramDatabase.programs), [`run`](../../openevolve/controller.md#OpenEvolve.run), [`database`](../../openevolve/controller.md#OpenEvolve.database), [`_save_checkpoint`](../../openevolve/controller.md#OpenEvolve._save_checkpoint), [`OpenEvolve`](../../openevolve/controller.md#OpenEvolve)

