---
title: 'Module: OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.metadata_pipeline.sample_submission_validator`/
symbols:
  validate_sample_submission: validate_sample_submission().
  validate_sample_submissions: validate_sample_submissions().
  get_metric: get_metric().
  _load_module_from_path: _load_module_from_path().
  evaluate_submission: evaluate_submission().
---
# Module: [`OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py)

## Functions
- `_load_module_from_path(module_name: str, file_path: Path)` — [`L15`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py#L15) — Dynamically load a Python module directly from its file path.
- `evaluate_submission(metric, submission_path: Path, data_path: Path)` — [`L54`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py#L54)
- `get_metric(competition_name: str, data_dir: str | Path)` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py#L37) — Get the metric class for a specific competition.
- `validate_sample_submission(task_dir: str | Path)` — [`L61`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py#L61)
- `validate_sample_submissions(folders: list | None = None, csv_name: str | None = None)` — [`L106`](../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/sample_submission_validator.py#L106)

