---
title: 'Module: packages/coding-agent/test/centered-overlay.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/centered-overlay.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`centered-overlay.test.ts`/TestComponent#
symbols:
  TestComponent: ''
  TestComponent.handleInput: handleInput().
  TestComponent.inputs: inputs.
  TestComponent.focused: focused.
  TestComponent.invalidate: invalidate().
  TestComponent.render: render().
---
# Module: [`packages/coding-agent/test/centered-overlay.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts)

## Classes
### `TestComponent`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/test/centered-overlay.test.ts:5`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L5)
- signature: `class TestComponent`
- members:
  - `handleInput(method)` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L17) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L9) — Invalidate any cached rendering state.
  - `render(method)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L13) — Render the component to lines for the given viewport width
  - `focused` — [`L6`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L6) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `inputs` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/centered-overlay.test.ts#L7)
- uses (calls/refs, reference-scoped): [`Component`](../../tui/src/tui.ts.md#Component), [`Focusable`](../../tui/src/tui.ts.md#Focusable)
- used by: [`Component`](../../tui/src/tui.ts.md#Component), [`render`](../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../tui/src/tui.ts.md#Focusable), [`focused`](../../tui/src/tui.ts.md#Focusable.focused)  (1 test-only)

