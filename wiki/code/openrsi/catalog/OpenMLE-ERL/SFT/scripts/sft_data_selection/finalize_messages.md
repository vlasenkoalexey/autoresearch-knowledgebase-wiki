---
title: 'Module: OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.scripts.sft_data_selection.finalize_messages`/
symbols:
  main: main().
  normalize_for_json: normalize_for_json().
  full_message_tokens: full_message_tokens().
  normalized_message_text: normalized_message_text().
  message_hash: message_hash().
  write_rows: write_rows().
  deduplicate: deduplicate().
  write_jsonl: write_jsonl().
  parse_args: parse_args().
  add_shared_arguments: add_shared_arguments().
  read_rows: read_rows().
---
# Module: [`OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py)

## Functions
- `add_shared_arguments(parser: argparse.ArgumentParser)` — [`L126`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L126)
- `deduplicate(rows: list[dict[str, Any]])` — [`L81`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L81)
- `full_message_tokens(tokenizer: Any, messages: Any)` — [`L105`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L105)
- `main()` — [`L165`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L165)
- `message_hash(messages: Any)` — [`L32`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L32)
- `normalize_for_json(value: Any)` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L13)
- `normalized_message_text(messages: Any)` — [`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L23)
- `parse_args()` — [`L136`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L136)
- `read_rows(path: Path)` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L36)
- `write_jsonl(path: Path, rows: list[dict[str, Any]])` — [`L119`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L119)
- `write_rows(path: Path, rows: list[dict[str, Any]], *, source_table: Any | None, indices: list[int])` — [`L58`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/finalize_messages.py#L58)

