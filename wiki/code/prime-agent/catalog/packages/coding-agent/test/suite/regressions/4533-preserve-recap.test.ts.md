---
title: 'Module: packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4533-preserve-recap.test.ts`/
symbols:
  render: render().
  createRenderMode: createRenderMode().
  renderRecap: renderRecap.
  handleEvent: handleEvent.
  createMessageStartMode: createMessageStartMode().
  RecapRenderMode: RecapRenderMode#
  RecapRenderMode.typeLiteral0.recapContainer: RecapRenderMode#typeLiteral0:recapContainer.
  RenderRecapHost: RenderRecapHost#
  MessageStartMode.typeLiteral3.addMessageToChat: MessageStartMode#typeLiteral3:addMessageToChat.
  HandleEventHost: HandleEventHost#
  HandleEventHost.typeLiteral15.handleEvent: HandleEventHost#typeLiteral15:handleEvent().
  MessageStartMode: MessageStartMode#
  stripAnsi: stripAnsi().
  RecapRenderMode.typeLiteral0.sessionRecap: RecapRenderMode#typeLiteral0:sessionRecap.
  RenderRecapHost.typeLiteral2.renderRecap: RenderRecapHost#typeLiteral2:renderRecap().
  MessageStartMode.typeLiteral3.sessionRecap: MessageStartMode#typeLiteral3:sessionRecap.
  MessageStartMode.typeLiteral3.renderRecap: MessageStartMode#typeLiteral3:renderRecap.
  MessageStartMode.typeLiteral3.updatePendingMessagesDisplay: MessageStartMode#typeLiteral3:updatePendingMessagesDisplay.
  HandleEventHost.typeLiteral15.handleEvent.event-typeLiteral16.type: HandleEventHost#typeLiteral15:handleEvent().(event)typeLiteral16:type.
  HandleEventHost.typeLiteral15.handleEvent.event-typeLiteral16.message: HandleEventHost#typeLiteral15:handleEvent().(event)typeLiteral16:message.
  RecapRenderMode.typeLiteral0.agentRunFileChanges: RecapRenderMode#typeLiteral0:agentRunFileChanges.
  RecapRenderMode.typeLiteral0.isAgentStreaming: RecapRenderMode#typeLiteral0:isAgentStreaming.
  RecapRenderMode.typeLiteral0.ui: RecapRenderMode#typeLiteral0:ui.
  RecapRenderMode.typeLiteral0.ui.typeLiteral1.requestRender: RecapRenderMode#typeLiteral0:ui.typeLiteral1:requestRender.
  MessageStartMode.typeLiteral3.isInitialized: MessageStartMode#typeLiteral3:isInitialized.
  MessageStartMode.typeLiteral3.footer: MessageStartMode#typeLiteral3:footer.
  MessageStartMode.typeLiteral3.footer.typeLiteral4.invalidate: MessageStartMode#typeLiteral3:footer.typeLiteral4:invalidate.
  MessageStartMode.typeLiteral3.updateConnectionStateFromEvent: MessageStartMode#typeLiteral3:updateConnectionStateFromEvent.
  MessageStartMode.typeLiteral3.contextUsageTokenBaseline: MessageStartMode#typeLiteral3:contextUsageTokenBaseline.
  MessageStartMode.typeLiteral3.setSessionHasMessages: MessageStartMode#typeLiteral3:setSessionHasMessages.
  MessageStartMode.typeLiteral3.clearShortcutGuide: MessageStartMode#typeLiteral3:clearShortcutGuide.
  MessageStartMode.typeLiteral3.activityTracker: MessageStartMode#typeLiteral3:activityTracker.
  MessageStartMode.typeLiteral3.activityTracker.typeLiteral9.handleEvent: MessageStartMode#typeLiteral3:activityTracker.typeLiteral9:handleEvent.
  MessageStartMode.typeLiteral3.updateWorkingLoaderMessage: MessageStartMode#typeLiteral3:updateWorkingLoaderMessage.
  MessageStartMode.typeLiteral3.ui: MessageStartMode#typeLiteral3:ui.
  MessageStartMode.typeLiteral3.ui.typeLiteral14.requestRender: MessageStartMode#typeLiteral3:ui.typeLiteral14:requestRender.
  MessageStartMode.typeLiteral3.agentRunFileChanges: MessageStartMode#typeLiteral3:agentRunFileChanges.
---
# Module: [`packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts)

## Classes
### `HandleEventHost`
- def: [`packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L36)
- signature: `type HandleEventHost`
- members:
  - `handleEvent(method)` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L37)
  - `message` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L37)
  - `type` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L37)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)  (1 test-only)
- used by: (2 test-only callers)

### `MessageStartMode`
- def: [`packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts:19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L19)
- signature: `type MessageStartMode`
- members:
  - `activityTracker` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L26)
  - `addMessageToChat` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L28)
  - `agentRunFileChanges` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L31)
  - `clearShortcutGuide` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L25)
  - `contextUsageTokenBaseline` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L23)
  - `footer` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L21)
  - `handleEvent` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L26)
  - `invalidate` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L21)
  - `isInitialized` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L20)
  - `renderRecap` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L32)
  - `requestRender` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L29)
  - `sessionRecap` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L30)
  - `setSessionHasMessages` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L24)
  - `ui` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L29)
  - `updateConnectionStateFromEvent` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L22)
  - `updatePendingMessagesDisplay` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L33)
  - `updateWorkingLoaderMessage` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L27)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)
- used by: (3 test-only callers)

### `RecapRenderMode`
- def: [`packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts:7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L7)
- signature: `type RecapRenderMode`
- members:
  - `agentRunFileChanges` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L10)
  - `isAgentStreaming` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L11)
  - `recapContainer` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L8)
  - `requestRender` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L12)
  - `sessionRecap` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L9)
  - `ui` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L12)
- uses (calls/refs, reference-scoped): [`Container`](../../../../tui/src/tui.ts.md#Container)
- used by: (4 test-only callers)

### `RenderRecapHost`
- def: [`packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts:15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L15)
- signature: `type RenderRecapHost`
- members:
  - `renderRecap(method)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L16)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `createMessageStartMode()` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L53)
- `createRenderMode(sessionRecap?: string | undefined)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L43)
- `render(mode: RecapRenderMode, width?: number)` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L72)
- `stripAnsi(text: string)` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L77)

## Module values
- `handleEvent` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L41)
- `renderRecap` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4533-preserve-recap.test.ts#L40)

