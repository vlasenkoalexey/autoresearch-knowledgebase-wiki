---
title: AgentsViewMode — the multi-session dashboard TUI
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-agents-view-agents-view-mode.ts
updated: 2026-08-12
status: fresh
---
# AgentsViewMode — the multi-session dashboard TUI

## Overview

`runAgentsViewMode` starts an `AgentsViewMode` [`Component`](packages-tui-src-tui.ts.md) that renders every
attached-daemon [`SessionSummary`](packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) as a
row — the terminal dashboard for watching several concurrent (including RLM-subagent) sessions at once.
`reconcileCatalogs` recomputes the row list via `buildAgentsViewRows` and calls `requestRender` on the
underlying [`TUI`](packages-tui-src-tui.ts.md) whenever the session set changes; `run` mounts the component
tree with `addChild` and awaits until the view exits.

## See also
- [`packages-coding-agent-src-modes-daemon-daemon-session-list.ts`](packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) —
  the `SessionSummary` rows this view renders.
- [`packages-tui-src-tui.ts`](packages-tui-src-tui.ts.md) — the `Component`/`Container`/`TUI` render loop
  this mode is built on.
