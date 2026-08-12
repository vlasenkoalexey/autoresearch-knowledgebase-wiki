---
title: 'Module: packages/coding-agent/test/interactive-mode-streaming.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-mode-streaming.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-mode-streaming.test.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  EMPTY_USAGE: EMPTY_USAGE.
  createFakeInteractiveModeThis: createFakeInteractiveModeThis().
  renderChat: renderChat().
  HandleEvent: HandleEvent#
  HandleEventThis.typeLiteral0.agentRunFileChanges: HandleEventThis#typeLiteral0:agentRunFileChanges.
  HandleEventThis.typeLiteral0.chatContainer: HandleEventThis#typeLiteral0:chatContainer.
  HandleEventThis.typeLiteral0.recapContainer: HandleEventThis#typeLiteral0:recapContainer.
  HandleEventThis.typeLiteral0.streamingComponent: HandleEventThis#typeLiteral0:streamingComponent.
  HandleEventThis.typeLiteral0.streamingMessage: HandleEventThis#typeLiteral0:streamingMessage.
  HandleEventThis.typeLiteral0.ui: HandleEventThis#typeLiteral0:ui.
  HandleEventThis.typeLiteral0.pendingTools: HandleEventThis#typeLiteral0:pendingTools.
  HandleEventThis.typeLiteral0.updateConnectionStateFromEvent: HandleEventThis#typeLiteral0:updateConnectionStateFromEvent().
  HandleEventThis.typeLiteral0.getMarkdownThemeWithSettings: HandleEventThis#typeLiteral0:getMarkdownThemeWithSettings().
  HandleEventThis.typeLiteral0.getOrCreatePendingToolComponent: HandleEventThis#typeLiteral0:getOrCreatePendingToolComponent().
  HandleEventThis: HandleEventThis#
  HandleEventThis.typeLiteral0.refreshConnectionContextUsage: HandleEventThis#typeLiteral0:refreshConnectionContextUsage().
  HandleSubagentSummaryChatAction: HandleSubagentSummaryChatAction#
  HandleEventThis.typeLiteral0.getRetryAttempt: HandleEventThis#typeLiteral0:getRetryAttempt().
  GetUserInput: GetUserInput#
  HandleEventThis.typeLiteral0.isInitialized: HandleEventThis#typeLiteral0:isInitialized.
  HandleEventThis.typeLiteral0.settingsManager: HandleEventThis#typeLiteral0:settingsManager.
  HandleEventThis.typeLiteral0.settingsManager.typeLiteral1.getShowTerminalProgress: HandleEventThis#typeLiteral0:settingsManager.typeLiteral1:getShowTerminalProgress().
  HandleEventThis.typeLiteral0.connectionState: HandleEventThis#typeLiteral0:connectionState.
  HandleEventThis.typeLiteral0.connectionState.typeLiteral2.isStreaming: HandleEventThis#typeLiteral0:connectionState.typeLiteral2:isStreaming.
  HandleEventThis.typeLiteral0.toolOutputExpanded: HandleEventThis#typeLiteral0:toolOutputExpanded.
  HandleEventThis.typeLiteral0.footer: HandleEventThis#typeLiteral0:footer.
  HandleEventThis.typeLiteral0.footer.typeLiteral3.invalidate: HandleEventThis#typeLiteral0:footer.typeLiteral3:invalidate().
  HandleEventThis.typeLiteral0.sessionRecap: HandleEventThis#typeLiteral0:sessionRecap.
  HandleEventThis.typeLiteral0.hideThinkingBlock: HandleEventThis#typeLiteral0:hideThinkingBlock.
  HandleEventThis.typeLiteral0.hiddenThinkingLabel: HandleEventThis#typeLiteral0:hiddenThinkingLabel.
  HandleEventThis.typeLiteral0.getCurrentCwd: HandleEventThis#typeLiteral0:getCurrentCwd().
  HandleEventThis.typeLiteral0.stopWorkingLoader: HandleEventThis#typeLiteral0:stopWorkingLoader().
  HandleEventThis.typeLiteral0.resetPendingToolState: HandleEventThis#typeLiteral0:resetPendingToolState().
  HandleEventThis.typeLiteral0.checkShutdownRequested: HandleEventThis#typeLiteral0:checkShutdownRequested().
  HandleEventThis.typeLiteral0.applyOptimisticContextUsage: HandleEventThis#typeLiteral0:applyOptimisticContextUsage().
  HandleEventThis.typeLiteral0.setSessionHasMessages: HandleEventThis#typeLiteral0:setSessionHasMessages().
  HandleEventThis.typeLiteral0.clearShortcutGuide: HandleEventThis#typeLiteral0:clearShortcutGuide().
  HandleEventThis.typeLiteral0.addMessageToChat: HandleEventThis#typeLiteral0:addMessageToChat().
