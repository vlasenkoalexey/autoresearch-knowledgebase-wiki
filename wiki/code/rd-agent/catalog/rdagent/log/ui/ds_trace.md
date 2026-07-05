---
title: 'Module: rdagent/log/ui/ds_trace.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/ds_trace.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.ds_trace`/
symbols:
  llm_log_win: llm_log_win().
  summarize_win: summarize_win().
  load_data: load_data().
  main_win: main_win().
  loop_id: loop_id.
  available_models: available_models.
  default_index: default_index.
  workspace_win: workspace_win().
  exp_gen_win: exp_gen_win().
  running_win: running_win().
  max_id: max_id.
  coding_win: coding_win().
  stdout_win: stdout_win().
  evolving_win: evolving_win().
  timedelta_to_str: timedelta_to_str().
  day_srv: day_srv.
  convert_defaultdict_to_dict: convert_defaultdict_to_dict().
  llm_log_win.to_str_recursive: llm_log_win().to_str_recursive().
  sota_win: sota_win().
  get_llm_call_stats: get_llm_call_stats().
  folders: folders.
  show_text: show_text().
  summarize_win.style_dataframe_by_root: summarize_win().style_dataframe_by_root().
  replace_ep_path: replace_ep_path().
  min_id: min_id.
  feedback_win: feedback_win().
  get_folders_sorted: get_folders_sorted().
  hypothesis_win: hypothesis_win().
  get_state_data_range: get_state_data_range().
  load_stdout: load_stdout().
  task_win: task_win().
  highlight_prompts_uri: highlight_prompts_uri().
  get_timeout_stats: get_timeout_stats().
  summarize_win.style_dataframe_by_root.apply_color: summarize_win().style_dataframe_by_root().apply_color().
  summarize_win.comp_stat_func: summarize_win().comp_stat_func().
  day_map: day_map.
---
# Module: [`rdagent/log/ui/ds_trace.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py)

## Functions
- `apply_color(row)` — [`L932`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L932)
- `coding_win(data, base_exp, llm_data: dict | None = None)` — [`L452`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L452)
- `comp_stat_func(x: pd.DataFrame)` — [`L1002`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1002)
- `convert_defaultdict_to_dict(d)` — [`L68`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L68)
- `evolving_win(data, key, llm_data=None, base_workspace=None)` — [`L408`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L408)
- `exp_gen_win(exp_gen_data, llm_data=None)` — [`L394`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L394)
- `feedback_win(fb_data, llm_data=None)` — [`L524`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L524)
- `get_folders_sorted(log_path, sort_by_time=False)` — [`L1101`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1101) — Cache and return the sorted list of folders, with progress printing.
- `get_llm_call_stats(llm_data: dict)` — [`L621`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L621)
- `get_state_data_range(state_data)` — [`L1180`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1180)
- `get_timeout_stats(llm_data: dict)` — [`L643`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L643)
- `highlight_prompts_uri(uri)` — [`L257`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L257) — 高亮 URI 的格式
- `hypothesis_win(hypo)` — [`L387`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L387)
- `llm_log_win(llm_d: list)` — [`L265`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L265)
- `load_data(log_path: Path)` — [`L74`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L74) — Load and normalize logged data for the UI.
- `load_stdout(stdout_path: Path)` — [`L176`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L176)
- `main_win(loop_id, llm_data=None)` — [`L557`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L557)
- `replace_ep_path(p: Path)` — [`L609`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L609)
- `running_win(data, base_exp, llm_data=None, last_sota_exp=None)` — [`L488`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L488)
- `show_text(text, lang=None)` — [`L247`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L247) — 显示文本代码块
- `sota_win(sota_exp, trace)` — [`L540`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L540)
- `stdout_win(loop_id: int)` — [`L1077`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1077)
- `style_dataframe_by_root(df, root_nodes)` — [`L916`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L916)
- `summarize_win()` — [`L677`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L677) — documented in [rdagent-log-base](../../../../concepts/rdagent-log-base.md)
- `task_win(task)` — [`L185`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L185)
- `timedelta_to_str(td: timedelta | None)` — [`L667`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L667)
- `to_str_recursive(obj)` — [`L266`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L266)
- `workspace_win(workspace, cmp_workspace=None, cmp_name="last code.")` — [`L199`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L199)

## Module values
- `available_models` — [`L61`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L61)
- `day_map` — [`L1123`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1123)
- `day_srv` — [`L1124`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1124)
- `default_index` — [`L1148`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1148)
- `folders` — [`L1146`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1146)
- `loop_id` — [`L1200`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1200)
- `max_id` — [`L1198`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1198)
- `min_id` — [`L1198`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/ds_trace.py#L1198)

