---
title: ExtensionAPI — the plugin surface
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-extensions-types.ts
updated: 2026-08-12
status: fresh
---
# ExtensionAPI — the plugin surface

## Overview

[`ExtensionAPI`](../catalog/packages/coding-agent/src/core/extensions/types.ts.md#ExtensionAPI) —
*"ExtensionAPI passed to extension factory functions"* — is an event-subscription interface
([`on`](../catalog/packages/coding-agent/src/core/extensions/types.ts.md#ExtensionAPI.on), covering events
like `resources_discover`, `session_start`, `session_before_switch`) plus a UI context
([`ui`](../catalog/packages/coding-agent/src/core/extensions/types.ts.md#ExtensionContext.ui) —
*"UI methods for user interaction"*, e.g.
[`notify`](../catalog/packages/coding-agent/src/core/extensions/types.ts.md#ExtensionUIContext.notify) —
*"Show a notification to the user"*) — the plugin/extension mechanism third-party code hooks into,
independent of the RLM/Continual-Harness core.

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  the session lifecycle these events fire around.
