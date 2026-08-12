---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.analysis_utils.meta_error_summary`/
symbols:
  slurm_id_to_log: slurm_id_to_log().
  summarize_single_crash: summarize_single_crash().
  generate_error_reports: generate_error_reports().
  save_dir: save_dir.
  final_report_from_summaries: final_report_from_summaries().
  gather_submitit_data: gather_submitit_data().
  create_client: create_client().
  log_dir: log_dir.
  get_last_approx_tokens: get_last_approx_tokens().
  likely_crashed: likely_crashed().
  job_summary_schema: job_summary_schema.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py)

## Functions
- `create_client()` — [`L22`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L22)
- `final_report_from_summaries(summaries)` — [`L233`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L233) — Takes a list of per-job summaries (in JSON form) and does
- `gather_submitit_data(logs_folder, job_ids)` — [`L94`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L94) — - Walks the logs_folder.
- `generate_error_reports(log_dir, save_dir)` — [`L274`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L274) — 1. Gather data from logs.
- `get_last_approx_tokens(filepath, approx_token_count=70000, avg_chars_per_token=4)` — [`L30`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L30) — Returns approximately the last `approx_token_count` tokens from a file.
- `likely_crashed(log_text)` — [`L74`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L74) — Simple heuristic to guess if a job crashed
- `slurm_id_to_log(logs_folder)` — [`L61`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L61) — Extracts 'Output dir: *' from *.out files, cleaning ANSI escape characters.
- `summarize_single_crash(job, job_to_name)` — [`L162`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L162)

## Module values
- `job_summary_schema` — [`L130`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L130)
- `log_dir` — [`L327`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L327)
- `save_dir` — [`L330`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/analysis_utils/meta_error_summary.py#L330)

