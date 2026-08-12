---
title: 'Module: packages/coding-agent/test/edit-tool-no-full-redraw.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/edit-tool-no-full-redraw.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`edit-tool-no-full-redraw.test.ts`/
symbols:
  waitForRender: waitForRender().
  FakeTerminal: FakeTerminal#
  FakeTerminal.-get-fullClearCount: FakeTerminal#`<get>fullClearCount`().
  waitForRenderedText: waitForRenderedText().
  createLargeEdits: createLargeEdits().
  FakeTerminal.write: FakeTerminal#write().
  FakeTerminal.enterAltScreen: FakeTerminal#enterAltScreen().
  FakeTerminal.leaveAltScreen: FakeTerminal#leaveAltScreen().
  FakeTerminal.setMouseTracking: FakeTerminal#setMouseTracking().
  FakeTerminal.writes: FakeTerminal#writes.
  FakeTerminal.altScreenActive: FakeTerminal#altScreenActive.
  FakeTerminal.mouseTrackingActive: FakeTerminal#mouseTrackingActive.
  FakeTerminal.columns: FakeTerminal#columns.
  FakeTerminal.rows: FakeTerminal#rows.
  FakeTerminal.kittyProtocolActive: FakeTerminal#kittyProtocolActive.
  FakeTerminal.start: FakeTerminal#start().
  FakeTerminal.stop: FakeTerminal#stop().
  FakeTerminal.drainInput: FakeTerminal#drainInput().
  FakeTerminal.moveBy: FakeTerminal#moveBy().
  FakeTerminal.hideCursor: FakeTerminal#hideCursor().
  FakeTerminal.showCursor: FakeTerminal#showCursor().
  FakeTerminal.clearLine: FakeTerminal#clearLine().
  FakeTerminal.clearFromCursor: FakeTerminal#clearFromCursor().
  FakeTerminal.clearScreen: FakeTerminal#clearScreen().
  FakeTerminal.setTitle: FakeTerminal#setTitle().
  FakeTerminal.setProgress: FakeTerminal#setProgress().
---
# Module: [`packages/coding-agent/test/edit-tool-no-full-redraw.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts)

## Classes
### `FakeTerminal`  ·  implements/extends Terminal
- def: [`packages/coding-agent/test/edit-tool-no-full-redraw.test.ts:12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L12)
- signature: `class FakeTerminal`
- members:
  - `<get>fullClearCount` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L44)
  - `clearFromCursor(method)` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L28)
  - `clearLine(method)` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L27)
  - `clearScreen(method)` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L29)
  - `drainInput(method)` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L20) — Drain stdin before exiting to prevent Kitty key release events from
  - `enterAltScreen(method)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L33)
  - `hideCursor(method)` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L25)
  - `leaveAltScreen(method)` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L36)
  - `moveBy(method)` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L24)
  - `setMouseTracking(method)` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L40)
  - `setProgress(method)` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L31)
  - `setTitle(method)` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L30)
  - `showCursor(method)` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L26)
  - `start(method)` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L18)
  - `stop(method)` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L19)
  - `write(method)` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L21)
  - `altScreenActive` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L32)
  - `columns` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L13)
  - `kittyProtocolActive` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L15)
  - `mouseTrackingActive` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L39)
  - `rows` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L14)
  - `writes` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L16)
- uses (calls/refs, reference-scoped): [`Terminal`](../../tui/src/terminal.ts.md#Terminal)
- used by: [`Terminal`](../../tui/src/terminal.ts.md#Terminal), [`write`](../../tui/src/terminal.ts.md#Terminal.write), [`<get>rows`](../../tui/src/terminal.ts.md#Terminal.-get-rows), [`hideCursor`](../../tui/src/terminal.ts.md#Terminal.hideCursor), [`stop`](../../tui/src/terminal.ts.md#Terminal.stop), [`setProgress`](../../tui/src/terminal.ts.md#Terminal.setProgress), [`setTitle`](../../tui/src/terminal.ts.md#Terminal.setTitle), [`showCursor`](../../tui/src/terminal.ts.md#Terminal.showCursor), [`drainInput`](../../tui/src/terminal.ts.md#Terminal.drainInput), [`leaveAltScreen`](../../tui/src/terminal.ts.md#Terminal.leaveAltScreen), [`enterAltScreen`](../../tui/src/terminal.ts.md#Terminal.enterAltScreen), [`setMouseTracking`](../../tui/src/terminal.ts.md#Terminal.setMouseTracking), [`start`](../../tui/src/terminal.ts.md#Terminal.start), [`clearFromCursor`](../../tui/src/terminal.ts.md#Terminal.clearFromCursor), [`clearLine`](../../tui/src/terminal.ts.md#Terminal.clearLine), [`clearScreen`](../../tui/src/terminal.ts.md#Terminal.clearScreen), [`moveBy`](../../tui/src/terminal.ts.md#Terminal.moveBy), [`<get>columns`](../../tui/src/terminal.ts.md#Terminal.-get-columns), [`<get>altScreenActive`](../../tui/src/terminal.ts.md#Terminal.-get-altScreenActive), [`<get>mouseTrackingActive`](../../tui/src/terminal.ts.md#Terminal.-get-mouseTrackingActive), [`<get>kittyProtocolActive`](../../tui/src/terminal.ts.md#Terminal.-get-kittyProtocolActive)  (1 test-only)

## Functions
- `createLargeEdits(lines: string[])` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L72)
- `waitForRender()` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L49)
- `waitForRenderedText(getRender: () => string, expectedText: string, onRetry?: (() => void) | undefined, timeoutMs?: number)` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/edit-tool-no-full-redraw.test.ts#L53)