---
# Module: [`packages/coding-agent/test/interactive-mode-streaming.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts)

## Classes
### `GetUserInput`
- def: [`packages/coding-agent/test/interactive-mode-streaming.test.ts:60`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L60)
- signature: `type GetUserInput`
- used by: (1 test-only callers)

### `HandleEvent`
- def: [`packages/coding-agent/test/interactive-mode-streaming.test.ts:59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L59)
- signature: `type HandleEvent`
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionEvent`](../src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent)  (1 test-only)
- used by: (1 test-only callers)

### `HandleEventThis`
- def: [`packages/coding-agent/test/interactive-mode-streaming.test.ts:28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L28)
- signature: `type HandleEventThis`
- members:
  - `addMessageToChat(method)` — [`L56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L56)
  - `applyOptimisticContextUsage(method)` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L52)
  - `checkShutdownRequested(method)` — [`L51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L51)
  - `clearShortcutGuide(method)` — [`L55`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L55)
  - `getCurrentCwd(method)` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L48)
  - `getMarkdownThemeWithSettings(method)` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L45)
  - `getOrCreatePendingToolComponent(method)` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L46)
  - `getRetryAttempt(method)` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L47)
  - `getShowTerminalProgress(method)` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L30)
  - `invalidate(method)` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L33)
  - `refreshConnectionContextUsage(method)` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L53)
  - `resetPendingToolState(method)` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L50)
  - `setSessionHasMessages(method)` — [`L54`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L54)
  - `stopWorkingLoader(method)` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L49)
  - `updateConnectionStateFromEvent(method)` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L44)
  - `agentRunFileChanges` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L43)
  - `chatContainer` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L35)
  - `connectionState` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L31)
  - `footer` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L33)
  - `hiddenThinkingLabel` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L39)
  - `hideThinkingBlock` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L38)
  - `isInitialized` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L29)
  - `isStreaming` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L31)
  - `pendingTools` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L42)
  - `recapContainer` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L36)
  - `sessionRecap` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L37)
  - `settingsManager` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L30)
  - `streamingComponent` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L40)
  - `streamingMessage` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L41)
  - `toolOutputExpanded` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L32)
  - `ui` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L34)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`Container`](../../tui/src/tui.ts.md#Container), [`TUI`](../../tui/src/tui.ts.md#TUI), [`AgentConnectionSessionEvent`](../src/modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`ToolExecutionComponent`](../src/modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent), [`MarkdownTheme`](../../tui/src/components/markdown.ts.md#MarkdownTheme), [`AssistantMessageComponent`](../src/modes/interactive/components/assistant-message.ts.md#AssistantMessageComponent), [`FileChangeSummary`](../src/modes/interactive/components/edit-summary.ts.md#FileChangeSummary)
- used by: (3 test-only callers)

### `HandleSubagentSummaryChatAction`
- def: [`packages/coding-agent/test/interactive-mode-streaming.test.ts:64`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L64)
- signature: `type HandleSubagentSummaryChatAction`
- used by: (1 test-only callers)

## Functions
- `createAssistantMessage(text: string)` — [`L113`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L113)
- `createFakeInteractiveModeThis()` — [`L75`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L75)
- `renderChat(container: Container)` — [`L126`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L126)

## Module values
- `EMPTY_USAGE` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-streaming.test.ts#L13)

