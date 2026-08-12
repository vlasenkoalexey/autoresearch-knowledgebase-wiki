---
title: 'Module: OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.scripts.sft_data_selection.exclude_reserved_tasks`/
symbols:
  main: main().
  normalize_value: normalize_value().
  build_reserved_hash_index: build_reserved_hash_index().
  write_jsonl: write_jsonl().
  read_rows: read_rows().
  get_user_message: get_user_message().
  reserved_metadata: reserved_metadata().
  write_kept_data: write_kept_data().
  canonicalize_task_description: canonicalize_task_description().
  sha256_text: sha256_text().
  extract_task_description_from_user: extract_task_description_from_user().
  read_jsonl: read_jsonl().
  validate_manifest_order: validate_manifest_order().
  parse_args: parse_args().
---
# Module: [`OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py)

## Functions
- `build_reserved_hash_index(prompt_rows: list[dict[str, Any]])` — [`L99`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L99)
- `canonicalize_task_description(text: str)` — [`L24`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L24)
- `extract_task_description_from_user(user_text: str)` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L44)
- `get_user_message(messages: Any)` — [`L34`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L34)
- `main()` — [`L200`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L200)
- `normalize_value(value: Any)` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L14)
- `parse_args()` — [`L169`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L169)
- `read_jsonl(path: Path)` — [`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L68)
- `read_rows(path: Path)` — [`L83`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L83)
- `reserved_metadata(row: dict[str, Any])` — [`L92`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L92)
- `sha256_text(text: str)` — [`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L30)
- `validate_manifest_order(manifest_path: Path, ordered_metadata: list[dict[str, str]])` — [`L120`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L120)
- `write_jsonl(path: Path, rows: Iterable[dict[str, Any]])` — [`L142`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L142)
- `write_kept_data(input_path: Path, output_path: Path, kept_rows: list[dict[str, Any]], kept_indices: list[int], source_table: Any | None)` — [`L149`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/exclude_reserved_tasks.py#L149)

