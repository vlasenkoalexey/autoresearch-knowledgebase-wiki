---
title: BaseStore — the generic CRUD base every store subclasses
type: concept
provenance: mixed
concept: utils-stores-base_store
updated: 2026-08-12
status: fresh
---
# BaseStore — the generic CRUD base every store subclasses

## Overview

[`BaseStore.add`](../catalog/utils/stores/base_store.md#BaseStore.add) — *"Create a new entry. Returns the
entry ID"* — plus `get`/`get_tree_overview`/`entries` is the generic parent
[`utils-stores-subagents`](utils-stores-subagents.md)'s `SubagentStore` and `Memory` both subclass; see that
page for the design rationale (one CRUD base, three semantically distinct stores).

## See also
- [`utils-stores-subagents`](utils-stores-subagents.md) — the fuller treatment.
- [`utils-stores-memory`](utils-stores-memory.md) — the memory-specific subclass.
