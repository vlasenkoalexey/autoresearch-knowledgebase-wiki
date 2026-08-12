---
title: 'Module: packages/coding-agent/skills/websearch/src/websearch/websearch.py'
type: catalog
provenance: extracted
module: packages/coding-agent/skills/websearch/src/websearch/websearch.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `packages.coding-agent.skills.websearch.src.websearch.websearch`/
symbols:
  _fetch_serper: _fetch_serper().
  run: run().
  _resolve_api_key: _resolve_api_key().
  _env_int: _env_int().
  _agent_dir: _agent_dir().
  _resolve_config_value: _resolve_config_value().
  _format_serper_results: _format_serper_results().
---
# Module: [`packages/coding-agent/skills/websearch/src/websearch/websearch.py`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py)

## Functions
- `_agent_dir()` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L20) — Resolve the Prime Agent config dir the same way the runtime does.
- `_env_int(name: str, default: int)` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L12) — Read an int from the environment, falling back to default on bad values.
- `_fetch_serper(query: str, api_key: str, timeout: int = 45, num_results: int = 5)` — [`L109`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L109) — Execute a single Serper API search.
- `_format_serper_results(data: dict, query: str, num_results: int = 5)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L56) — Format a Serper API response into readable text.
- `_resolve_api_key()` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L30)
- `_resolve_config_value(value: str)` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L47)
- `run(query: str, *, max_output: int = 8192, timeout: int | None = None, num_results: int | None = None)` — [`L130`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/websearch/src/websearch/websearch.py#L130) — Run a Google search via Serper and return formatted results.

