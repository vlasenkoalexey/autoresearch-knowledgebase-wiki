---
title: 'Module: tools/edit.py'
type: catalog
provenance: extracted
module: tools/edit.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `tools.edit`/
symbols:
  tool_function: tool_function().
  view_path: view_path().
  result: result.
  format_output: format_output().
  write_file: write_file().
  maybe_truncate: maybe_truncate().
  validate_path: validate_path().
  read_file: read_file().
  tool_info: tool_info().
---
# Module: [`tools/edit.py`](../../../../../raw/code/dgm/tools/edit.py)

## Functions
- `format_output(content: str, path: str, init_line: int = 1)` — [`L75`](../../../../../raw/code/dgm/tools/edit.py#L75) — Format output with line numbers (for file content).
- `maybe_truncate(content: str, max_length: int = 10000)` — [`L35`](../../../../../raw/code/dgm/tools/edit.py#L35) — Truncate long content and add marker.
- `read_file(path: Path)` — [`L85`](../../../../../raw/code/dgm/tools/edit.py#L85) — Read and return the entire file contents.
- `tool_function(command: str, path: str, file_text: str = None)` — [`L122`](../../../../../raw/code/dgm/tools/edit.py#L122) — Main tool function that handles:
- `tool_info()` — [`L4`](../../../../../raw/code/dgm/tools/edit.py#L4)
- `validate_path(path: str, command: str)` — [`L41`](../../../../../raw/code/dgm/tools/edit.py#L41) — Validate the file path for each command:
- `view_path(path_obj: Path)` — [`L99`](../../../../../raw/code/dgm/tools/edit.py#L99) — View the entire file contents or directory listing.
- `write_file(path: Path, content: str)` — [`L92`](../../../../../raw/code/dgm/tools/edit.py#L92) — Write (overwrite) entire file contents.

## Module values
- `result` — [`L155`](../../../../../raw/code/dgm/tools/edit.py#L155)

