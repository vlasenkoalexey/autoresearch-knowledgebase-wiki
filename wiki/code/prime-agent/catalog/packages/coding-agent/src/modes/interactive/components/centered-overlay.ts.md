---
title: 'Module: packages/coding-agent/src/modes/interactive/components/centered-overlay.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/centered-overlay.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`centered-overlay.ts`/
symbols:
  showFullPaneOverlay: showFullPaneOverlay().
  CenteredOverlayComponent.render: CenteredOverlayComponent#render().
  CenteredOverlayComponent.-set-focused: CenteredOverlayComponent#`<set>focused`().
  CenteredOverlayComponent.handleInput: CenteredOverlayComponent#handleInput().
  CenteredOverlayComponent.-constructor: CenteredOverlayComponent#`<constructor>`().
  hasInputHandler: hasInputHandler().
  CenteredOverlayComponent: CenteredOverlayComponent#
  CenteredOverlayComponent.place: CenteredOverlayComponent#place().
  CenteredOverlayOptions.getRows: CenteredOverlayOptions#getRows.
  CenteredOverlayComponent.-get-focused: CenteredOverlayComponent#`<get>focused`().
  CenteredOverlayOptions.maxContentWidth: CenteredOverlayOptions#maxContentWidth.
  FullPaneOverlayOptions: FullPaneOverlayOptions#
  CenteredOverlayComponent.invalidate: CenteredOverlayComponent#invalidate().
  CenteredOverlayComponent._focused: CenteredOverlayComponent#_focused.
  CenteredOverlayComponent.blank: CenteredOverlayComponent#blank().
  CenteredOverlayOptions: CenteredOverlayOptions#
  CenteredOverlayOptions.verticalOffset: CenteredOverlayOptions#verticalOffset.
  InputHandler: InputHandler#
  InputHandler.handleInput: InputHandler#handleInput().
  FullPaneOverlayOptions.maxContentWidth: FullPaneOverlayOptions#maxContentWidth.
  FullPaneOverlayOptions.fullWidth: FullPaneOverlayOptions#fullWidth.
  FullPaneOverlayOptions.suspendFullscreenMouse: FullPaneOverlayOptions#suspendFullscreenMouse.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/centered-overlay.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts)

## Classes
### `CenteredOverlayComponent`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/centered-overlay.ts:64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L64)
- signature: `class CenteredOverlayComponent`
- members:
  - `<constructor>(component: Component, options: CenteredOverlayOptions)` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L67)
  - `<get>focused` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L72) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L76) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `blank(method)` — [`L122`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L122)
  - `handleInput(method)` — [`L87`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L87) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L83) — Invalidate any cached rendering state.
  - `place(method)` — [`L114`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L114)
  - `render(method)` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L93) — Render the component to lines for the given viewport width
- protocol/private: `_focused`[`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L65)
- uses (calls/refs, reference-scoped): [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`focused`](../../../../../tui/src/tui.ts.md#Focusable.focused), [`isFocusable`](../../../../../tui/src/tui.ts.md#isFocusable), [`hasInputHandler`](centered-overlay.ts.md#hasInputHandler), [`getRows`](centered-overlay.ts.md#CenteredOverlayOptions.getRows), [`maxContentWidth`](centered-overlay.ts.md#CenteredOverlayOptions.maxContentWidth), [`CenteredOverlayOptions`](centered-overlay.ts.md#CenteredOverlayOptions), [`handleInput`](centered-overlay.ts.md#InputHandler.handleInput), [`verticalOffset`](centered-overlay.ts.md#CenteredOverlayOptions.verticalOffset)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showFullPaneOverlay`](centered-overlay.ts.md#showFullPaneOverlay)  (1 test-only)

### `CenteredOverlayOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/centered-overlay.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L12)
- signature: `interface CenteredOverlayOptions`
- members:
  - `getRows` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L13)
  - `maxContentWidth` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L14)
  - `verticalOffset` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L15)
- used by: [`showFullPaneOverlay`](centered-overlay.ts.md#showFullPaneOverlay), [`render`](centered-overlay.ts.md#CenteredOverlayComponent.render), [`<constructor>`](centered-overlay.ts.md#CenteredOverlayComponent.-constructor)  (1 test-only)

### `FullPaneOverlayOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/centered-overlay.ts:22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L22)
- signature: `interface FullPaneOverlayOptions`
- members:
  - `fullWidth` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L24)
  - `maxContentWidth` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L23)
  - `suspendFullscreenMouse` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L25)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`showFullPaneOverlay`](centered-overlay.ts.md#showFullPaneOverlay), [`showFullPaneOverlay`](../interactive-mode.ts.md#InteractiveMode.showFullPaneOverlay)

### `InputHandler`
- def: [`packages/coding-agent/src/modes/interactive/components/centered-overlay.ts:18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L18)
- signature: `interface InputHandler`
- members:
  - `handleInput(method)` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L19)
- used by: [`handleInput`](centered-overlay.ts.md#CenteredOverlayComponent.handleInput), [`hasInputHandler`](centered-overlay.ts.md#hasInputHandler)

## Functions
- `hasInputHandler(component: Component)` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L28)
- `showFullPaneOverlay(ui: TUI, component: Component, options?: number | FullPaneOverlayOptions)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/centered-overlay.ts#L33) — Shows a component as a full-pane centered overlay on the given TUI.

