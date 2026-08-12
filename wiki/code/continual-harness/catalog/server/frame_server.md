---
title: 'Module: server/frame_server.py'
type: catalog
provenance: extracted
module: server/frame_server.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `server.frame_server`/
symbols:
  get_frame: get_frame().
  load_frame_from_cache: load_frame_from_cache().
  args: args.
  frame_thread: frame_thread.
  get_status: get_status().
  app: app.
  frame_counter: frame_counter.
  frame_updater: frame_updater().
  get_frame_cache_file: get_frame_cache_file().
  parser: parser.
  current_frame: current_frame.
  last_update: last_update.
  health_check: health_check().
  frame_lock: frame_lock.
  FRAME_UPDATE_INTERVAL: FRAME_UPDATE_INTERVAL.
---
# Module: [`server/frame_server.py`](../../../../../raw/code/continual-harness/server/frame_server.py)

## Functions
- `frame_updater()` — [`L76`](../../../../../raw/code/continual-harness/server/frame_server.py#L76) — Background thread to periodically check for new frames
- `get_frame()` — [`L91`](../../../../../raw/code/continual-harness/server/frame_server.py#L91) — Get the current game frame
- `get_frame_cache_file()` — [`L50`](../../../../../raw/code/continual-harness/server/frame_server.py#L50) — Get the frame cache file path based on current run_id
- `get_status()` — [`L134`](../../../../../raw/code/continual-harness/server/frame_server.py#L134) — Get frame server status
- `health_check()` — [`L86`](../../../../../raw/code/continual-harness/server/frame_server.py#L86) — Simple health check endpoint
- `load_frame_from_cache()` — [`L55`](../../../../../raw/code/continual-harness/server/frame_server.py#L55) — Load the latest frame from shared cache file

## Module values
- `FRAME_UPDATE_INTERVAL` — [`L48`](../../../../../raw/code/continual-harness/server/frame_server.py#L48)
- `app` — [`L29`](../../../../../raw/code/continual-harness/server/frame_server.py#L29)
- `args` — [`L149`](../../../../../raw/code/continual-harness/server/frame_server.py#L149)
- `current_frame` — [`L41`](../../../../../raw/code/continual-harness/server/frame_server.py#L41)
- `frame_counter` — [`L43`](../../../../../raw/code/continual-harness/server/frame_server.py#L43)
- `frame_lock` — [`L42`](../../../../../raw/code/continual-harness/server/frame_server.py#L42)
- `frame_thread` — [`L155`](../../../../../raw/code/continual-harness/server/frame_server.py#L155)
- `last_update` — [`L44`](../../../../../raw/code/continual-harness/server/frame_server.py#L44)
- `parser` — [`L146`](../../../../../raw/code/continual-harness/server/frame_server.py#L146)

