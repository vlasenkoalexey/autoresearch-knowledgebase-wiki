---
title: 'Module: tests/test_evolution_trace.py'
type: catalog
provenance: extracted
module: tests/test_evolution_trace.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_evolution_trace`/Test
symbols:
  TestEvolutionTracer.child_program: EvolutionTracer#child_program.
  TestEvolutionTrace.test_to_dict: EvolutionTrace#test_to_dict().
  TestEvolutionTracer.parent_program: EvolutionTracer#parent_program.
  TestCheckpointExtraction._create_test_program: CheckpointExtraction#_create_test_program().
  TestCheckpointExtraction.test_extract_single_parent_child: CheckpointExtraction#test_extract_single_parent_child().
  TestEvolutionTrace.test_calculate_improvement: EvolutionTrace#test_calculate_improvement().
  TestEvolutionTraceIntegration.test_config_integration: EvolutionTraceIntegration#test_config_integration().
  TestEvolutionTraceIntegration.test_yaml_config: EvolutionTraceIntegration#test_yaml_config().
  TestEvolutionTrace.test_trace_creation: EvolutionTrace#test_trace_creation().
  TestEvolutionTracer.test_statistics: EvolutionTracer#test_statistics().
  TestEvolutionTracer.test_jsonl_format: EvolutionTracer#test_jsonl_format().
  TestEvolutionTracer.test_json_format: EvolutionTracer#test_json_format().
  TestEvolutionTracer.test_buffer_flushing: EvolutionTracer#test_buffer_flushing().
  TestEvolutionTracer.test_artifact_logging: EvolutionTracer#test_artifact_logging().
  TestCheckpointExtraction.checkpoint_dir: CheckpointExtraction#checkpoint_dir.
  TestEvolutionTracer.test_tracer_disabled: EvolutionTracer#test_tracer_disabled().
  TestEvolutionTracer.test_context_manager: EvolutionTracer#test_context_manager().
  TestCheckpointExtraction.test_extract_with_code_inclusion: CheckpointExtraction#test_extract_with_code_inclusion().
  TestCheckpointExtraction.test_extract_without_code: CheckpointExtraction#test_extract_without_code().
  TestCheckpointExtraction.test_extract_full_lineage_json_output: CheckpointExtraction#test_extract_full_lineage_json_output().
  TestCheckpointExtraction.programs_dir: CheckpointExtraction#programs_dir.
  TestCheckpointExtraction.test_extract_multiple_generations: CheckpointExtraction#test_extract_multiple_generations().
  TestCheckpointExtraction.test_save_extracted_traces_jsonl: CheckpointExtraction#test_save_extracted_traces_jsonl().
  TestCheckpointExtraction.test_save_extracted_traces_json: CheckpointExtraction#test_save_extracted_traces_json().
  TestCheckpointExtraction.test_extract_full_lineage: CheckpointExtraction#test_extract_full_lineage().
  TestCheckpointExtraction.test_extract_with_corrupted_file: CheckpointExtraction#test_extract_with_corrupted_file().
  TestCheckpointExtraction.test_extract_with_missing_parent: CheckpointExtraction#test_extract_with_missing_parent().
  TestEvolutionTracer.temp_dir: EvolutionTracer#temp_dir.
  TestCheckpointExtraction.temp_dir: CheckpointExtraction#temp_dir.
  TestCheckpointExtraction.test_extract_from_empty_checkpoint: CheckpointExtraction#test_extract_from_empty_checkpoint().
  TestCheckpointExtraction.test_programs_dir_not_found: CheckpointExtraction#test_programs_dir_not_found().
  TestEvolutionTracer.tearDown: EvolutionTracer#tearDown().
  TestCheckpointExtraction.tearDown: CheckpointExtraction#tearDown().
  TestCheckpointExtraction.test_checkpoint_not_found: CheckpointExtraction#test_checkpoint_not_found().
  TestEvolutionTrace: EvolutionTrace#
  TestEvolutionTracer: EvolutionTracer#
  TestEvolutionTracer.setUp: EvolutionTracer#setUp().
  TestEvolutionTraceIntegration: EvolutionTraceIntegration#
  TestCheckpointExtraction: CheckpointExtraction#
  TestCheckpointExtraction.setUp: CheckpointExtraction#setUp().
---
# Module: [`tests/test_evolution_trace.py`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py)

## Classes
### `TestCheckpointExtraction`  ·  implements/extends TestCase
- def: [`tests/test_evolution_trace.py:360`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L360)
- doc: Test checkpoint extraction functionality
- signature: `class TestCheckpointExtraction(unittest.TestCase):`
- members:
  - `_create_test_program(self, prog_id, parent_id=None, iteration=0, metrics=None, generation=0)` — [`L375`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L375) — Helper to create a test program JSON file
  - `setUp(self)` — [`L363`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L363) — Set up test fixtures
  - `tearDown(self)` — [`L370`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L370) — Clean up test fixtures
  - `test_checkpoint_not_found(self)` — [`L638`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L638) — Test error handling for non-existent checkpoint
  - `test_extract_from_empty_checkpoint(self)` — [`L398`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L398) — Test extraction from checkpoint with no programs — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_extract_full_lineage(self)` — [`L517`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L517) — Test full lineage extraction
  - `test_extract_full_lineage_json_output(self)` — [`L576`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L576) — Test full lineage extraction with JSON output
  - `test_extract_multiple_generations(self)` — [`L421`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L421) — Test extraction with multiple generations
  - `test_extract_single_parent_child(self)` — [`L403`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L403) — Test extraction with single parent-child pair
  - `test_extract_with_code_inclusion(self)` — [`L437`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L437) — Test extraction with code included — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_extract_with_corrupted_file(self)` — [`L623`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L623) — Test extraction handles corrupted files gracefully — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_extract_with_missing_parent(self)` — [`L613`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L613) — Test extraction handles missing parents gracefully — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_extract_without_code(self)` — [`L453`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L453) — Test extraction without code — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_programs_dir_not_found(self)` — [`L643`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L643) — Test error handling when programs directory is missing
  - `test_save_extracted_traces_json(self)` — [`L492`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L492) — Test saving extracted traces in JSON format
  - `test_save_extracted_traces_jsonl(self)` — [`L467`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L467) — Test saving extracted traces in JSONL format
  - `checkpoint_dir` — [`L366`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L366)
  - `programs_dir` — [`L367`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L367)
  - `temp_dir` — [`L365`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L365)
