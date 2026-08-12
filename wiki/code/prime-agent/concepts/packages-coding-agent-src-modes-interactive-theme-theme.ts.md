---
title: Theme — terminal color/style resolution
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-interactive-theme-theme.ts
updated: 2026-08-12
status: fresh
---
# Theme — terminal color/style resolution

## Overview

A global `theme: `[`Theme`](../catalog/packages/coding-agent/src/modes/interactive/theme/theme.ts.md#theme)
instance and its [`fg`](../catalog/packages/coding-agent/src/modes/interactive/theme/theme.ts.md#Theme.fg)
method resolve semantic colors to terminal escape sequences for
[`InteractiveMode`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md)'s rendering —
presentation-layer only.

## See also
- [`packages-coding-agent-src-modes-interactive-interactive-mode.ts`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) —
  the consumer.
