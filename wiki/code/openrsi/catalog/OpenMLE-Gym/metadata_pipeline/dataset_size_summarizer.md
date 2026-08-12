---
title: 'Module: OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.metadata_pipeline.dataset_size_summarizer`/
symbols:
  annotate_dataset_sizes: annotate_dataset_sizes().
  format_size: format_size().
  _directory_size: _directory_size().
---
# Module: [`OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py)

## Functions
- `_directory_size(path: Path)` — [`L24`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py#L24)
- `annotate_dataset_sizes(all_subdirs: list[Path] | None = None, csv_name: str = "overview.csv", timeout: int = 5)` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py#L38) — Update Raw Size and Final Size columns in an overview CSV.
- `format_size(size_bytes: int)` — [`L14`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/dataset_size_summarizer.py#L14) — Return a human-readable size string.

