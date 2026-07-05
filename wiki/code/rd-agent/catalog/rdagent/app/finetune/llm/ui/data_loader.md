---
title: 'Module: rdagent/app/finetune/llm/ui/data_loader.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/llm/ui/data_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.llm.ui.data_loader`/
symbols:
  load_ft_session: load_ft_session().
  parse_event: parse_event().
  Event.content: Event#content.
  Event: Event#
  get_summary: get_summary().
  Event.title: Event#title.
  Event.timestamp: Event#timestamp.
  Event.tag: Event#tag.
  Event.loop_id: Event#loop_id.
  Event.stage: Event#stage.
  Loop.coding: Loop#coding.
  Event.success: Event#success.
  Session.loops: Session#loops.
  Session.init_events: Session#init_events.
  EvoLoop.success: EvoLoop#success.
  Loop.exp_gen: Loop#exp_gen.
  Loop.runner: Loop#runner.
  Loop.feedback: Loop#feedback.
  Event.evo_id: Event#evo_id.
  EvoLoop.events: EvoLoop#events.
  EvoLoop: EvoLoop#
  Loop: Loop#
  Session: Session#
  Loop.loop_id: Loop#loop_id.
  Event.time_str: Event#time_str().
  Event.duration: Event#duration.
  EvoLoop.evo_id: EvoLoop#evo_id.
  get_valid_sessions: get_valid_sessions().
  extract_loop_id: extract_loop_id().
  extract_evo_id: extract_evo_id().
  extract_stage: extract_stage().
---
# Module: [`rdagent/app/finetune/llm/ui/data_loader.py`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py)

## Classes
### `Event`
- def: [`rdagent/app/finetune/llm/ui/data_loader.py:19`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L19)
- doc: Timeline event
- signature: `class Event:`
- members:
  - `time_str(self)` — [`L34`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L34)
  - `content` — [`L26`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L26)
  - `duration` — [`L30`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L30)
  - `evo_id` — [`L28`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L28)
  - `loop_id` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L27)
  - `stage` — [`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L29)
  - `success` — [`L31`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L31)
  - `tag` — [`L24`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L24)
  - `timestamp` — [`L23`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L23)
  - `title` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L25)
- uses (calls/refs, reference-scoped): [`EventType`](config.md#EventType)
- used by: [`render_event`](components.md#render_event), [`parse_event`](data_loader.md#parse_event), [`main`](app.md#main), [`render_loop`](components.md#render_loop), [`init_events`](data_loader.md#Session.init_events), [`exp_gen`](data_loader.md#Loop.exp_gen), [`feedback`](data_loader.md#Loop.feedback), [`runner`](data_loader.md#Loop.runner), [`events`](data_loader.md#EvoLoop.events)

### `EvoLoop`
- def: [`rdagent/app/finetune/llm/ui/data_loader.py:39`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L39)
- doc: Evolution loop containing events
- signature: `class EvoLoop:`
- members:
  - `events` — [`L43`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L43)
  - `evo_id` — [`L42`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L42)
  - `success` — [`L44`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L44)
- uses (calls/refs, reference-scoped): [`Event`](data_loader.md#Event)
- used by: [`load_ft_session`](data_loader.md#load_ft_session), [`render_loop`](components.md#render_loop), [`get_summary`](data_loader.md#get_summary), [`coding`](data_loader.md#Loop.coding), [`render_evo_loop`](components.md#render_evo_loop)

### `Loop`
- def: [`rdagent/app/finetune/llm/ui/data_loader.py:48`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L48)
- doc: Main loop containing stages
- signature: `class Loop:`
- members:
  - `coding` — [`L53`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L53)
  - `exp_gen` — [`L52`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L52)
  - `feedback` — [`L55`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L55)
  - `loop_id` — [`L51`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L51)
  - `runner` — [`L54`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L54)
- uses (calls/refs, reference-scoped): [`Event`](data_loader.md#Event), [`EvoLoop`](data_loader.md#EvoLoop)
- used by: [`load_ft_session`](data_loader.md#load_ft_session), [`render_loop`](components.md#render_loop), [`get_summary`](data_loader.md#get_summary), [`_render_loop_content`](components.md#_render_loop_content), [`loops`](data_loader.md#Session.loops)

### `Session`
- def: [`rdagent/app/finetune/llm/ui/data_loader.py:59`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L59)
- doc: Session containing init events and loops
- signature: `class Session:`
- members:
  - `init_events` — [`L62`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L62)
  - `loops` — [`L63`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L63)
- uses (calls/refs, reference-scoped): [`Event`](data_loader.md#Event), [`Loop`](data_loader.md#Loop)
- used by: [`load_ft_session`](data_loader.md#load_ft_session), [`main`](app.md#main), [`get_summary`](data_loader.md#get_summary), [`render_session`](components.md#render_session)

## Functions
- `extract_evo_id(tag: str)` — [`L71`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L71)
- `extract_loop_id(tag: str)` — [`L66`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L66)
- `extract_stage(tag: str)` — [`L76`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L76)
- `get_summary(session: Session)` — [`L423`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L423) — Get summary statistics
- `get_valid_sessions(log_folder: Path)` — [`L88`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L88)
- `load_ft_session(log_path: Path)` — [`L365`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L365) — Load events into hierarchical session structure — documented in [rdagent-log-base](../../../../../../concepts/rdagent-log-base.md)
- `parse_event(tag: str, content: Any, timestamp: datetime)` — [`L98`](../../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/llm/ui/data_loader.py#L98)

