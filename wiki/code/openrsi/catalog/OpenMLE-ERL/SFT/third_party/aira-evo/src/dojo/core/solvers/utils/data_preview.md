---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.data_preview`/
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
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py)

## Functions
- `_walk(path: Path, skip_hidden=True)` — [`L75`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L75) — Recursively walk a directory (analogous to os.walk but for pathlib.Path)
- `file_tree(path: Path, depth=0, skip_hidden=True)` — [`L51`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L51) — Generate a tree structure of files in a directory
- `generate(base_path, include_file_details=True, simple=False)` — [`L172`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L172) — Generate a textual preview of a directory, including an overview of the directory
- `get_file_len_size(f: Path)` — [`L30`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L30) — Calculate the size of a file (#lines for plaintext files, otherwise #bytes)
- `preview_csv(p: Path, file_name: str, simple=True)` — [`L94`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L94) — Generate a textual preview of a csv file
- `preview_json(p: Path, file_name: str)` — [`L142`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L142) — Generate a textual preview of a json file using a generated json schema

## Module values
- `code_files` — [`L25`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L25)
- `plaintext_files` — [`L27`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/data_preview.py#L27)

