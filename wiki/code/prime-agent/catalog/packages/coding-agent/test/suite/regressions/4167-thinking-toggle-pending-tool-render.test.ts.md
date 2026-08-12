---
title: 'Module: packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4167-thinking-toggle-pending-tool-render.test.ts`/
symbols:
  createFakeInteractiveModeThis: createFakeInteractiveModeThis().
  createAssistantToolCallMessage: createAssistantToolCallMessage().
  EMPTY_USAGE: EMPTY_USAGE.
  createToolResultMessage: createToolResultMessage().
  createSessionContext: createSessionContext().
  RenderSessionContext: RenderSessionContext#
  renderChat: renderChat().
  RenderSessionContextThis.typeLiteral0.pendingTools: RenderSessionContextThis#typeLiteral0:pendingTools.
  HandleEvent: HandleEvent#
  RenderSessionContextThis.typeLiteral0.chatContainer: RenderSessionContextThis#typeLiteral0:chatContainer.
  TOOL_CALL_ID: TOOL_CALL_ID.
  RenderSessionContextThis: RenderSessionContextThis#
  RenderSessionContextThis.typeLiteral0.ipythonToolComponents: RenderSessionContextThis#typeLiteral0:ipythonToolComponents.
  RenderSessionContextThis.typeLiteral0.ui: RenderSessionContextThis#typeLiteral0:ui.
  RenderSessionContextThis.typeLiteral0.activityTracker: RenderSessionContextThis#typeLiteral0:activityTracker.
  RenderSessionContextThis.typeLiteral0.updateConnectionStateFromEvent: RenderSessionContextThis#typeLiteral0:updateConnectionStateFromEvent().
  RenderSessionContextThis.typeLiteral0.addMessageToChat: RenderSessionContextThis#typeLiteral0:addMessageToChat().
  TOOL_NAME: TOOL_NAME.
  RenderSessionContextThis.typeLiteral0.lateIpythonSentAgentMessages: RenderSessionContextThis#typeLiteral0:lateIpythonSentAgentMessages.
  RenderSessionContextThis.typeLiteral0.pendingToolCreations: RenderSessionContextThis#typeLiteral0:pendingToolCreations.
  RenderSessionContextThis.typeLiteral0.startedToolCalls: RenderSessionContextThis#typeLiteral0:startedToolCalls.
  RenderSessionContextThis.typeLiteral0.resetPendingToolState: RenderSessionContextThis#typeLiteral0:resetPendingToolState().
  RenderSessionContextThis.typeLiteral0.footer: RenderSessionContextThis#typeLiteral0:footer.
  RenderSessionContextThis.typeLiteral0.footer.typeLiteral1.invalidate: RenderSessionContextThis#typeLiteral0:footer.typeLiteral1:invalidate().
  RenderSessionContextThis.typeLiteral0.settingsManager: RenderSessionContextThis#typeLiteral0:settingsManager.
  RenderSessionContextThis.typeLiteral0.settingsManager.typeLiteral2.getShowImages: RenderSessionContextThis#typeLiteral0:settingsManager.typeLiteral2:getShowImages().
  RenderSessionContextThis.typeLiteral0.toolOutputExpanded: RenderSessionContextThis#typeLiteral0:toolOutputExpanded.
  RenderSessionContextThis.typeLiteral0.isInitialized: RenderSessionContextThis#typeLiteral0:isInitialized.
  RenderSessionContextThis.typeLiteral0.updateWorkingLoaderMessage: RenderSessionContextThis#typeLiteral0:updateWorkingLoaderMessage().
  RenderSessionContextThis.typeLiteral0.updateEditorBorderColor: RenderSessionContextThis#typeLiteral0:updateEditorBorderColor().
  RenderSessionContextThis.typeLiteral0.getCurrentCwd: RenderSessionContextThis#typeLiteral0:getCurrentCwd().
  RenderSessionContextThis.typeLiteral0.getRetryAttempt: RenderSessionContextThis#typeLiteral0:getRetryAttempt().
  RenderSessionContextThis.typeLiteral0.preloadToolDefinitions: RenderSessionContextThis#typeLiteral0:preloadToolDefinitions().
  RenderSessionContextThis.typeLiteral0.getCachedToolDefinition: RenderSessionContextThis#typeLiteral0:getCachedToolDefinition().
  RenderSessionContextThis.typeLiteral0.addMessageToChat.options-typeLiteral3.populateHistory: RenderSessionContextThis#typeLiteral0:addMessageToChat().(options)typeLiteral3:populateHistory.
---
# Module: [`packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts)

## Classes
### `HandleEvent`
- def: [`packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts:65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L65)
- signature: `type HandleEvent`
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEvent`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent)  (1 test-only)
- used by: (1 test-only callers)

### `RenderSessionContext`
- def: [`packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts:59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L59)
- signature: `type RenderSessionContext`
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionContext`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionSessionContext)  (1 test-only)
- used by: (1 test-only callers)

### `RenderSessionContextThis`
- def: [`packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts:33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L33)
- signature: `type RenderSessionContextThis`
- members:
  - `addMessageToChat(method)` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L56)
  - `getCachedToolDefinition(method)` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L55)
  - `getCurrentCwd(method)` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L52)
  - `getRetryAttempt(method)` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L53)
  - `getShowImages(method)` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L44)
  - `invalidate(method)` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L41)
  - `preloadToolDefinitions(method)` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L54)
  - `resetPendingToolState(method)` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L39)
  - `updateConnectionStateFromEvent(method)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L51)
  - `updateEditorBorderColor(method)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L50)
  - `updateWorkingLoaderMessage(method)` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L49)
  - `activityTracker` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L48)
  - `chatContainer` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L40)
  - `footer` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L41)
  - `ipythonToolComponents` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L35)
  - `isInitialized` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L47)
  - `lateIpythonSentAgentMessages` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L36)
  - `pendingToolCreations` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L37)
  - `pendingTools` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L34)
  - `populateHistory` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L56)
  - `settingsManager` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L43)
  - `startedToolCalls` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L38)
  - `toolOutputExpanded` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L46)
  - `ui` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L42)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../../agent/src/types.ts.md#AgentMessage), [`Container`](../../../../tui/src/tui.ts.md#Container), [`TUI`](../../../../tui/src/tui.ts.md#TUI), [`AgentConnectionSessionEvent`](../../../src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`ToolExecutionComponent`](../../../src/modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent), [`AgentActivityTracker`](../../../src/modes/interactive/agent-activity.ts.md#AgentActivityTracker)
- used by: (4 test-only callers)

## Functions
- `createAssistantToolCallMessage()` — [`L107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L107)
- `createFakeInteractiveModeThis()` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L67)
- `createSessionContext(messages: AgentMessage[])` — [`L138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L138)
- `createToolResultMessage(text: string)` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L127)
- `renderChat(container: Container)` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L147)

## Module values
- `EMPTY_USAGE` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L18)
- `TOOL_CALL_ID` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L15)
- `TOOL_NAME` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4167-thinking-toggle-pending-tool-render.test.ts#L16)

