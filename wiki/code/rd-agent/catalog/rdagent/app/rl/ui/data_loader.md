---
title: 'Module: rdagent/app/rl/ui/data_loader.py'
type: catalog
provenance: extracted
module: rdagent/app/rl/ui/data_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.rl.ui.data_loader`/
symbols:
  parse_event: parse_event().
  load_session: load_session().
  Event: Event#
  get_summary: get_summary().
  Event.timestamp: Event#timestamp.
  Event.title: Event#title.
  Event.content: Event#content.
  Event.tag: Event#tag.
  Event.loop_id: Event#loop_id.
  Event.stage: Event#stage.
  Session.loops: Session#loops.
  Event.success: Event#success.
  Loop.proposal: Loop#proposal.
  Loop.running: Loop#running.
  Loop.feedback: Loop#feedback.
  Loop.coding: Loop#coding.
  Session.init_events: Session#init_events.
  Session: Session#
  Loop: Loop#
  Event.time_str: Event#time_str().
  Event.duration: Event#duration.
  Loop.loop_id: Loop#loop_id.
  get_valid_sessions: get_valid_sessions().
  extract_loop_id: extract_loop_id().
  extract_stage: extract_stage().
---
# Module: [`rdagent/app/rl/ui/data_loader.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py)

## Classes
### `Event`
- def: [`rdagent/app/rl/ui/data_loader.py:21`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L21)
- doc: Timeline event
- signature: `class Event:`
- members:
  - `time_str(self)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L35)
  - `content` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L28)
  - `duration` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L31)
  - `loop_id` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L29)
  - `stage` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L30)
  - `success` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L32)
  - `tag` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L26)
  - `timestamp` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L25)
  - `title` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L27)
- uses (calls/refs, reference-scoped): [`EventType`](config.md#EventType)
- used by: [`render_event`](components.md#render_event), [`parse_event`](data_loader.md#parse_event), [`render_loop`](components.md#render_loop), [`feedback`](data_loader.md#Loop.feedback), [`proposal`](data_loader.md#Loop.proposal), [`running`](data_loader.md#Loop.running), [`coding`](data_loader.md#Loop.coding), [`init_events`](data_loader.md#Session.init_events)

### `Loop`
- def: [`rdagent/app/rl/ui/data_loader.py:40`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L40)
- doc: Main loop containing stages (no EvoLoop for RL)
- signature: `class Loop:`
- members:
  - `coding` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L45)
  - `feedback` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L47)
  - `loop_id` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L43)
  - `proposal` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L44)
  - `running` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L46)
- uses (calls/refs, reference-scoped): [`Event`](data_loader.md#Event)
- used by: [`load_session`](data_loader.md#load_session), [`render_loop`](components.md#render_loop), [`get_summary`](data_loader.md#get_summary), [`loops`](data_loader.md#Session.loops)

### `Session`
- def: [`rdagent/app/rl/ui/data_loader.py:51`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L51)
- doc: Session containing init events and loops
- signature: `class Session:`
- members:
  - `init_events` — [`L54`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L54)
  - `loops` — [`L55`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L55)
- uses (calls/refs, reference-scoped): [`Event`](data_loader.md#Event), [`Loop`](data_loader.md#Loop)
- used by: [`load_session`](data_loader.md#load_session), [`get_summary`](data_loader.md#get_summary), [`render_session`](components.md#render_session)

## Functions
- `extract_loop_id(tag: str)` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L58)
- `extract_stage(tag: str)` — [`L63`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L63)
- `get_summary(session: Session)` — [`L285`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L285) — Get summary statistics
- `get_valid_sessions(log_folder: Path)` — [`L75`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L75)
- `load_session(log_path: Path)` — [`L237`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L237) — Load events into hierarchical session structure
- `parse_event(tag: str, content: Any, timestamp: datetime)` — [`L85`](../../../../../../../../raw/code/rd-agent/rdagent/app/rl/ui/data_loader.py#L85)

