---
title: 'Module: rdagent/app/finetune/llm/ui/ft_summary.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/ft_summary.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.ft_summary`/
symbols:
  get_job_summary_df: get_job_summary_df().
  render_job_summary: render_job_summary().
  get_task_full_benchmark_df: get_task_full_benchmark_df().
  get_loop_status: get_loop_status().
  get_max_loops: get_max_loops().
  render_task_detail_selector: render_task_detail_selector().
  extract_benchmark_score: extract_benchmark_score().
  extract_benchmark_scores: extract_benchmark_scores().
  extract_baseline_scores: extract_baseline_scores().
  style_df_with_decisions: style_df_with_decisions().
  style_df_with_decisions.apply_styles: style_df_with_decisions().apply_styles().
  is_valid_task: is_valid_task().
  extract_baseline_score: extract_baseline_score().
  get_loop_dirs: get_loop_dirs().
  style_status_cell: style_status_cell().
  extract_full_benchmark: extract_full_benchmark().
  extract_baseline_full_benchmark: extract_baseline_full_benchmark().
---
# Module: [`rdagent/app/finetune/llm/ui/ft_summary.py`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py)

## Functions
- `apply_styles(row_idx: int, col: str)` — [`L372`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L372)
- `extract_baseline_full_benchmark(task_path: Path, split: str = "validation")` — [`L457`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L457) — Extract full accuracy_summary from baseline scenario.
- `extract_baseline_score(task_path: Path)` — [`L73`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L73) — Extract baseline benchmark score from scenario object (legacy, validation only).
- `extract_baseline_scores(task_path: Path)` — [`L101`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L101) — Extract both validation and test baseline benchmark scores from scenario.
- `extract_benchmark_score(loop_path: Path, split: str = "")` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L27) — Extract benchmark score, metric name, and direction from loop directory.
- `extract_benchmark_scores(loop_path: Path)` — [`L60`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L60) — Extract both validation and test benchmark scores from loop directory.
- `extract_full_benchmark(loop_path: Path, split: str = "")` — [`L429`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L429) — Extract full accuracy_summary from loop directory.
- `get_job_summary_df(job_path: Path)` — [`L224`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L224) — Generate summary DataFrame and decision DataFrame for all tasks in job
- `get_loop_dirs(task_path: Path)` — [`L21`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L21) — Get sorted list of Loop directories
- `get_loop_status(task_path: Path, loop_id: int)` — [`L144`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L144) — Get loop status, validation score, test score, metric name with direction arrow, feedback decision, and direction.
- `get_max_loops(job_path: Path)` — [`L214`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L214) — Get maximum number of loops across all tasks
- `get_task_full_benchmark_df(task_path: Path, split: str)` — [`L490`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L490) — Generate full benchmark table for a single task and split.
- `is_valid_task(task_path: Path)` — [`L16`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L16) — Check if directory is a valid FT task (has __session__ subdirectory)
- `render_job_summary(job_path: Path, is_root: bool = False)` — [`L386`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L386) — Render job summary UI
- `render_task_detail_selector(job_path: Path)` — [`L554`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L554) — Render task selector dropdown and full benchmark tables.
- `style_df_with_decisions(df: pd.DataFrame, decisions_df: pd.DataFrame)` — [`L364`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L364) — Apply styling to dataframe based on decision data
- `style_status_cell(val: str, decision: bool | None = None)` — [`L318`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/ft_summary.py#L318) — Style cell based on status value and feedback decision

