---
title: 'Module: ai_scientist/treesearch/utils/data_preview.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/data_preview.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.data_preview`/
symbols:
  generate: generate().
  file_tree: file_tree().
  plaintext_files: plaintext_files.
  get_file_len_size: get_file_len_size().
  _walk: _walk().
  code_files: code_files.
  preview_csv: preview_csv().
  preview_json: preview_json().
---
# Module: [`ai_scientist/treesearch/utils/data_preview.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py)

## Functions
- `_walk(path: Path)` — [`L50`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L50) — Recursively walk a directory (analogous to os.walk but for pathlib.Path)
- `file_tree(path: Path, depth=0)` — [`L32`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L32) — Generate a tree structure of files in a directory
- `generate(base_path, include_file_details=True, simple=False)` — [`L121`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L121) — Generate a textual preview of a directory, including an overview of the directory
- `get_file_len_size(f: Path)` — [`L19`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L19) — Calculate the size of a file (#lines for plaintext files, otherwise #bytes)
- `preview_csv(p: Path, file_name: str, simple=True)` — [`L59`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L59) — Generate a textual preview of a csv file
- `preview_json(p: Path, file_name: str)` — [`L111`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L111) — Generate a textual preview of a json file using a generated json schema

## Module values
- `code_files` — [`L14`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L14)
- `plaintext_files` — [`L16`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/data_preview.py#L16)

