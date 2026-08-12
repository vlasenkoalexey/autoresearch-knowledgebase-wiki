---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.tasks.mlebench.utils.data`/
symbols:
  extract_all_from_path: extract_all_from_path().
  logger: logger.
  tar_directory: tar_directory().
  extract_all_from_path.extract: extract_all_from_path().extract().
  extract_all_from_path.is_compressed: extract_all_from_path().is_compressed().
  get_competition_ids_in_split: get_competition_ids_in_split().
  TASK_DIR: TASK_DIR.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py)

## Functions
- `extract(file: Path, dst: Path)` — [`L43`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L43) — Extracts a compressed file to the specified destination.
- `extract_all_from_path(path: Path, already_extracted: set = set(), force: bool = True, delete_compressed: bool = False)` — [`L38`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L38) — Extracts the contents of a compressed file to a destination directory.
- `get_competition_ids_in_split(split_id)` — [`L29`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L29)
- `is_compressed(file: Path)` — [`L71`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L71) — Check if the file is a compressed format that we can handle.
- `tar_directory(root_dir, output_file)` — [`L20`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L20)

## Module values
- `TASK_DIR` — [`L17`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L17)
- `logger` — [`L15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/tasks/mlebench/utils/data.py#L15)

