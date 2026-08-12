---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.alignment`/
symbols:
  write_alignment_dataset: write_alignment_dataset().
  write_sampling_report: write_sampling_report().
  to_training_frame: to_training_frame().
  sample_tasks: sample_tasks().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py)

## Functions
- `sample_tasks(rows: list[dict[str, Any]], *, fractions: tuple[float, ...] = (0.5, 0.25), seed: int = 20260502, task_key: str = "task_id")` — [`L70`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py#L70) — Sample task ids and keep all rows for selected tasks.
- `to_training_frame(rows: list[dict[str, Any]])` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py#L14) — Return the minimal training format expected by SFT jobs.
- `write_alignment_dataset(rows: list[dict[str, Any]], *, output_dir: Path, name: str, write_manifest: bool = True)` — [`L29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py#L29) — Write JSONL, parquet, and optional manifest for SFT rows.
- `write_sampling_report(path: Path, summary: dict[str, Any])` — [`L125`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/alignment.py#L125) — Write a JSON sampling summary.

