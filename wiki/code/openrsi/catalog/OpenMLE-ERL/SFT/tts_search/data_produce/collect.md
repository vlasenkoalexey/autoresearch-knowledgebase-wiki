---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/collect.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/collect.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.collect`/
symbols:
  collect_sft_rows: collect_sft_rows().
  load_eval_results: load_eval_results().
  feedback_is_success: feedback_is_success().
  load_gen_results: load_gen_results().
  extract_feedback_status: extract_feedback_status().
  extract_feedback_result: extract_feedback_result().
  _rank_eval_row: _rank_eval_row().
  _build_rejection_policy: _build_rejection_policy().
  load_gen_results_by_request_id: load_gen_results_by_request_id().
  find_step_dir: find_step_dir().
  step_dir_from_eval_row: step_dir_from_eval_row().
  _step_key: _step_key().
  STATUS_RE: STATUS_RE.
  RESULT_RE: RESULT_RE.
  build_assistant_content: build_assistant_content().
  load_prompt_source: load_prompt_source().
  _source_prompt_for_row: _source_prompt_for_row().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/collect.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py)

## Functions
- `_build_rejection_policy(name: str | None)` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L77) — Lazily import rejection policy builder to avoid package import cycles. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `_rank_eval_row(row: dict[str, Any])` — [`L161`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L161) — Rank duplicate eval rows for deterministic collapse.
- `_source_prompt_for_row(*, task_id: str, task_name: str, by_task_id: dict[str, tuple[dict[str, Any], list[dict[str, Any]]]], by_task_name: dict[str, tuple[dict[str, Any], list[dict[str, Any]]]])` — [`L331`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L331) — Return source system/user prompt text for a result row.
- `_step_key(row: dict[str, Any])` — [`L146`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L146) — Build the join key for gen/eval step rows.
- `build_assistant_content(reasoning: str, code: str, response: str)` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L84) — Build the assistant message for an SFT row.
- `collect_sft_rows(*, run_dir: Path, source_parquet: Path, rejection_policy: RejectionPolicy | str | None = "accept_scored", min_reward: float | None = 0, eval_statuses: set[str] | None = None, require_feedback_success: bool = True, id_prefix: str = "sft_candidate")` — [`L358`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L358) — Collect evaluated rollouts as SFT training rows.
- `extract_feedback_result(feedback_text: str)` — [`L40`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L40) — Extract sandbox result label from formatted feedback.
- `extract_feedback_status(feedback_text: str)` — [`L27`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L27) — Extract sandbox status from formatted feedback.
- `feedback_is_success(feedback_text: str, *, status_values: set[str] | None = None, result_values: set[str] | None = None)` — [`L53`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L53) — Check whether feedback represents a successful run.
- `find_step_dir(run_dir: Path, *, task_name: str, task_id: str | None, step_index: int)` — [`L266`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L266) — Find the artifact directory for one generated step.
- `load_eval_results(path: Path)` — [`L184`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L184) — Load and deduplicate eval_results.jsonl.
- `load_gen_results(path: Path)` — [`L220`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L220) — Load latest generation row for each task step.
- `load_gen_results_by_request_id(path: Path)` — [`L242`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L242) — Load generation rows by request id, preserving same-step rollouts.
- `load_prompt_source(source_parquet: Path, *, metadata_col: str = "metadata", prompt_col: str = "prompt")` — [`L107`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L107) — Load source prompts indexed by task id and task name.
- `step_dir_from_eval_row(eval_row: dict[str, Any], run_dir: Path, *, task_name: str, task_id: str, step_index: int)` — [`L296`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L296) — Resolve the artifact directory for an eval row.

## Module values
- `RESULT_RE` — [`L24`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L24)
- `STATUS_RE` — [`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/collect.py#L23)

