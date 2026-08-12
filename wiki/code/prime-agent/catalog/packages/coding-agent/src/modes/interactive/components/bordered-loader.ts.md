---
title: 'Module: packages/coding-agent/src/modes/interactive/components/bordered-loader.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/bordered-loader.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`bordered-loader.ts`/BorderedLoader#
symbols:
  BorderedLoader.-constructor: '`<constructor>`().'
  BorderedLoader.loader: loader.
  BorderedLoader.-get-signal: '`<get>signal`().'
  BorderedLoader.-set-onAbort: '`<set>onAbort`().'
  BorderedLoader.handleInput: handleInput().
  BorderedLoader.dispose: dispose().
  BorderedLoader: ''
  BorderedLoader.cancellable: cancellable.
  BorderedLoader.signalController: signalController.
  BorderedLoader.-constructor-.options-typeLiteral0.cancellable: '`<constructor>`().(options)typeLiteral0:cancellable.'
---
# Module: [`packages/coding-agent/src/modes/interactive/components/bordered-loader.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts)

## Classes
### `BorderedLoader`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/bordered-loader.ts:7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L7)
- doc: Loader wrapped with borders for extension UI
- signature: `class BorderedLoader`
- members:
  - `<constructor>(tui: TUI, theme: Theme, message: string, options?: { cancellable?: boolean | undefined; } | undefined)` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L12) — Loader wrapped with borders for extension UI
  - `<get>signal` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L42)
  - `<set>onAbort(() => void)` — [`L49`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L49)
  - `dispose(method)` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L61)
  - `handleInput(method)` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L55)
  - `cancellable` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L9)
  - `cancellable` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L12)
  - `loader` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L8)
  - `signalController` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/bordered-loader.ts#L10)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Theme`](../theme/theme.ts.md#Theme), [`keyHint`](keybinding-hints.ts.md#keyHint), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`Loader`](../../../../../tui/src/components/loader.ts.md#Loader), [`<constructor>`](../../../../../tui/src/components/loader.ts.md#Loader.-constructor), [`stop`](../../../../../tui/src/components/loader.ts.md#Loader.stop), [`handleInput`](../../../../../tui/src/components/cancellable-loader.ts.md#CancellableLoader.handleInput), [`CancellableLoader`](../../../../../tui/src/components/cancellable-loader.ts.md#CancellableLoader), [`dispose`](../../../../../tui/src/components/cancellable-loader.ts.md#CancellableLoader.dispose), [`<get>signal`](../../../../../tui/src/components/cancellable-loader.ts.md#CancellableLoader.-get-signal), [`onAbort`](../../../../../tui/src/components/cancellable-loader.ts.md#CancellableLoader.onAbort)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`handleShareCommand`](../interactive-mode.ts.md#InteractiveMode.handleShareCommand)  (2 test-only)

