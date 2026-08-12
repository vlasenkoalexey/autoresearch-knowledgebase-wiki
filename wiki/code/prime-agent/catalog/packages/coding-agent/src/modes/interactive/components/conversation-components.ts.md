---
title: 'Module: packages/coding-agent/src/modes/interactive/components/conversation-components.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/conversation-components.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`conversation-components.ts`/
symbols:
  buildConversationComponents: buildConversationComponents().
  isCompactAgentMessageNeighbor: isCompactAgentMessageNeighbor().
  ConversationComponentsOptions.markdownTheme: ConversationComponentsOptions#markdownTheme.
  ConversationComponentsOptions.ui: ConversationComponentsOptions#ui.
  ConversationComponentsOptions.toolOptions: ConversationComponentsOptions#toolOptions.
  ConversationComponentsOptions.getToolDefinition: ConversationComponentsOptions#getToolDefinition.
  ConversationComponentsOptions.cwd: ConversationComponentsOptions#cwd.
  ConversationComponentsOptions: ConversationComponentsOptions#
  ConversationComponentsOptions.hideThinkingBlock: ConversationComponentsOptions#hideThinkingBlock.
  ConversationComponentsOptions.hiddenThinkingLabel: ConversationComponentsOptions#hiddenThinkingLabel.
  ConversationComponentsOptions.toolsExpanded: ConversationComponentsOptions#toolsExpanded.
  ConversationComponentsOptions.agentMessagesExpanded: ConversationComponentsOptions#agentMessagesExpanded.
  ConversationComponentsOptions.isRecognizedSlashCommand: ConversationComponentsOptions#isRecognizedSlashCommand.
  readUserText: readUserText().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/conversation-components.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts)

## Classes
### `ConversationComponentsOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/conversation-components.ts:31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L31)
- signature: `interface ConversationComponentsOptions`
- members:
  - `agentMessagesExpanded` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L40)
  - `cwd` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L33)
  - `getToolDefinition` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L35)
  - `hiddenThinkingLabel` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L38)
  - `hideThinkingBlock` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L37)
  - `isRecognizedSlashCommand` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L41)
  - `markdownTheme` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L36)
  - `toolOptions` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L34)
  - `toolsExpanded` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L39)
  - `ui` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L32)
- uses (calls/refs, reference-scoped): [`TUI`](../../../../../tui/src/tui.ts.md#TUI), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`ToolExecutionDefinition`](tool-execution.ts.md#ToolExecutionDefinition), [`ToolExecutionOptions`](tool-execution.ts.md#ToolExecutionOptions)
- used by: [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents)  (2 test-only)

## Functions
- `buildConversationComponents(messages: readonly AgentMessage[], options: ConversationComponentsOptions)` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L66) — Build conversation components from a message list, matching tool results to their calls.
- `isCompactAgentMessageNeighbor(component: Component | undefined)` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L44)
- `readUserText(content: string | { type: string; text?: string | undefined; }[])` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/conversation-components.ts#L53)

