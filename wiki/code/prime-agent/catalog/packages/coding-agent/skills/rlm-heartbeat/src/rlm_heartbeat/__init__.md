---
title: 'Module: packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py'
type: catalog
provenance: extracted
module: packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `packages.coding-agent.skills.rlm-heartbeat.src.rlm_heartbeat`/
symbols:
  update: update().
  create: create().
  _normalize_delivery_mode: _normalize_delivery_mode().
  DeliveryMode: DeliveryMode.
  StatusUpdate: StatusUpdate.
  list: list().
  delete: delete().
---
# Module: [`packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py)

## Functions
- `_normalize_delivery_mode(delivery_mode: DeliveryMode | None)` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L18)
- `create(instruction: str, interval: str | None = None, label: str | None = None, delivery_mode: DeliveryMode | None = None)` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L35) — Create an internal recurring heartbeat for the current agent session.
- `delete(id: str)` — [`L98`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L98) — Cancel one internal RLM heartbeat for the current agent session.
- `list(include_inactive: bool = False)` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L28) — List internal RLM heartbeats for the current agent session.
- `update(id: str, instruction: str | None = None, interval: str | None = None, label: str | None = None, status: StatusUpdate | None = None, delivery_mode: DeliveryMode | None = None)` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L64) — Update one internal RLM heartbeat for the current agent session.

## Module values
- `DeliveryMode` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L15)
- `StatusUpdate` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/rlm-heartbeat/src/rlm_heartbeat/__init__.py#L14)

