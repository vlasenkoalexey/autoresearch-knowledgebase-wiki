---
title: AuthStorage — credential persistence
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-auth-storage.ts
updated: 2026-08-12
status: fresh
---
# AuthStorage — credential persistence

## Overview

[`AuthStorage`](../catalog/packages/coding-agent/src/core/auth-storage.ts.md#AuthStorage) —
*"Credential storage backed by a JSON file"* — with `.`[`create`](../catalog/packages/coding-agent/src/core/auth-storage.ts.md#AuthStorage.create)
(file-backed, under the agent dir) and `.`[`inMemory`](../catalog/packages/coding-agent/src/core/auth-storage.ts.md#AuthStorage.inMemory)
(test/ephemeral) constructors, holds API-key and OAuth credentials
(`ApiKeyCredential.`[`type`](../catalog/packages/coding-agent/src/core/auth-storage.ts.md#ApiKeyCredential.typeLiteral1.type) `=
"api_key"`) keyed by provider. `createAgentSession` and `main` both construct one at startup — the
provider-credential layer underneath model selection, orthogonal to the RLM/Continual-Harness mechanisms.

## See also
- [`packages-coding-agent-src-core-settings-manager.ts`](packages-coding-agent-src-core-settings-manager.ts.md) —
  the sibling general-settings store, loaded alongside auth at startup.
