---
title: 'Module: run_cli.py'
type: catalog
provenance: extracted
module: run_cli.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 run_cli/
symbols:
  _run_agent_loop: _run_agent_loop().
  main: main().
  logger: logger.
  _start_services: _start_services().
  _cleanup_services: _cleanup_services().
  launch_cli_agent: launch_cli_agent().
  _load_last_session_id: _load_last_session_id().
  preflight_cli: preflight_cli().
  _cleanup_cli_session: _cleanup_cli_session().
  _write_last_session_id: _write_last_session_id().
  Services.server: Services#server.
  termination_monitor: termination_monitor().
  _restore_from_backup: _restore_from_backup().
  Services.frame_server: Services#frame_server.
  Services.mcp_process: Services#mcp_process.
  Services: Services#
  start_server: start_server().
  check_termination_condition: check_termination_condition().
  _terminate_process: _terminate_process().
  Services.server_url: Services#server_url.
  LAST_CLI_SESSION_ID_FILENAME: LAST_CLI_SESSION_ID_FILENAME.
  _preflight_claude: _preflight_claude().
  _preflight_gemini: _preflight_gemini().
  _preflight_codex: _preflight_codex().
  _preflight_hermes: _preflight_hermes().
  _build_container_image: _build_container_image().
  start_frame_server: start_frame_server().
  start_mcp_sse_server: start_mcp_sse_server().
  main._sigterm_handler: main()._sigterm_handler().
---
# Module: [`run_cli.py`](../../../../raw/code/continual-harness/run_cli.py)

## Classes
### `Services`
- def: [`run_cli.py:503`](../../../../raw/code/continual-harness/run_cli.py#L503)
- doc: Running services (server, frame server, MCP) and URLs.
- signature: `class Services:`
- members:
  - `frame_server` — [`L506`](../../../../raw/code/continual-harness/run_cli.py#L506)
  - `mcp_process` — [`L507`](../../../../raw/code/continual-harness/run_cli.py#L507)
  - `server` — [`L505`](../../../../raw/code/continual-harness/run_cli.py#L505)
  - `server_url` — [`L508`](../../../../raw/code/continual-harness/run_cli.py#L508)
- used by: [`_run_agent_loop`](run_cli.md#_run_agent_loop), [`_start_services`](run_cli.md#_start_services), [`_cleanup_services`](run_cli.md#_cleanup_services)

## Functions
- `_build_container_image(backend)` — [`L256`](../../../../raw/code/continual-harness/run_cli.py#L256) — Build the container image for the given backend. Returns True on success.
- `_cleanup_cli_session(session: CliSession | None, log_file=None)` — [`L81`](../../../../raw/code/continual-harness/run_cli.py#L81) — Clean up resources from a single CLI agent session.
- `_cleanup_services(services: Services | None, cli_session: CliSession | None, cli_log_file, args, graceful_timeout: int = 30)` — [`L589`](../../../../raw/code/continual-harness/run_cli.py#L589) — Clean up server, frame server, MCP server, and CLI agent.
- `_load_last_session_id(backend: CliAgentBackend, agent_memory_dir: Path)` — [`L514`](../../../../raw/code/continual-harness/run_cli.py#L514) — Load persisted CLI session ID from cache (for --resume across runs/restores).
- `_preflight_claude()` — [`L115`](../../../../raw/code/continual-harness/run_cli.py#L115) — Preflight checks for Claude Code CLI.
- `_preflight_codex()` — [`L182`](../../../../raw/code/continual-harness/run_cli.py#L182) — Preflight checks for Codex CLI.
- `_preflight_gemini()` — [`L149`](../../../../raw/code/continual-harness/run_cli.py#L149) — Preflight checks for Gemini CLI.
- `_preflight_hermes()` — [`L225`](../../../../raw/code/continual-harness/run_cli.py#L225) — Preflight checks for Hermes CLI.
- `_restore_from_backup(backup_path: str)` — [`L541`](../../../../raw/code/continual-harness/run_cli.py#L541) — Restore cache from backup zip. Returns True if successful.
- `_run_agent_loop(services: Services, args, run_manager, agent_memory_dir: Path, backend: CliAgentBackend)` — [`L705`](../../../../raw/code/continual-harness/run_cli.py#L705) — Run the agent loop until termination. Returns (termination_reason, last_cli_session, cli_log_file).
- `_sigterm_handler(signum, frame)` — [`L1002`](../../../../raw/code/continual-harness/run_cli.py#L1002) — So timeout(1) or kill sends SIGTERM → same cleanup as Ctrl+C (stop container).
- `_start_services(args, run_manager)` — [`L558`](../../../../raw/code/continual-harness/run_cli.py#L558) — Start server, frame server, and optionally MCP SSE server. Returns Services or None if server failed.
- `_terminate_process(process: subprocess.Popen, graceful_timeout: int, label: str, use_process_group: bool = False)` — [`L49`](../../../../raw/code/continual-harness/run_cli.py#L49) — Terminate process gracefully, then force kill if needed.
- `_write_last_session_id(session_id: str)` — [`L530`](../../../../raw/code/continual-harness/run_cli.py#L530) — Persist CLI session ID to cache (included in backups for restore).
- `check_termination_condition(server_url: str, condition_type: str = "gym_badge_count", threshold: int = 1)` — [`L458`](../../../../raw/code/continual-harness/run_cli.py#L458) — Check if termination condition is met by polling the server.
- `launch_cli_agent(backend, server_url: str, directive_path: str, working_dir: str, *, project_root: str | None = None, dangerously_skip_permissions: bool = True, log_file=None, metrics: CliSessionMetrics | None = None, containerized: bool = False, session_number: int = 1, resume_session_id: str | None = None, thinking_effort: str | None = None, mcp_sse_port: int | None = None, run_id: str | None = None, agent_memory_dir: str | None = None)` — [`L635`](../../../../raw/code/continual-harness/run_cli.py#L635) — Launch an external CLI agent session as subprocess using the given backend.
- `main()` — [`L897`](../../../../raw/code/continual-harness/run_cli.py#L897) — Main entry point for CLI agent experiments.
- `preflight_cli(args)` — [`L98`](../../../../raw/code/continual-harness/run_cli.py#L98) — Validate CLI availability and show actionable setup errors.
- `start_frame_server(port)` — [`L376`](../../../../raw/code/continual-harness/run_cli.py#L376) — Start the lightweight frame server for stream.html visualization.
- `start_mcp_sse_server(server_url: str, mcp_port: int, project_root: str | None = None, log_path: Path | None = None)` — [`L392`](../../../../raw/code/continual-harness/run_cli.py#L392) — Start the MCP SSE server used by containerized agents.
- `start_server(args, run_id=None)` — [`L294`](../../../../raw/code/continual-harness/run_cli.py#L294) — Start the server process with appropriate arguments.
- `termination_monitor(server_url: str, termination_triggered: threading.Event, condition_type: str = "gym_badge_count", threshold: int = 1, poll_interval: int = 10)` — [`L482`](../../../../raw/code/continual-harness/run_cli.py#L482) — Poll server for termination condition. Sets event when met.

## Module values
- `LAST_CLI_SESSION_ID_FILENAME` — [`L511`](../../../../raw/code/continual-harness/run_cli.py#L511)
- `logger` — [`L46`](../../../../raw/code/continual-harness/run_cli.py#L46)

