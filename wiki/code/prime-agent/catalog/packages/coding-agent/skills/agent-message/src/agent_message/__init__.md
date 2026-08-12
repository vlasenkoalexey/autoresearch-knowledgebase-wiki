---
title: 'Module: packages/coding-agent/skills/agent-message/src/agent_message/__init__.py'
type: catalog
provenance: extracted
module: packages/coding-agent/skills/agent-message/src/agent_message/__init__.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `packages.coding-agent.skills.agent-message.src.agent_message`/
symbols:
  send: send().
  _emit_sent_message: _emit_sent_message().
  ReceiverRole: ReceiverRole.
  _MESSAGE_DISPLAY_MIME: _MESSAGE_DISPLAY_MIME.
  list_agents: list_agents().
---
# Module: [`packages/coding-agent/skills/agent-message/src/agent_message/__init__.py`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py)

## Functions
- `_emit_sent_message(receipt: dict[str, Any], receiver_role: str | None = None)` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py#L70)
- `list_agents()` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py#L18) — List this agent's parent, siblings, and children, including inactive family.
- `send(message: str, broadcast_message: str | None = None, *, receiver_role: ReceiverRole | str | None = None, receiver_name: str | None = None)` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py#L23) — Send one direct role-addressed message or broadcast to ``"all"``.

## Module values
- `ReceiverRole` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py#L14)
- `_MESSAGE_DISPLAY_MIME` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/agent-message/src/agent_message/__init__.py#L15)

