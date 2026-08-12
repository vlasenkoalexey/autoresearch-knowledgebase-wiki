---
slug: prime-agent
commit: a3b3e753490d0a6ed180e905200c1a6690d78608
scip_tool: scip-python
updated: 2026-08-12
---

# prime-agent internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| packages-agent-src-types.ts | [packages-agent-src-types.ts](concepts/packages-agent-src-types.ts.md) | fresh |
| packages-ai-src-types.ts | [packages-ai-src-types.ts](concepts/packages-ai-src-types.ts.md) | fresh |
| packages-coding-agent-src-core-agent-messages.ts | [packages-coding-agent-src-core-agent-messages.ts](concepts/packages-coding-agent-src-core-agent-messages.ts.md) | fresh |
| packages-coding-agent-src-core-agent-session.ts | [packages-coding-agent-src-core-agent-session.ts](concepts/packages-coding-agent-src-core-agent-session.ts.md) | fresh |
| packages-coding-agent-src-core-auth-storage.ts | [packages-coding-agent-src-core-auth-storage.ts](concepts/packages-coding-agent-src-core-auth-storage.ts.md) | fresh |
| packages-coding-agent-src-core-cron-jobs.ts | [packages-coding-agent-src-core-cron-jobs.ts](concepts/packages-coding-agent-src-core-cron-jobs.ts.md) | fresh |
| packages-coding-agent-src-core-extensions-types.ts | [packages-coding-agent-src-core-extensions-types.ts](concepts/packages-coding-agent-src-core-extensions-types.ts.md) | fresh |
| packages-coding-agent-src-core-kernel-index.ts | [packages-coding-agent-src-core-kernel-index.ts](concepts/packages-coding-agent-src-core-kernel-index.ts.md) | fresh |
| packages-coding-agent-src-core-messages.ts | [packages-coding-agent-src-core-messages.ts](concepts/packages-coding-agent-src-core-messages.ts.md) | fresh |
| packages-coding-agent-src-core-package-manager.ts | [packages-coding-agent-src-core-package-manager.ts](concepts/packages-coding-agent-src-core-package-manager.ts.md) | fresh |
| packages-coding-agent-src-core-refinement-refinement.ts | [packages-coding-agent-src-core-refinement-refinement.ts](concepts/packages-coding-agent-src-core-refinement-refinement.ts.md) | fresh |
| packages-coding-agent-src-core-session-action-store.ts | [packages-coding-agent-src-core-session-action-store.ts](concepts/packages-coding-agent-src-core-session-action-store.ts.md) | fresh |
| packages-coding-agent-src-core-session-manager.ts | [packages-coding-agent-src-core-session-manager.ts](concepts/packages-coding-agent-src-core-session-manager.ts.md) | fresh |
| packages-coding-agent-src-core-settings-manager.ts | [packages-coding-agent-src-core-settings-manager.ts](concepts/packages-coding-agent-src-core-settings-manager.ts.md) | fresh |
| packages-coding-agent-src-modes-agent-connection-types.ts | [packages-coding-agent-src-modes-agent-connection-types.ts](concepts/packages-coding-agent-src-modes-agent-connection-types.ts.md) | fresh |
| packages-coding-agent-src-modes-agents-view-agents-view-mode.ts | [packages-coding-agent-src-modes-agents-view-agents-view-mode.ts](concepts/packages-coding-agent-src-modes-agents-view-agents-view-mode.ts.md) | fresh |
| packages-coding-agent-src-modes-daemon-active-session-state.ts | [packages-coding-agent-src-modes-daemon-active-session-state.ts](concepts/packages-coding-agent-src-modes-daemon-active-session-state.ts.md) | fresh |
| packages-coding-agent-src-modes-daemon-daemon-mode.ts | [packages-coding-agent-src-modes-daemon-daemon-mode.ts](concepts/packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) | fresh |
| packages-coding-agent-src-modes-daemon-daemon-protocol.ts | [packages-coding-agent-src-modes-daemon-daemon-protocol.ts](concepts/packages-coding-agent-src-modes-daemon-daemon-protocol.ts.md) | fresh |
| packages-coding-agent-src-modes-daemon-daemon-session-list.ts | [packages-coding-agent-src-modes-daemon-daemon-session-list.ts](concepts/packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) | fresh |
| packages-coding-agent-src-modes-daemon-daemon-supervisor.ts | [packages-coding-agent-src-modes-daemon-daemon-supervisor.ts](concepts/packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md) | fresh |
| packages-coding-agent-src-modes-interactive-interactive-mode.ts | [packages-coding-agent-src-modes-interactive-interactive-mode.ts](concepts/packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) | fresh |
| packages-coding-agent-src-modes-interactive-theme-theme.ts | [packages-coding-agent-src-modes-interactive-theme-theme.ts](concepts/packages-coding-agent-src-modes-interactive-theme-theme.ts.md) | fresh |
| packages-tui-src-components-editor.ts | [packages-tui-src-components-editor.ts](concepts/packages-tui-src-components-editor.ts.md) | fresh |
| packages-tui-src-tui.ts | [packages-tui-src-tui.ts](concepts/packages-tui-src-tui.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [long-running-agent-continuity](doc-concepts/long-running-agent-continuity.md)
- [prime-agent-trust-model](doc-concepts/prime-agent-trust-model.md)
- [rlm-continual-harness-composition](doc-concepts/rlm-continual-harness-composition.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **20157** across 774 modules
- deep (concept pages): **68** (0.3%)
- catalog-only: **20089**
- represented total: **20157** (100.0%)
- classes represented: **1984/1984**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
