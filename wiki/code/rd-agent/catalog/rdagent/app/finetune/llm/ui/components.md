---
title: 'Module: rdagent/app/finetune/llm/ui/components.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/components.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.components`/
symbols:
  render_event: render_event().
  render_loop: render_loop().
  _render_loop_content: _render_loop_content().
  render_session: render_session().
  render_evo_loop: render_evo_loop().
  render_docker_exec: render_docker_exec().
  render_summary: render_summary().
  render_llm_call: render_llm_call().
  render_feedback: render_feedback().
  render_benchmark_result: render_benchmark_result().
  format_duration: format_duration().
  convert_latex_for_streamlit: convert_latex_for_streamlit().
  _render_single_feedback: _render_single_feedback().
  render_scenario: render_scenario().
  render_dataset_selection: render_dataset_selection().
  render_hypothesis: render_hypothesis().
  render_settings: render_settings().
  render_template: render_template().
  render_experiment: render_experiment().
  render_code: render_code().
  _extract_evaluator_name: _extract_evaluator_name().
  render_token: render_token().
  render_time_info: render_time_info().
  render_generic: render_generic().
  render_training_result: render_training_result().
---
# Module: [`rdagent/app/finetune/llm/ui/components.py`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py)

## Functions
- `_extract_evaluator_name(title: str)` — [`L410`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L410) — Extract evaluator name from event title like 'Eval (Data Processing) ✓'.
- `_render_loop_content(loop: Loop, show_types: list[str])` — [`L124`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L124) — Render loop content (called after lazy load)
- `_render_single_feedback(fb: Any, evaluator_name: str = "")` — [`L416`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L416) — Render a single CoSTEERSingleFeedback object.
- `convert_latex_for_streamlit(text: str)` — [`L17`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L17) — Convert LaTeX syntax to Streamlit-compatible format.
- `format_duration(seconds: float | None)` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L32)
- `render_benchmark_result(content: dict)` — [`L665`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L665) — Render benchmark evaluation result
- `render_code(content: Any)` — [`L392`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L392)
- `render_dataset_selection(content: Any)` — [`L279`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L279)
- `render_docker_exec(content: Any, event_title: str = "")` — [`L461`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L461)
- `render_event(event: Event)` — [`L170`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L170) — Render a single event
- `render_evo_loop(evo: EvoLoop, show_types: list[str])` — [`L158`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L158) — Render evolution loop
- `render_experiment(content: Any)` — [`L378`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L378) — Render experiment tasks (Base Model and Datasets shown in page header, not here).
- `render_feedback(content: Any)` — [`L530`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L530)
- `render_generic(content: Any)` — [`L593`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L593)
- `render_hypothesis(content: Any)` — [`L296`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L296) — Render hypothesis content (Base Model shown in page header, not here).
- `render_llm_call(content: Any)` — [`L313`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L313)
- `render_loop(loop: Loop, show_types: list[str])` — [`L58`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L58) — Render a single loop with lazy loading
- `render_scenario(content: Any)` — [`L208`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L208) — Render scenario details (main info shown in page header, this shows extras).
- `render_session(session: Session, show_types: list[str])` — [`L42`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L42) — Render full session with hierarchy
- `render_settings(content: Any)` — [`L306`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L306)
- `render_summary(summary: dict)` — [`L709`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L709)
- `render_template(content: Any)` — [`L354`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L354)
- `render_time_info(content: Any)` — [`L585`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L585)
- `render_token(content: Any)` — [`L572`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L572)
- `render_training_result(result: dict)` — [`L602`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/components.py#L602)

