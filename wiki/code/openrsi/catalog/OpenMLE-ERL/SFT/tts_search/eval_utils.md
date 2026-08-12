---
title: 'Module: OpenMLE-ERL/SFT/tts_search/eval_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/eval_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.eval_utils`/
symbols:
  write_summary_csv: write_summary_csv().
  write_epoch_stat: write_epoch_stat().
  ALL_TASK_LIST.ALL_TASK_LIST: ALL_TASK_LIST.ALL_TASK_LIST.
  build_submit_grade_and_medal: build_submit_grade_and_medal().
  get_medal_for_score: get_medal_for_score().
  write_global_stat.aggregate: write_global_stat().aggregate().
  write_global_stat: write_global_stat().
  get_medal_for_grade: get_medal_for_grade().
  load_leaderboard: load_leaderboard().
  get_grade_for_score: get_grade_for_score().
  write_summary_csv.std: write_summary_csv().std().
  write_summary_csv.mean: write_summary_csv().mean().
  write_epoch_stat.std: write_epoch_stat().std().
  write_global_stat.std: write_global_stat().std().
  is_lower_better: is_lower_better().
  LOW_TASK_LIST.LOW_TASK_LIST: LOW_TASK_LIST.LOW_TASK_LIST.
  MIDDLE_TASK_LIST.MIDDLE_TASK_LIST: MIDDLE_TASK_LIST.MIDDLE_TASK_LIST.
  HIGH_TASK_LIST.HIGH_TASK_LIST: HIGH_TASK_LIST.HIGH_TASK_LIST.
  TIME_SCALING_SCORE_SECONDS: TIME_SCALING_SCORE_SECONDS.
  _medal_positions: _medal_positions().
  write_epoch_stat.mean: write_epoch_stat().mean().
  write_global_stat.mean: write_global_stat().mean().
  write_summary_csv.epoch_index: write_summary_csv().epoch_index().
  write_global_stat.epoch_index: write_global_stat().epoch_index().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/eval_utils.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py)

## Functions
- `_medal_positions(num_teams: int)` — [`L137`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L137)
- `aggregate(values: list[float | None])` — [`L482`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L482)
- `build_submit_grade_and_medal(submit_score: float | None, leaderboard: pd.DataFrame | None)` — [`L196`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L196) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `epoch_index(path: Path)` — [`L306`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L306)
- `epoch_index(path: Path)` — [`L468`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L468)
- `get_grade_for_score(score: float, leaderboard: pd.DataFrame)` — [`L126`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L126)
- `get_medal_for_grade(grade: float, leaderboard: pd.DataFrame)` — [`L181`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L181)
- `get_medal_for_score(score: float, leaderboard: pd.DataFrame)` — [`L157`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L157)
- `is_lower_better(leaderboard: pd.DataFrame)` — [`L121`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L121)
- `load_leaderboard(metadata: dict[str, Any])` — [`L95`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L95) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `mean(values: list[float])` — [`L215`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L215)
- `mean(values: list[float])` — [`L310`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L310)
- `mean(values: list[float])` — [`L472`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L472)
- `std(values: list[float])` — [`L218`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L218)
- `std(values: list[float])` — [`L313`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L313)
- `std(values: list[float])` — [`L475`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L475)
- `write_epoch_stat(epoch_output_dir: Path)` — [`L206`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L206)
- `write_global_stat(output_dir: Path)` — [`L465`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L465)
- `write_summary_csv(output_dir: Path, task_metadata_map: dict[str, dict[str, Any]])` — [`L302`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L302)

## Module values
- `ALL_TASK_LIST` — [`L91`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L91)
- `HIGH_TASK_LIST` — [`L74`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L74)
- `LOW_TASK_LIST` — [`L10`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L10)
- `MIDDLE_TASK_LIST` — [`L34`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L34)
- `TIME_SCALING_SCORE_SECONDS` — [`L92`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/eval_utils.py#L92)

