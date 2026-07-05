---
title: 'Module: rdagent/log/ui/app.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/app.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.app`/
symbols:
  feedback_window: feedback_window().
  summary_window: summary_window().
  tasks_window: tasks_window().
  evolving_window: evolving_window().
  get_msgs_until: get_msgs_until().
  round: round.
  research_window: research_window().
  refresh: refresh().
  d_c: d_c.
  SIMILAR_SCENARIOS: SIMILAR_SCENARIOS.
  evolving_feedback_window: evolving_feedback_window().
  c2: c2.
  main_log_path: main_log_path.
  folders: folders.
  toc: toc.
  should_display: should_display().
  display_hypotheses: display_hypotheses().
  css: css.
  dcol2: dcol2.
  args: args.
  debug: debug.
  theme: theme.
  metrics_window.hypothesis_hover_text: metrics_window().hypothesis_hover_text().
  manually: manually.
  img_path: img_path.
  lc2: lc2.
  header_c3: header_c3.
  parser: parser.
  r_options: r_options.
  metrics_window: metrics_window().
  scen_c: scen_c.
  QLIB_SELECTED_METRICS: QLIB_SELECTED_METRICS.
  tabs_hint: tabs_hint().
  filter_log_folders: filter_log_folders().
  rf_c: rf_c.
  display_hypotheses.style_rows: display_hypotheses().style_rows().
  display_hypotheses.style_columns: display_hypotheses().style_columns().
  analyze_task_completion: analyze_task_completion().
  lc1: lc1.
  c1: c1.
  dcol1: dcol1.
  header_c1: header_c1.
  image_c: image_c.
---
# Module: [`rdagent/log/ui/app.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py)

## Functions
- `analyze_task_completion()` — [`L866`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L866)
- `display_hypotheses(hypotheses: dict[int, Hypothesis], decisions: dict[int, bool], success_only: bool = False)` — [`L327`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L327)
- `evolving_feedback_window(wsf: FactorSingleFeedback | ModelSingleFeedback)` — [`L292`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L292)
- `evolving_window()` — [`L670`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L670)
- `feedback_window()` — [`L586`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L586)
- `filter_log_folders(main_log_path)` — [`L72`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L72) — Filter and return the log folders relative to the main log path.
- `get_msgs_until(end_func: Callable[[Message], bool] = lambda _: True)` — [`L142`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L142)
- `hypothesis_hover_text(h: Hypothesis, d: bool = False)` — [`L373`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L373)
- `metrics_window(df: pd.DataFrame, R: int, C: int, *, height: int = 300, colors: list[str] = None)` — [`L370`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L370)
- `refresh(same_trace: bool = False)` — [`L258`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L258)
- `research_window()` — [`L550`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L550)
- `should_display(msg: Message)` — [`L131`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L131)
- `style_columns(col)` — [`L361`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L361)
- `style_rows(row)` — [`L356`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L356)
- `summary_window()` — [`L424`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L424)
- `tabs_hint()` — [`L501`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L501)
- `tasks_window(tasks: list[FactorTask | ModelTask])` — [`L508`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L508)

## Module values
- `QLIB_SELECTED_METRICS` — [`L56`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L56)
- `SIMILAR_SCENARIOS` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L63)
- `args` — [`L46`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L46)
- `c1` — [`L767`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L767)
- `c2` — [`L767`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L767)
- `css` — [`L856`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L856)
- `d_c` — [`L1110`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L1110)
- `dcol1` — [`L803`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L803)
- `dcol2` — [`L803`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L803)
- `debug` — [`L791`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L791)
- `folders` — [`L762`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L762)
- `header_c1` — [`L830`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L830)
- `header_c3` — [`L830`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L830)
- `image_c` — [`L846`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L846)
- `img_path` — [`L848`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L848)
- `lc1` — [`L754`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L754)
- `lc2` — [`L754`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L754)
- `main_log_path` — [`L48`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L48)
- `manually` — [`L758`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L758)
- `parser` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L43)
- `r_options` — [`L1103`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L1103)
- `rf_c` — [`L1110`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L1110)
- `round` — [`L1106`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L1106)
- `scen_c` — [`L846`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L846)
- `theme` — [`L853`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L853)
- `toc` — [`L728`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/app.py#L728)

