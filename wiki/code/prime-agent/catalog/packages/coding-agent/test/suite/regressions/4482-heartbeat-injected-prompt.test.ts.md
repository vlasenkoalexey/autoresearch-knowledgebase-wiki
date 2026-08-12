---
title: 'Module: packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4482-heartbeat-injected-prompt.test.ts`/
symbols:
  createHeartbeat: createHeartbeat().
  handleMessageStart: handleMessageStart().
  render: render().
  AddMessageToChatHost.typeLiteral0.addMessageToChat: AddMessageToChatHost#typeLiteral0:addMessageToChat().
  createMessageStartMode: createMessageStartMode().
  LegacyHeartbeatRenderMode.typeLiteral2.connectionState.typeLiteral3.heartbeat: LegacyHeartbeatRenderMode#typeLiteral2:connectionState.typeLiteral3:heartbeat.
  LegacyHeartbeatRenderMode.typeLiteral2.chatContainer: LegacyHeartbeatRenderMode#typeLiteral2:chatContainer.
  LegacyHeartbeatRenderMode.typeLiteral2.getMarkdownThemeWithSettings: LegacyHeartbeatRenderMode#typeLiteral2:getMarkdownThemeWithSettings.
  MessageStartHandleMode: MessageStartHandleMode#
  MessageStartHandleMode.typeLiteral7.addMessageToChat: MessageStartHandleMode#typeLiteral7:addMessageToChat.
  MessageStartHandleHost: MessageStartHandleHost#
  MessageStartHandleHost.typeLiteral17.handleEvent: MessageStartHandleHost#typeLiteral17:handleEvent().
  LegacyHeartbeatRenderMode: LegacyHeartbeatRenderMode#
  stripAnsi: stripAnsi().
  AddMessageToChatHost: AddMessageToChatHost#
  LegacyHeartbeatRenderMode.typeLiteral2.connectionState: LegacyHeartbeatRenderMode#typeLiteral2:connectionState.
  LegacyHeartbeatRenderMode.typeLiteral2.toolOutputExpanded: LegacyHeartbeatRenderMode#typeLiteral2:toolOutputExpanded.
  LegacyHeartbeatRenderMode.typeLiteral2.editor: LegacyHeartbeatRenderMode#typeLiteral2:editor.
  MessageStartHandleMode.typeLiteral7.sessionRecap: MessageStartHandleMode#typeLiteral7:sessionRecap.
  MessageStartHandleMode.typeLiteral7.renderRecap: MessageStartHandleMode#typeLiteral7:renderRecap.
  MessageStartHandleMode.typeLiteral7.updatePendingMessagesDisplay: MessageStartHandleMode#typeLiteral7:updatePendingMessagesDisplay.
  LegacyHeartbeatRenderMode.typeLiteral2.editor.typeLiteral4.addToHistory: LegacyHeartbeatRenderMode#typeLiteral2:editor.typeLiteral4:addToHistory.
  MessageStartHandleHost.typeLiteral17.handleEvent.event-typeLiteral18.type: MessageStartHandleHost#typeLiteral17:handleEvent().(event)typeLiteral18:type.
  MessageStartHandleHost.typeLiteral17.handleEvent.event-typeLiteral18.message: MessageStartHandleHost#typeLiteral17:handleEvent().(event)typeLiteral18:message.
  AddMessageToChatHost.typeLiteral0.addMessageToChat.options-typeLiteral1.populateHistory: AddMessageToChatHost#typeLiteral0:addMessageToChat().(options)typeLiteral1:populateHistory.
  MessageStartHandleMode.typeLiteral7.isInitialized: MessageStartHandleMode#typeLiteral7:isInitialized.
  MessageStartHandleMode.typeLiteral7.footer: MessageStartHandleMode#typeLiteral7:footer.
  MessageStartHandleMode.typeLiteral7.footer.typeLiteral8.invalidate: MessageStartHandleMode#typeLiteral7:footer.typeLiteral8:invalidate.
  MessageStartHandleMode.typeLiteral7.updateConnectionStateFromEvent: MessageStartHandleMode#typeLiteral7:updateConnectionStateFromEvent.
  MessageStartHandleMode.typeLiteral7.contextUsageTokenBaseline: MessageStartHandleMode#typeLiteral7:contextUsageTokenBaseline.
  MessageStartHandleMode.typeLiteral7.activityTracker: MessageStartHandleMode#typeLiteral7:activityTracker.
  MessageStartHandleMode.typeLiteral7.activityTracker.typeLiteral11.handleEvent: MessageStartHandleMode#typeLiteral7:activityTracker.typeLiteral11:handleEvent.
  MessageStartHandleMode.typeLiteral7.updateWorkingLoaderMessage: MessageStartHandleMode#typeLiteral7:updateWorkingLoaderMessage.
  MessageStartHandleMode.typeLiteral7.ui: MessageStartHandleMode#typeLiteral7:ui.
  MessageStartHandleMode.typeLiteral7.ui.typeLiteral16.requestRender: MessageStartHandleMode#typeLiteral7:ui.typeLiteral16:requestRender.
---
# Module: [`packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts)

## Classes
### `AddMessageToChatHost`
- def: [`packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts:17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L17)
- signature: `type AddMessageToChatHost`
- members:
  - `addMessageToChat(method)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L18)
  - `populateHistory` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L21)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)  (1 test-only)
- used by: (1 test-only callers)

### `LegacyHeartbeatRenderMode`
- def: [`packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L25)
- signature: `type LegacyHeartbeatRenderMode`
- members:
  - `addToHistory` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L29)
  - `chatContainer` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L27)
  - `connectionState` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L26)
  - `editor` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L29)
  - `getMarkdownThemeWithSettings` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L30)
  - `heartbeat` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L26)
  - `toolOutputExpanded` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L28)
- uses (calls/refs, reference-scoped): [`Container`](../../../../tui/src/tui.ts.md#Container), [`AgentCronJob`](../../../src/core/cron-jobs.ts.md#AgentCronJob), [`MarkdownTheme`](../../../../tui/src/components/markdown.ts.md#MarkdownTheme)
- used by: (2 test-only callers)

### `MessageStartHandleHost`
- def: [`packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts:47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L47)
- signature: `type MessageStartHandleHost`
- members:
  - `handleEvent(method)` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L48)
  - `message` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L48)
  - `type` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L48)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)  (1 test-only)
- used by: (1 test-only callers)

### `MessageStartHandleMode`
- def: [`packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L33)
- signature: `type MessageStartHandleMode`
- members:
  - `activityTracker` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L38)
  - `addMessageToChat` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L40)
  - `contextUsageTokenBaseline` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L37)
  - `footer` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L35)
  - `handleEvent` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L38)
  - `invalidate` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L35)
  - `isInitialized` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L34)
  - `renderRecap` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L43)
  - `requestRender` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L41)
  - `sessionRecap` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L42)
  - `ui` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L41)
  - `updateConnectionStateFromEvent` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L36)
  - `updatePendingMessagesDisplay` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L44)
  - `updateWorkingLoaderMessage` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L39)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage)
- used by: (4 test-only callers)

## Functions
- `createHeartbeat()` — [`L59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L59)
- `createMessageStartMode(sessionRecap?: string)` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L77)
- `handleMessageStart(mode: MessageStartHandleMode, message: AgentMessage)` — [`L93`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L93)
- `render(component: InjectedPromptMessageComponent)` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L55)
- `stripAnsi(text: string)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4482-heartbeat-injected-prompt.test.ts#L51)

