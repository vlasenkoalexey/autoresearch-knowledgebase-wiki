---
title: 'Module: packages/coding-agent/src/modes/interactive/components/armin.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/armin.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`armin.ts`/
symbols:
  ArminComponent.-constructor: ArminComponent#`<constructor>`().
  ArminComponent.tickEffect: ArminComponent#tickEffect().
  DISPLAY_HEIGHT: DISPLAY_HEIGHT.
  ArminComponent.startAnimation: ArminComponent#startAnimation().
  ArminComponent.render: ArminComponent#render().
  ArminComponent.tickRain: ArminComponent#tickRain().
  ArminComponent.tickCrt: ArminComponent#tickCrt().
  ArminComponent.currentGrid: ArminComponent#currentGrid.
  ArminComponent.effectState: ArminComponent#effectState.
  ArminComponent.initEffect: ArminComponent#initEffect().
  ArminComponent.tickTypewriter: ArminComponent#tickTypewriter().
  ArminComponent.tickScanline: ArminComponent#tickScanline().
  ArminComponent.tickGlitch: ArminComponent#tickGlitch().
  WIDTH: WIDTH.
  ArminComponent.finalGrid: ArminComponent#finalGrid.
  getPixel: getPixel().
  buildFinalGrid: buildFinalGrid().
  ArminComponent.tickFade: ArminComponent#tickFade().
  ArminComponent.tickDissolve: ArminComponent#tickDissolve().
  ArminComponent.createEmptyGrid: ArminComponent#createEmptyGrid().
  ArminComponent.effect: ArminComponent#effect.
  ArminComponent: ArminComponent#
  EFFECTS: EFFECTS.
  ArminComponent.ui: ArminComponent#ui.
  ArminComponent.stopAnimation: ArminComponent#stopAnimation().
  ArminComponent.interval: ArminComponent#interval.
  ArminComponent.cachedLines: ArminComponent#cachedLines.
  BYTES_PER_ROW: BYTES_PER_ROW.
  getChar: getChar().
  ArminComponent.updateDisplay: ArminComponent#updateDisplay().
  ArminComponent.cachedWidth: ArminComponent#cachedWidth.
  ArminComponent.gridVersion: ArminComponent#gridVersion.
  ArminComponent.invalidate: ArminComponent#invalidate().
  ArminComponent.dispose: ArminComponent#dispose().
  HEIGHT: HEIGHT.
  Effect: Effect#
  ArminComponent.cachedVersion: ArminComponent#cachedVersion.
  BITS: BITS.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/armin.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts)

## Classes
### `ArminComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/armin.ts:60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L60)
- signature: `class ArminComponent`
- members:
  - `<constructor>(ui: TUI)` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L72)
  - `createEmptyGrid(method)` — [`L112`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L112)
  - `dispose(method)` — [`L379`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L379)
  - `initEffect(method)` — [`L116`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L116)
  - `invalidate(method)` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L82) — Invalidate any cached rendering state.
  - `render(method)` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L86) — Render the component to lines for the given viewport width
  - `startAnimation(method)` — [`L180`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L180)
  - `stopAnimation(method)` — [`L192`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L192)
  - `tickCrt(method)` — [`L310`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L310)
  - `tickDissolve(method)` — [`L362`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L362)
  - `tickEffect(method)` — [`L199`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L199)
  - `tickFade(method)` — [`L297`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L297)
  - `tickGlitch(method)` — [`L330`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L330)
  - `tickRain(method)` — [`L246`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L246)
  - `tickScanline(method)` — [`L234`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L234)
  - `tickTypewriter(method)` — [`L220`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L220)
  - `updateDisplay(method)` — [`L375`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L375)
  - `cachedLines` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L67)
  - `cachedVersion` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L70)
  - `cachedWidth` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L68)
  - `currentGrid` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L65)
  - `effect` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L63)
  - `effectState` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L66)
  - `finalGrid` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L64)
  - `gridVersion` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L69)
  - `interval` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L62)
  - `ui` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L61)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`DISPLAY_HEIGHT`](armin.ts.md#DISPLAY_HEIGHT), [`WIDTH`](armin.ts.md#WIDTH), [`buildFinalGrid`](armin.ts.md#buildFinalGrid), [`EFFECTS`](armin.ts.md#EFFECTS), [`Effect`](armin.ts.md#Effect)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleArminSaysHi`](../interactive-mode.ts.md#InteractiveMode.handleArminSaysHi)

### `Effect`
- def: [`packages/coding-agent/src/modes/interactive/components/armin.ts:25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L25)
- signature: `type Effect`
- used by: [`effect`](armin.ts.md#ArminComponent.effect), [`EFFECTS`](armin.ts.md#EFFECTS)

## Functions
- `buildFinalGrid()` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L48)
- `getChar(x: number, row: number)` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L38)
- `getPixel(x: number, y: number)` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L30)

## Module values
- `BITS` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L11)
- `BYTES_PER_ROW` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L22)
- `DISPLAY_HEIGHT` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L23)
- `EFFECTS` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L27)
- `HEIGHT` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L10)
- `WIDTH` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/armin.ts#L9)

