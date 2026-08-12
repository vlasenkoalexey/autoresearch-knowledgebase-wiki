---
title: BaseStore / SubagentStore — the persistent CRUD target
type: concept
provenance: mixed
concept: utils-stores-subagents
updated: 2026-08-12
status: fresh
---
# BaseStore / SubagentStore — the persistent CRUD target

## Overview

[`BaseStore`](../catalog/utils/stores/base_store.md#BaseStore) — *"Persistent JSON store with tree overview
and CRUD"* — is the generic parent [`SubagentStore`](../catalog/utils/stores/subagents.md#SubagentStore),
[`Memory`](../catalog/utils/stores/memory.md#Memory), and
[`SkillStore`](../catalog/utils/stores/skills.md#SkillStore) all subclass; it is the literal implementation
target of [`HarnessEvolver`](agents-utils-harness_evolver.md)'s create/update/retire calls
(`store.add`/`.update`/`.remove`). One `BaseStore[T]` per component type, each persisting a typed entry
dataclass to JSON.

## Design rationale (why it's built this way)

**Built-in entries are seeded once, then evolution only adds on top.** [`SubagentStore._seed_builtins`](../catalog/utils/stores/subagents.md#SubagentStore._seed_builtins) —
*"Populate built-in entries if none exist yet"* — guarantees a baseline subagent set exists before any
evolution has run, so `HarnessEvolver`'s create/update/retire operations are always modifying a store that
already has a sane starting point, never an empty one.

**One generic `BaseStore[T]` backs three semantically different stores.** `Memory`, `SkillStore`, and
`SubagentStore` are all thin subclasses over the same generic CRUD base — [`BaseStore.add`](../catalog/utils/stores/base_store.md#BaseStore.add)'s
own docstring, *"Create a new entry. Returns the entry ID,"* is identical in contract whether the entry is
a memory, a skill, or a subagent. This is what lets `HarnessEvolver`'s three CRUD passes
(`_evolve_subagents`, `_evolve_skills`, `_evolve_memory`) share the same create/update/retire shape against
structurally different content.

## Entry points
- [`get_subagent_store`](../catalog/utils/stores/subagents.md#get_subagent_store) — *"Get or create the
  global SubagentStore instance"* — the accessor `HarnessEvolver._get_subagent_store` calls.
- [`BaseStore.add`](../catalog/utils/stores/base_store.md#BaseStore.add) — the create operation every
  evolved entry (subagent, skill, or memory) is written through.

## Key data structures
- [`SubagentEntry`](../catalog/utils/stores/subagents.md#SubagentEntry) — *"A single entry in the subagent
  registry"* — the persisted shape a `create` recommendation from `HarnessEvolver` becomes.
- `BaseStore.entries: dict[str, T]` — the in-memory index every store subclass shares, keyed by entry ID.

## See also
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — the CRUD caller.
- [`agents-tools-registry`](agents-tools-registry.md) — how a stored subagent's tool becomes callable.
