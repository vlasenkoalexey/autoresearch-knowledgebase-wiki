---
title: 'Module: OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.scripts.sft_data_selection.select_evolutionary`/
symbols:
  build_segments: build_segments().
  main: main().
  debug_descendants: debug_descendants().
  load_annotations: load_annotations().
  strict_score: strict_score().
  medal_rank: medal_rank().
  parent_scores_from_root: parent_scores_from_root().
  class_flags: class_flags().
  write_jsonl: write_jsonl().
  normalize_operator: normalize_operator().
  ROOT_OPERATORS: ROOT_OPERATORS.
  DEBUG_OPERATOR: DEBUG_OPERATOR.
  MEDAL_RANK: MEDAL_RANK.
  read_jsonl: read_jsonl().
  numeric_field: numeric_field().
  load_task_stat: load_task_stat().
  load_higher_is_better: load_higher_is_better().
  score_better_than_parents: score_better_than_parents().
  parse_index_list: parse_index_list().
  select_steps: select_steps().
  parse_args: parse_args().
---
# Module: [`OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py)

## Functions
- `build_segments(stat_root: Path)` — [`L202`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L202)
- `class_flags(*, segment_type: str, endpoint_score: float | None, endpoint_medal_rank: int, parent_scores: list[float], missing_parent_score_steps: list[int], higher_is_better: bool)` — [`L168`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L168)
- `debug_descendants(root_step: int, children: dict[int, list[int]], steps_by_index: dict[int, dict[str, Any]])` — [`L113`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L113)
- `load_annotations(path: Path | None)` — [`L283`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L283)
- `load_higher_is_better(task_dir: Path)` — [`L104`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L104)
- `load_task_stat(stat_path: Path)` — [`L81`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L81)
- `main()` — [`L387`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L387)
- `medal_rank(value: Any)` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L77)
- `normalize_operator(value: Any)` — [`L55`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L55)
- `numeric_field(obj: dict[str, Any] | None, key: str)` — [`L60`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L60)
- `parent_scores_from_root(root: dict[str, Any], steps_by_index: dict[int, dict[str, Any]])` — [`L132`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L132)
- `parse_args()` — [`L365`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L365)
- `parse_index_list(value: Any)` — [`L271`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L271)
- `read_jsonl(path: Path)` — [`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L30)
- `score_better_than_parents(*, endpoint_score: float | None, parent_scores: list[float], higher_is_better: bool, allow_missing_parent_by_positive_endpoint: bool)` — [`L153`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L153)
- `select_steps(segments: list[dict[str, Any]], annotations: dict[str, list[int]], stat_root: Path)` — [`L313`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L313)
- `strict_score(obj: dict[str, Any] | None)` — [`L73`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L73)
- `write_jsonl(path: Path, rows: Iterable[dict[str, Any]])` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L45)

## Module values
- `DEBUG_OPERATOR` — [`L16`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L16)
- `MEDAL_RANK` — [`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L17)
- `ROOT_OPERATORS` — [`L15`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_evolutionary.py#L15)

