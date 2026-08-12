---
title: 'Module: OpenMLE-Evo/tts_search/eval_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/eval_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.eval_utils`/
symbols:
  write_summary_csv: write_summary_csv().
  write_epoch_stat: write_epoch_stat().
  write_time_scaling: write_time_scaling().
  get_medal_for_grade: get_medal_for_grade().
  write_global_stat: write_global_stat().
  build_submit_grade_and_medal: build_submit_grade_and_medal().
  write_global_stat.aggregate: write_global_stat().aggregate().
  _level_tasks_for: _level_tasks_for().
  ALL_TASK_LIST.ALL_TASK_LIST: ALL_TASK_LIST.ALL_TASK_LIST.
  TIME_SCALING_SCORE_SECONDS: TIME_SCALING_SCORE_SECONDS.
  get_total_model_plus_sandbox_time: get_total_model_plus_sandbox_time().
  _read_json_file: _read_json_file().
  load_leaderboard: load_leaderboard().
  write_summary_csv.std: write_summary_csv().std().
  get_medal_for_score: get_medal_for_score().
  write_summary_csv.mean: write_summary_csv().mean().
  write_epoch_stat.std: write_epoch_stat().std().
  get_grade_for_score: get_grade_for_score().
  logger: logger.
  write_epoch_stat.mean: write_epoch_stat().mean().
  write_global_stat.std: write_global_stat().std().
  get_total_sandbox_time: get_total_sandbox_time().
  is_lower_better: is_lower_better().
  _ordered_unique: _ordered_unique().
  get_total_model_time: get_total_model_time().
  _medal_positions: _medal_positions().
  write_global_stat.mean: write_global_stat().mean().
  LOW_TASK_LIST.LOW_TASK_LIST: LOW_TASK_LIST.LOW_TASK_LIST.
  MIDDLE_TASK_LIST.MIDDLE_TASK_LIST: MIDDLE_TASK_LIST.MIDDLE_TASK_LIST.
  HIGH_TASK_LIST.HIGH_TASK_LIST: HIGH_TASK_LIST.HIGH_TASK_LIST.
  write_summary_csv.epoch_index: write_summary_csv().epoch_index().
  write_global_stat.epoch_index: write_global_stat().epoch_index().
  write_time_scaling.epoch_index: write_time_scaling().epoch_index().
---
# Module: [`OpenMLE-Evo/tts_search/eval_utils.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py)

## Functions
- `_level_tasks_for(task_names: list[str])` — [`L124`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L124) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `_medal_positions(num_teams: int)` — [`L207`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L207) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `_ordered_unique(values: list[str] | tuple[str, ...] | None)` — [`L98`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L98) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `_read_json_file(path: Path)` — [`L112`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L112) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `aggregate(values: list[float | None])` — [`L755`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L755)
- `build_submit_grade_and_medal(submit_score: float | None, leaderboard: pd.DataFrame | None)` — [`L266`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L266)
- `epoch_index(path: Path)` — [`L489`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L489)
- `epoch_index(path: Path)` — [`L741`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L741)
- `epoch_index(path: Path)` — [`L899`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L899)
- `get_grade_for_score(score: float, leaderboard: pd.DataFrame)` — [`L196`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L196) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `get_medal_for_grade(grade: float, leaderboard: pd.DataFrame)` — [`L251`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L251) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `get_medal_for_score(score: float, leaderboard: pd.DataFrame)` — [`L227`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L227)
- `get_total_model_plus_sandbox_time(payload: dict[str, Any])` — [`L143`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L143) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `get_total_model_time(payload: dict[str, Any])` — [`L133`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L133) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `get_total_sandbox_time(payload: dict[str, Any])` — [`L137`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L137) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `is_lower_better(leaderboard: pd.DataFrame)` — [`L191`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L191) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `load_leaderboard(metadata: dict[str, Any])` — [`L149`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L149) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `mean(values: list[float])` — [`L291`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L291)
- `mean(values: list[float])` — [`L493`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L493)
- `mean(values: list[float])` — [`L745`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L745)
- `std(values: list[float])` — [`L294`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L294)
- `std(values: list[float])` — [`L496`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L496)
- `std(values: list[float])` — [`L748`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L748)
- `write_epoch_stat(epoch_output_dir: Path, expected_task_names: list[str] | tuple[str, ...] | None = None)` — [`L276`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L276) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `write_global_stat(output_dir: Path)` — [`L738`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L738)
- `write_summary_csv(output_dir: Path, task_metadata_map: dict[str, dict[str, Any]], expected_task_names: list[str] | tuple[str, ...] | None = None)` — [`L484`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L484) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `write_time_scaling(output_dir: Path)` — [`L898`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L898) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)

## Module values
- `ALL_TASK_LIST` — [`L94`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L94)
- `HIGH_TASK_LIST` — [`L77`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L77) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `LOW_TASK_LIST` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L13) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `MIDDLE_TASK_LIST` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L37) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `TIME_SCALING_SCORE_SECONDS` — [`L95`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L95) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `logger` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/eval_utils.py#L11) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)

