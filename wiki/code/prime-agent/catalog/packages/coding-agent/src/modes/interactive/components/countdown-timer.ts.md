---
title: 'Module: packages/coding-agent/src/modes/interactive/components/countdown-timer.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/countdown-timer.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`countdown-timer.ts`/CountdownTimer#
symbols:
  CountdownTimer.-constructor: '`<constructor>`().'
  CountdownTimer.dispose: dispose().
  CountdownTimer: ''
  CountdownTimer.remainingSeconds: remainingSeconds.
  CountdownTimer.intervalId: intervalId.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/countdown-timer.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts)

## Classes
### `CountdownTimer`
- def: [`packages/coding-agent/src/modes/interactive/components/countdown-timer.ts:7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts#L7)
- signature: `class CountdownTimer`
- members:
  - `<constructor>(timeoutMs: number, tui: TUI | undefined, onTick: (seconds: number) => void, onExpire: () => void)` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts#L11)
  - `dispose(method)` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts#L32)
  - `intervalId` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts#L8)
  - `remainingSeconds` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/countdown-timer.ts#L9)
- uses (calls/refs, reference-scoped): [`requestRender`](../../../../../tui/src/tui.ts.md#TUI.requestRender), [`TUI`](../../../../../tui/src/tui.ts.md#TUI)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`<constructor>`](extension-selector.ts.md#ExtensionSelectorComponent.-constructor), [`extension-selector.ts`](extension-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-extension-selector.ts), [`<constructor>`](extension-input.ts.md#ExtensionInputComponent.-constructor), [`extension-input.ts`](extension-input.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-extension-input.ts), [`retryCountdown`](../interactive-mode.ts.md#InteractiveMode.retryCountdown), [`dispose`](extension-input.ts.md#ExtensionInputComponent.dispose), [`dispose`](extension-selector.ts.md#ExtensionSelectorComponent.dispose), [`countdown`](extension-input.ts.md#ExtensionInputComponent.countdown), [`countdown`](extension-selector.ts.md#ExtensionSelectorComponent.countdown)

