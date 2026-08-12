---
title: Editor — the multi-line text-input component
type: concept
provenance: mixed
concept: packages-tui-src-components-editor.ts
updated: 2026-08-12
status: fresh
---
# Editor — the multi-line text-input component

## Overview

`Editor.`[`handleInput`](../catalog/packages/tui/src/components/editor.ts.md#Editor.handleInput) —
*"Optional handler for keyboard input when component has focus"* — is a
[`Component`](packages-tui-src-tui.ts.md) implementation handling keystrokes, undo, word-deletion, and
autocomplete for prompt entry; `state`/`getText`/`setText` expose and mutate its `EditorState` (`lines`,
`cursorLine`, `cursorCol`). This is the concrete text-input widget
[`InteractiveMode`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) and the
`AgentsViewMode` reply box both build on.

## See also
- [`packages-tui-src-tui.ts`](packages-tui-src-tui.ts.md) — the `Component`/`TUI` render framework this
  editor implements.
- [`packages-coding-agent-src-modes-interactive-interactive-mode.ts`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) —
  a consumer for prompt entry.
