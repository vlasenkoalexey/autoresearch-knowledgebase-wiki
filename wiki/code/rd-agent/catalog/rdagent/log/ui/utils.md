---
title: 'Module: rdagent/log/ui/utils.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.utils`/
symbols:
  get_sota_exp_stat: get_sota_exp_stat().
  get_summary_df: get_summary_df().
  load_times_info: load_times_info().
  get_score_stat: get_score_stat().
  trace_figure: trace_figure().
  get_best_report: get_best_report().
  compare: compare().
  trace_figure.get_display_name: trace_figure().get_display_name().
  ALL: ALL.
  _log_path_hash_func: _log_path_hash_func().
  load_times_deprecated: load_times_deprecated().
  app: app.
  percent_df: percent_df().
  get_summary_df.compare_score: get_summary_df().compare_score().
  curve_figure: curve_figure().
  _get_sota_exp_stat_hash_func: _get_sota_exp_stat_hash_func().
  _get_score_stat_hash_func: _get_score_stat_hash_func().
  _log_folders_summary_hash_func: _log_folders_summary_hash_func().
  compare.apply_func: compare().apply_func().
  LITE: LITE.
  HIGH: HIGH.
  MEDIUM: MEDIUM.
  get_statistics_df: get_statistics_df().
  lite_curve_figure: lite_curve_figure().
  trace_figure.parent_avg_pos: trace_figure().parent_avg_pos().
  timeline_figure: timeline_figure().
  get_script_time: get_script_time().
  map_stat: map_stat().
  percent_df.num2percent: percent_df().num2percent().
---
# Module: [`rdagent/log/ui/utils.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py)

## Functions
- `_get_score_stat_hash_func(log_path: Path, sota_loop_id: int)` — [`L262`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L262)
- `_get_sota_exp_stat_hash_func(log_path: Path, selector: Literal["auto", "best_valid"] = "auto")` — [`L182`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L182)
- `_log_folders_summary_hash_func(log_folder: str | Path, hours: int | None = None)` — [`L423`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L423)
- `_log_path_hash_func(log_path: Path)` — [`L134`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L134)
- `apply_func(cdf: pd.DataFrame)` — [`L1103`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L1103)
- `compare(exp_list: list[str] = typer.Option(..., "--exp-list", help="List of experiment names.", show_default=False), output: str = typer.Option("merge_base_df.h5", help="Output summary file name."), hours: int | None = typer.Option(None, help="if None, use summary.pkl, else summary_{hours}h.pkl"), select_best: bool = typer.Option(False, help="Select best experiment for each competition."))` — [`L1089`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L1089) — Generate summary and base dataframe for given experiment list, and save to a summary file.
- `compare_score(s1, s2)` — [`L560`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L560)
- `curve_figure(scores: pd.DataFrame)` — [`L783`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L783) — scores.columns.name is the metric name, e.g., "accuracy", "f1", etc.
- `get_best_report(log_path: Path)` — [`L164`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L164)
- `get_display_name(idx: int)` — [`L892`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L892) — Convert to index in the queue (enque id) to loop_idx for easier understanding.
- `get_score_stat(log_path: Path, sota_loop_id: int)` — [`L266`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L266) — Get the scores before and after merge period. — documented in [rdagent-log-base](../../../../concepts/rdagent-log-base.md)
- `get_script_time(stdout_p: Path)` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L117)
- `get_sota_exp_stat(log_path: Path, selector: Literal["auto", "best_valid"] = "auto")` — [`L186`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L186) — Get the SOTA experiment and its statistics from the log path. — documented in [rdagent-log-base](../../../../concepts/rdagent-log-base.md)
- `get_statistics_df(summary_df: pd.DataFrame)` — [`L712`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L712)
- `get_summary_df(log_folder: str | Path, hours: int | None = None)` — [`L432`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L432) — Process experiment logs and generate summary DataFrame.
- `lite_curve_figure(summary)` — [`L818`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L818)
- `load_times_deprecated(log_path: Path)` — [`L365`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L365)
- `load_times_info(log_path: Path)` — [`L382`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L382) — Load timing information for each loop and step.
- `map_stat(sota_mle_score: dict | None)` — [`L146`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L146)
- `num2percent(num: int, total: int, show_origin=True)` — [`L690`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L690)
- `parent_avg_pos(node)` — [`L945`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L945)
- `percent_df(summary_df: pd.DataFrame, show_origin=True)` — [`L668`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L668) — Convert the summary DataFrame to a percentage format.
- `timeline_figure(times_dict: dict[int, dict[str, dict[Literal["start_time", "end_time"], datetime]]])` — [`L975`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L975)
- `trace_figure(trace: Trace, merge_loops: list = [])` — [`L884`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L884)

## Module values
- `ALL` — [`L114`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L114)
- `HIGH` — [`L55`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L55)
- `LITE` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L30)
- `MEDIUM` — [`L73`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L73)
- `app` — [`L1126`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/utils.py#L1126)