- uses (calls/refs, reference-scoped): [`extract_evolution_trace_from_checkpoint`](../openevolve/evolution_trace.md#extract_evolution_trace_from_checkpoint), [`child_metrics`](../openevolve/evolution_trace.md#EvolutionTrace.child_metrics), [`extract_full_lineage_traces`](../openevolve/evolution_trace.md#extract_full_lineage_traces), [`iteration`](../openevolve/evolution_trace.md#EvolutionTrace.iteration), [`parent_metrics`](../openevolve/evolution_trace.md#EvolutionTrace.parent_metrics), [`child_id`](../openevolve/evolution_trace.md#EvolutionTrace.child_id), [`parent_id`](../openevolve/evolution_trace.md#EvolutionTrace.parent_id), [`parent_code`](../openevolve/evolution_trace.md#EvolutionTrace.parent_code), [`child_code`](../openevolve/evolution_trace.md#EvolutionTrace.child_code), [`generation`](../openevolve/evolution_trace.md#EvolutionTrace.generation)

### `TestEvolutionTrace`  ·  implements/extends TestCase
- def: [`tests/test_evolution_trace.py:21`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L21)
- doc: Test the EvolutionTrace dataclass
- signature: `class TestEvolutionTrace(unittest.TestCase):`
- members:
  - `test_calculate_improvement(self)` — [`L39`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L39) — Test improvement calculation
  - `test_to_dict(self)` — [`L56`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L56) — Test conversion to dictionary
  - `test_trace_creation(self)` — [`L24`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L24) — Test creating an evolution trace entry
- uses (calls/refs, reference-scoped): [`EvolutionTrace`](../openevolve/evolution_trace.md#EvolutionTrace), [`calculate_improvement`](../openevolve/evolution_trace.md#EvolutionTrace.calculate_improvement), [`child_metrics`](../openevolve/evolution_trace.md#EvolutionTrace.child_metrics), [`iteration`](../openevolve/evolution_trace.md#EvolutionTrace.iteration), [`parent_metrics`](../openevolve/evolution_trace.md#EvolutionTrace.parent_metrics), [`child_id`](../openevolve/evolution_trace.md#EvolutionTrace.child_id), [`parent_id`](../openevolve/evolution_trace.md#EvolutionTrace.parent_id), [`parent_code`](../openevolve/evolution_trace.md#EvolutionTrace.parent_code), [`timestamp`](../openevolve/evolution_trace.md#EvolutionTrace.timestamp), [`island_id`](../openevolve/evolution_trace.md#EvolutionTrace.island_id), [`to_dict`](../openevolve/evolution_trace.md#EvolutionTrace.to_dict)

### `TestEvolutionTraceIntegration`  ·  implements/extends TestCase
- def: [`tests/test_evolution_trace.py:311`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L311)
- doc: Test integration with OpenEvolve configuration
- signature: `class TestEvolutionTraceIntegration(unittest.TestCase):`
- members:
  - `test_config_integration(self)` — [`L314`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L314) — Test that evolution trace config is properly integrated
  - `test_yaml_config(self)` — [`L334`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L334) — Test loading evolution trace config from YAML
- uses (calls/refs, reference-scoped): [`Config`](../openevolve/config.md#Config), [`from_dict`](../openevolve/config.md#Config.from_dict), [`evolution_trace`](../openevolve/config.md#Config.evolution_trace), [`format`](../openevolve/config.md#EvolutionTraceConfig.format), [`EvolutionTraceConfig`](../openevolve/config.md#EvolutionTraceConfig), [`enabled`](../openevolve/config.md#EvolutionTraceConfig.enabled), [`include_code`](../openevolve/config.md#EvolutionTraceConfig.include_code), [`include_prompts`](../openevolve/config.md#EvolutionTraceConfig.include_prompts), [`buffer_size`](../openevolve/config.md#EvolutionTraceConfig.buffer_size), [`output_path`](../openevolve/config.md#EvolutionTraceConfig.output_path)

### `TestEvolutionTracer`  ·  implements/extends TestCase
- def: [`tests/test_evolution_trace.py:77`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L77)
- doc: Test the EvolutionTracer class
- signature: `class TestEvolutionTracer(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L80`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L80) — Set up test fixtures
  - `tearDown(self)` — [`L99`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L99) — Clean up test fixtures
  - `test_artifact_logging(self)` — [`L277`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L277) — Test logging with artifacts
  - `test_buffer_flushing(self)` — [`L223`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L223) — Test buffer flushing behavior — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_context_manager(self)` — [`L260`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L260) — Test using tracer as context manager — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `test_json_format(self)` — [`L153`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L153) — Test JSON format output
  - `test_jsonl_format(self)` — [`L118`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L118) — Test JSONL format output
  - `test_statistics(self)` — [`L188`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L188) — Test statistics tracking
  - `test_tracer_disabled(self)` — [`L104`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L104) — Test that disabled tracer does nothing — documented in [openevolve-evolution_trace](../../concepts/openevolve-evolution_trace.md)
  - `child_program` — [`L90`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L90)
  - `parent_program` — [`L83`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L83)
  - `temp_dir` — [`L82`](../../../../../raw/code/openevolve/tests/test_evolution_trace.py#L82)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`code`](../openevolve/database.md#Program.code), [`log_trace`](../openevolve/evolution_trace.md#EvolutionTracer.log_trace), [`language`](../openevolve/database.md#Program.language), [`close`](../openevolve/evolution_trace.md#EvolutionTracer.close), [`generation`](../openevolve/database.md#Program.generation), [`parent_id`](../openevolve/database.md#Program.parent_id), [`EvolutionTracer`](../openevolve/evolution_trace.md#EvolutionTracer), [`get_statistics`](../openevolve/evolution_trace.md#EvolutionTracer.get_statistics)

