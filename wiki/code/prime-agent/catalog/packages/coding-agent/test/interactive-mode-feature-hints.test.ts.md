---
title: 'Module: packages/coding-agent/test/interactive-mode-feature-hints.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-mode-feature-hints.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-mode-feature-hints.test.ts`/
symbols:
  createMode: createMode().
  callPrivate: callPrivate().
  FakeLoader: FakeLoader#
  FakeLoader.stop: FakeLoader#stop.
  FakeLoader.invalidate: FakeLoader#invalidate().
  FakeLoader.render: FakeLoader#render().
---
# Module: [`packages/coding-agent/test/interactive-mode-feature-hints.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts)

## Classes
### `FakeLoader`  ·  implements/extends Component
- def: [`packages/coding-agent/test/interactive-mode-feature-hints.test.ts:9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L9)
- signature: `class FakeLoader`
- members:
  - `invalidate(method)` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L12) — Invalidate any cached rendering state.
  - `render(method)` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L14) — Render the component to lines for the given viewport width
  - `stop` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L10)
- uses (calls/refs, reference-scoped): [`Component`](../../tui/src/tui.ts.md#Component)
- used by: [`Component`](../../tui/src/tui.ts.md#Component), [`render`](../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../tui/src/tui.ts.md#Component.invalidate)  (2 test-only)

## Functions
- `callPrivate(mode: object, name: string)` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L19)
- `createMode()` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-feature-hints.test.ts#L23)

