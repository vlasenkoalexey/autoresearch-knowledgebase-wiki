---
title: 'Module: rdagent/log/ui/llm_st.py'
type: catalog
provenance: extracted
module: rdagent/log/ui/llm_st.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.ui.llm_st`/
symbols:
  v: v.
  t3: t3.
  loop_id: loop_id.
  current_loop: current_loop.
  evo_anchor: evo_anchor.
  col5: col5.
  rdict: rdict.
  loop_data: loop_data.
  func_anchor: func_anchor.
  resp: resp.
  loop_anchor: loop_anchor.
  obj: obj.
  folders: folders.
  main_log_path: main_log_path.
  tag: tag.
  total_loops: total_loops.
  rd: rd.
  evo_id: evo_id.
  tlist: tlist.
  func_name: func_name.
  total_pages: total_pages.
  code: code.
  spec: spec.
  toc: toc.
  k: k.
  loop_groups: loop_groups.
  d: d.
  parser: parser.
  args: args.
  sorted_loop_ids: sorted_loop_ids.
  show_text: show_text().
  load_data: load_data().
  manually: manually.
  uri: uri.
  tpl: tpl.
  cxt: cxt.
  system: system.
  user: user.
  get_folders_sorted: get_folders_sorted().
  progress_text: progress_text.
  t1: t1.
  t2: t2.
  showed_keys: showed_keys.
  highlight_prompts_uri: highlight_prompts_uri().
  progress_bar: progress_bar.
  col1: col1.
  col2: col2.
  col3: col3.
  col4: col4.
  LOOPS_PER_PAGE: LOOPS_PER_PAGE.
  i: i.
---
# Module: [`rdagent/log/ui/llm_st.py`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py)

## Functions
- `get_folders_sorted(log_path)` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L22) — 缓存并返回排序后的文件夹列表，并加入进度打印
- `highlight_prompts_uri(uri)` — [`L93`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L93) — 高亮 URI 的格式
- `load_data()` — [`L52`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L52) — 加载数据到 session_state 并显示进度
- `show_text(text, lang=None)` — [`L83`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L83) — 显示文本代码块

## Module values
- `LOOPS_PER_PAGE` — [`L104`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L104)
- `args` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L19)
- `code` — [`L273`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L273)
- `col1` — [`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L188)
- `col2` — [`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L188)
- `col3` — [`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L188)
- `col4` — [`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L188)
- `col5` — [`L188`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L188)
- `current_loop` — [`L212`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L212)
- `cxt` — [`L253`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L253)
- `d` — [`L108`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L108)
- `evo_anchor` — [`L239`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L239)
- `evo_id` — [`L232`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L232)
- `folders` — [`L74`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L74)
- `func_anchor` — [`L234`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L234)
- `func_name` — [`L231`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L231)
- `i` — [`L108`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L108)
- `k` — [`L285`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L285)
- `loop_anchor` — [`L221`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L221)
- `loop_data` — [`L227`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L227)
- `loop_groups` — [`L107`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L107)
- `loop_id` — [`L110`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L110)
- `main_log_path` — [`L39`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L39)
- `manually` — [`L70`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L70)
- `obj` — [`L230`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L230)
- `parser` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L17)
- `progress_bar` — [`L101`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L101)
- `progress_text` — [`L100`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L100)
- `rd` — [`L254`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L254)
- `rdict` — [`L271`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L271)
- `resp` — [`L266`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L266)
- `showed_keys` — [`L284`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L284)
- `sorted_loop_ids` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L117)
- `spec` — [`L278`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L278)
- `system` — [`L264`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L264)
- `t1` — [`L256`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L256)
- `t2` — [`L256`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L256)
- `t3` — [`L256`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L256)
- `tag` — [`L109`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L109)
- `tlist` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L49)
- `toc` — [`L305`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L305)
- `total_loops` — [`L118`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L118)
- `total_pages` — [`L119`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L119)
- `tpl` — [`L252`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L252)
- `uri` — [`L251`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L251)
- `user` — [`L265`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L265)
- `v` — [`L285`](../../../../../../../raw/code/rd-agent/rdagent/log/ui/llm_st.py#L285)

