---
title: 'Module: packages/coding-agent/src/modes/interactive/components/daxnuts.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/daxnuts.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`daxnuts.ts`/
symbols:
  DaxnutsComponent.render: DaxnutsComponent#render().
  DaxnutsComponent.startAnimation: DaxnutsComponent#startAnimation().
  buildImage: buildImage().
  DaxnutsComponent.-constructor: DaxnutsComponent#`<constructor>`().
  parseImage: parseImage().
  DaxnutsComponent.tick: DaxnutsComponent#tick.
  WIDTH: WIDTH.
  DaxnutsComponent.image: DaxnutsComponent#image.
  DaxnutsComponent.maxTicks: DaxnutsComponent#maxTicks.
  DaxnutsComponent: DaxnutsComponent#
  DaxnutsComponent.ui: DaxnutsComponent#ui.
  DaxnutsComponent.stopAnimation: DaxnutsComponent#stopAnimation().
  DaxnutsComponent.interval: DaxnutsComponent#interval.
  DaxnutsComponent.cachedWidth: DaxnutsComponent#cachedWidth.
  DAX_HEX: DAX_HEX.
  rgb: rgb().
  DaxnutsComponent.invalidate: DaxnutsComponent#invalidate().
  DaxnutsComponent.dispose: DaxnutsComponent#dispose().
  HEIGHT: HEIGHT.
  RESET: RESET.
  DaxnutsComponent.cachedLines: DaxnutsComponent#cachedLines.
  DaxnutsComponent.cachedTick: DaxnutsComponent#cachedTick.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/daxnuts.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts)

## Classes
### `DaxnutsComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/daxnuts.ts:57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L57)
- signature: `class DaxnutsComponent`
- members:
  - `<constructor>(ui: TUI)` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L67)
  - `dispose(method)` — [`L161`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L161)
  - `invalidate(method)` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L73) — Invalidate any cached rendering state.
  - `render(method)` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L95) — Render the component to lines for the given viewport width
  - `startAnimation(method)` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L77)
  - `stopAnimation(method)` — [`L88`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L88)
  - `cachedLines` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L63)
  - `cachedTick` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L65)
  - `cachedWidth` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L64)
  - `image` — [`L59`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L59)
  - `interval` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L60)
  - `maxTicks` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L62)
  - `tick` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L61)
  - `ui` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L58)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`buildImage`](daxnuts.ts.md#buildImage), [`WIDTH`](daxnuts.ts.md#WIDTH), [`rgb`](daxnuts.ts.md#rgb), [`RESET`](daxnuts.ts.md#RESET)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleDaxnuts`](../interactive-mode.ts.md#InteractiveMode.handleDaxnuts)

## Functions
- `buildImage()` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L39)
- `parseImage()` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L17)
- `rgb(r: number, g: number, b: number, bg?: boolean)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L33)

## Module values
- `DAX_HEX` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L11)
- `HEIGHT` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L15)
- `RESET` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L37)
- `WIDTH` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/daxnuts.ts#L14)

