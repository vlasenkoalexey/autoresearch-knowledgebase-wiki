---
title: 'Module: OpenMLE-Gym/builder_core/tools/tools.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/builder_core/tools/tools.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.builder_core.tools.tools`/
symbols:
  configure_task_paths: configure_task_paths().
  save: save().
  list_directory_contents: list_directory_contents().
  read_txt_md: read_txt_md().
  _READ_ROOT._READ_ROOT: _READ_ROOT._READ_ROOT.
  _resolve_read_path: _resolve_read_path().
  get_csv_summary: get_csv_summary().
  _SAVE_PATH._SAVE_PATH: _SAVE_PATH._SAVE_PATH.
  _resolve_save_path: _resolve_save_path().
---
# Module: [`OpenMLE-Gym/builder_core/tools/tools.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py)

## Functions
- `_resolve_read_path(value: str)` — [`L19`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L19)
- `_resolve_save_path(value: str)` — [`L36`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L36)
- `configure_task_paths(read_root: str | Path, save_path: str | Path)` — [`L12`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L12) — Bind tool access to one task. Each task runs in its own process.
- `get_csv_summary(csv_path: str)` — [`L106`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L106) — Analyzes a CSV file and returns a summary. Limits analysis to the first `max_cols` columns to ensure readability and performance.
- `list_directory_contents(path: str)` — [`L46`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L46) — Lists the contents of the specified path.
- `read_txt_md(file_path: str)` — [`L171`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L171) — Display a bounded preview of a text file. One preview is sufficient for inventory.
- `save(info_path: str, content: str)` — [`L195`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L195) — Fully overwrite the content in fileinfo.txt. The only EXIT of tool use. Call this to save, and terminate the tool use.

## Module values
- `_READ_ROOT` — [`L8`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L8)
- `_SAVE_PATH` — [`L9`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/tools/tools.py#L9)

