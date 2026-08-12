---
title: TUI Component/Container — the terminal rendering primitives
type: concept
provenance: mixed
concept: packages-tui-src-tui.ts
updated: 2026-08-12
status: fresh
---
# TUI Component/Container — the terminal rendering primitives

## Overview

[`Component`](../catalog/packages/tui/src/tui.ts.md#Component) — *"Component interface - all components
must implement this"* — and `Container.`[`addChild`](../catalog/packages/tui/src/tui.ts.md#Container.addChild)
are the base terminal-UI primitives `packages/tui` builds on; unrelated to the RLM/Continual-Harness core,
but the rendering substrate [`InteractiveMode`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md)
composes its screens from.

## See also
- [`packages-coding-agent-src-modes-interactive-interactive-mode.ts`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) —
  the consumer.
