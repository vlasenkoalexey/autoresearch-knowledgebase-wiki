---
title: 'Module: OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.scripts.sft_data_selection.select_parallel`/
symbols:
  main: main().
  select_joint_top4: select_joint_top4().
  select_glm_top4_unique_score: select_glm_top4_unique_score().
  task_value: task_value().
  numeric_score: numeric_score().
  stable_id: stable_id().
  read_jsonl: read_jsonl().
  write_jsonl: write_jsonl().
  generator_family: generator_family().
  parse_args: parse_args().
---
# Module: [`OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py)

## Functions
- `generator_family(row: dict[str, Any], field: str)` — [`L64`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L64)
- `main()` — [`L219`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L219)
- `numeric_score(row: dict[str, Any], field: str)` — [`L39`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L39)
- `parse_args()` — [`L197`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L197)
- `read_jsonl(path: Path)` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L14)
- `select_glm_top4_unique_score(rows: list[dict[str, Any]], *, task_field: str, score_field: str, id_field: str)` — [`L79`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L79) — Deduplicate equal scores per task, then retain the highest four.
- `select_joint_top4(rows: list[dict[str, Any]], *, task_field: str, score_field: str, id_field: str, family_field: str)` — [`L135`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L135) — Apply the historical mixed-family joint Top-4 policy.
- `stable_id(row: dict[str, Any], field: str)` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L57)
- `task_value(row: dict[str, Any], field: str)` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L50)
- `write_jsonl(path: Path, rows: Iterable[dict[str, Any]])` — [`L29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/scripts/sft_data_selection/select_parallel.py#L29)

