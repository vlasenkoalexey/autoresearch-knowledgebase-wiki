---
title: 'Module: OpenMLE-Evo/tts_search/validation_split_guidance.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/validation_split_guidance.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.validation_split_guidance`/
symbols:
  patch_eval_data_with_guidance: patch_eval_data_with_guidance().
  _patch_rows: _patch_rows().
  _inject_guidance: _inject_guidance().
  GuidancePatchStats.total_rows: GuidancePatchStats#total_rows.
  GuidancePatchStats.patched_rows: GuidancePatchStats#patched_rows.
  GuidancePatchStats.skipped_existing_rows: GuidancePatchStats#skipped_existing_rows.
  load_guidance_map: load_guidance_map().
  GuidancePatchStats: GuidancePatchStats#
  GuidancePatchStats.input_path: GuidancePatchStats#input_path.
  GuidancePatchStats.output_path: GuidancePatchStats#output_path.
  GuidancePatchStats.missing_tasks: GuidancePatchStats#missing_tasks.
  _inject_into_text: _inject_into_text().
  DEFAULT_GUIDANCE_HEADING: DEFAULT_GUIDANCE_HEADING.
  DEFAULT_INSERT_MARKER: DEFAULT_INSERT_MARKER.
  _task_name_from_metadata: _task_name_from_metadata().
---
# Module: [`OpenMLE-Evo/tts_search/validation_split_guidance.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py)

## Classes
### `GuidancePatchStats`
- def: [`OpenMLE-Evo/tts_search/validation_split_guidance.py:15`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L15)
- signature: `class GuidancePatchStats:`
- members:
  - `input_path` — [`L16`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L16)
  - `missing_tasks` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L20)
  - `output_path` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L17)
  - `patched_rows` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L19)
  - `skipped_existing_rows` — [`L21`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L21)
  - `total_rows` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L18)
- used by: [`patch_eval_data_with_guidance`](validation_split_guidance.md#patch_eval_data_with_guidance), [`_maybe_patch_eval_data_with_validation_guidance`](../scripts/evaluate_airaevo.md#_maybe_patch_eval_data_with_validation_guidance)  (1 test-only)

## Functions
- `_inject_guidance(prompt: Any, *, guidance: str, insert_marker: str, heading: str)` — [`L166`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L166)
- `_inject_into_text(text: str, guidance: str, insert_marker: str, heading: str)` — [`L202`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L202)
- `_patch_rows(*, rows: list[dict[str, Any]], guidance_map: dict[str, str], input_key: str, metadata_key: str, insert_marker: str, heading: str, strict: bool)` — [`L106`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L106)
- `_task_name_from_metadata(metadata: Any)` — [`L146`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L146)
- `load_guidance_map(instructions_path: Path)` — [`L24`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L24) — Parse task-specific validation guidance blocks from the markdown document.
- `patch_eval_data_with_guidance(*, eval_data_path: Path, output_path: Path, instructions_path: Path, input_key: str, metadata_key: str, insert_marker: str = DEFAULT_INSERT_MARKER, heading: str = DEFAULT_GUIDANCE_HEADING, strict: bool = False)` — [`L44`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L44)

## Module values
- `DEFAULT_GUIDANCE_HEADING` — [`L10`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L10)
- `DEFAULT_INSERT_MARKER` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/validation_split_guidance.py#L11)

