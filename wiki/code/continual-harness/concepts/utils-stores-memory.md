---
title: Memory — the long-term memory store
type: concept
provenance: mixed
concept: utils-stores-memory
updated: 2026-08-12
status: fresh
---
# Memory — the long-term memory store

## Overview

[`Memory`](../catalog/utils/stores/memory.md#Memory) — *"Persistent long-term memory store"* — is the
`BaseStore[MemoryEntry]` subclass [`HarnessEvolver`](agents-utils-harness_evolver.md)'s `_evolve_memory`
pass performs CRUD against, alongside a `search` method that lets the agent retrieve relevant memories
rather than only ever reading everything.

## See also
- [`utils-stores-base_store`](utils-stores-base_store.md) — the generic parent.
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — the CRUD caller.
