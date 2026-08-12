---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/selection.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/selection.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.selection`/
symbols:
  select_top_per_task: select_top_per_task().
  _build_rejection_policy: _build_rejection_policy().
  _sort_rows_for_selection: _sort_rows_for_selection().
  merge_new_with_old_data: merge_new_with_old_data().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/selection.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/selection.py)

## Functions
- `_build_rejection_policy(**kwargs)` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/selection.py#L13) — Lazily import rejection policy builder to avoid package import cycles. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `_sort_rows_for_selection(df: pd.DataFrame, *, task_key: str, rank_fields: tuple[str, ...])` — [`L20`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/selection.py#L20) — Sort rows deterministically before per-task selection.
- `merge_new_with_old_data(*, new_train: pd.DataFrame, new_manifest: pd.DataFrame, old_train: pd.DataFrame, old_manifest: pd.DataFrame, task_key: str = "task_id", drop_new_when_new_le: int | None = 1, drop_new_when_old_between: tuple[int, int] | None = (3, 4))` — [`L136`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/selection.py#L136) — Merge new SFT rows with old rows while handling task overlap.
- `select_top_per_task(rows: list[dict[str, Any]], *, top_k: int = 4, task_key: str = "task_id", dedupe_field: str | None = "reward", rank_fields: tuple[str, ...] = ("reward", "score"), rejection_policy: RejectionPolicy | str | None = "accept_scored", rejection_score_threshold: float | None = None, rejection_reward_threshold: float | None = None)` — [`L49`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/selection.py#L49) — Apply rejection policy, dedupe, then keep top-k rows per task.

