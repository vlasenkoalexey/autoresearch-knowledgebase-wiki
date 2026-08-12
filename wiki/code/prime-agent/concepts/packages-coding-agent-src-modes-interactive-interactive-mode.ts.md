---
title: InteractiveMode — the terminal UI event loop
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-interactive-interactive-mode.ts
updated: 2026-08-12
status: fresh
---
# InteractiveMode — the terminal UI event loop

## Overview

`InteractiveMode` is the interactive-terminal front end —
[`handleEvent`](../catalog/packages/coding-agent/src/modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent)
consumes `AgentConnectionSessionEvent`s from [`packages-coding-agent-src-modes-agent-connection-types.ts`](packages-coding-agent-src-modes-agent-connection-types.ts.md)
and renders them via the [`packages-tui-src-tui.ts`](packages-tui-src-tui.ts.md) component tree; one of
several modes (see [`daemon-mode`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md)) that all sit
on top of the same underlying `AgentSession`.

## See also
- [`packages-coding-agent-src-modes-agent-connection-types.ts`](packages-coding-agent-src-modes-agent-connection-types.ts.md) —
  the event source.
- [`packages-tui-src-tui.ts`](packages-tui-src-tui.ts.md) — the rendering layer.
