---
title: 'Module: rdagent/app/rl/ui/rl_summary.py'
type: catalog
provenance: extracted
module: rdagent/app/rl/ui/rl_summary.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.rl.ui.rl_summary`/
symbols:
  get_job_summary_df: get_job_summary_df().
  render_job_summary: render_job_summary().
  get_max_loops: get_max_loops().
  style_df_with_decisions: style_df_with_decisions().
  style_df_with_decisions.apply_styles: style_df_with_decisions().apply_styles().
  is_valid_task: is_valid_task().
  get_loop_dirs: get_loop_dirs().
  get_loop_status: get_loop_status().
  style_status_cell: style_status_cell().
---
# Module: [`rdagent/app/rl/ui/rl_summary.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py)

## Functions
- `apply_styles(row_idx: int, col: str)` — [`L139`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L139)
- `get_job_summary_df(job_path: Path)` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L74) — Generate summary DataFrame for all tasks in job
- `get_loop_dirs(task_path: Path)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L18) — Get sorted list of Loop directories
- `get_loop_status(task_path: Path, loop_id: int)` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L24) — Get loop status and feedback decision.
- `get_max_loops(job_path: Path)` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L64) — Get maximum number of loops across all tasks
- `is_valid_task(task_path: Path)` — [`L13`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L13) — Check if directory is a valid RL task (has __session__ subdirectory)
- `render_job_summary(job_path: Path, is_root: bool = False)` — [`L152`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L152) — Render job summary UI
- `style_df_with_decisions(df: pd.DataFrame, decisions_df: pd.DataFrame)` — [`L136`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L136) — Apply styling to dataframe
- `style_status_cell(val: str, decision: bool | None = None)` — [`L119`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/rl_summary.py#L119) — Style cell based on status value

