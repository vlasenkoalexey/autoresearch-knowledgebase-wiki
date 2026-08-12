---
title: 'Module: run.py'
type: catalog
provenance: extracted
module: run.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 run/
symbols:
  main: main().
  SUPPORTED_SCAFFOLDS: SUPPORTED_SCAFFOLDS.
  CUSTOM_AGENT_CONFIGS: CUSTOM_AGENT_CONFIGS.
  SERVER_MANAGED_SCAFFOLDS: SERVER_MANAGED_SCAFFOLDS.
  start_server: start_server().
  SCAFFOLD_DESCRIPTIONS: SCAFFOLD_DESCRIPTIONS.
  start_frame_server: start_frame_server().
  start_custom_agent: start_custom_agent().
---
# Module: [`run.py`](../../../../raw/code/continual-harness/run.py)

## Functions
- `main()` — [`L291`](../../../../raw/code/continual-harness/run.py#L291) — Main entry point for the Pokemon Agent
- `start_custom_agent(agent_config, args)` — [`L212`](../../../../raw/code/continual-harness/run.py#L212) — Generic helper to start any custom benchmark agent.
- `start_frame_server(port)` — [`L196`](../../../../raw/code/continual-harness/run.py#L196) — Start the lightweight frame server for stream.html visualization
- `start_server(args, run_id=None)` — [`L106`](../../../../raw/code/continual-harness/run.py#L106) — Start the server process with appropriate arguments

## Module values
- `CUSTOM_AGENT_CONFIGS` — [`L16`](../../../../raw/code/continual-harness/run.py#L16)
- `SCAFFOLD_DESCRIPTIONS` — [`L92`](../../../../raw/code/continual-harness/run.py#L92)
- `SERVER_MANAGED_SCAFFOLDS` — [`L103`](../../../../raw/code/continual-harness/run.py#L103)
- `SUPPORTED_SCAFFOLDS` — [`L101`](../../../../raw/code/continual-harness/run.py#L101)

