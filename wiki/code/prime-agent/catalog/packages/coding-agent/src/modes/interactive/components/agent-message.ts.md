---
title: 'Module: packages/coding-agent/src/modes/interactive/components/agent-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/agent-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`agent-message.ts`/
symbols:
  AgentMessageComponent.updateDisplay: AgentMessageComponent#updateDisplay().
  AgentMessageComponent.headerText: AgentMessageComponent#headerText().
  AgentMessageComponent: AgentMessageComponent#
  AgentMessageComponent.-constructor: AgentMessageComponent#`<constructor>`().
  AgentMessageComponent.-constructor-.options-typeLiteral26.suppressLeadingSpace: AgentMessageComponent#`<constructor>`().(options)typeLiteral26:suppressLeadingSpace.
  agentMessageBodyLines: agentMessageBodyLines().
  agentMessageSummaryLine: agentMessageSummaryLine().
  AgentMessageComponent.setExpanded: AgentMessageComponent#setExpanded().
  agentMessagePreview: agentMessagePreview().
  AgentMessageComponent.content: AgentMessageComponent#content.
  AgentMessageComponent.expanded: AgentMessageComponent#expanded.
  AgentMessageComponent.invalidate: AgentMessageComponent#invalidate().
  AgentMessageComponent.header: AgentMessageComponent#header.
  AgentMessageBodyComponent: AgentMessageBodyComponent#
  AgentMessageBodyComponent.render: AgentMessageBodyComponent#render().
  collapseText: collapseText().
  AgentMessageBodyComponent.-constructor: AgentMessageBodyComponent#`<constructor>`().
  AgentMessageBodyComponent.invalidate: AgentMessageBodyComponent#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/agent-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts)

## Classes
### `AgentMessageBodyComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/agent-message.ts:47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L47)
- signature: `class AgentMessageBodyComponent`
- members:
  - `<constructor>(message: string)` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L48)
  - `invalidate(method)` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L54) — Invalidate any cached rendering state.
  - `render(method)` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L50) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`Component`](../../../../../tui/src/tui.ts.md#Component), [`agentMessageBodyLines`](agent-message.ts.md#agentMessageBodyLines)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`updateDisplay`](agent-message.ts.md#AgentMessageComponent.updateDisplay)

### `AgentMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/agent-message.ts:57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L57)
- signature: `class AgentMessageComponent`
- members:
  - `<constructor>(message: AgentSessionMessage, _markdownTheme?: MarkdownTheme, options?: { suppressLeadingSpace?: boolean | undefined; })` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L62)
  - `headerText(method)` — [`L95`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L95)
  - `invalidate(method)` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L81) — Invalidate any cached rendering state.
  - `setExpanded(method)` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L73)
  - `updateDisplay(method)` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L86)
  - `content` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L58)
  - `expanded` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L60)
  - `header` — [`L59`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L59)
  - `suppressLeadingSpace` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L65)
- uses (calls/refs, reference-scoped): [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`formatAgentMessageParticipant`](../../../core/agent-messages.ts.md#formatAgentMessageParticipant), [`details`](../../../core/agent-messages.ts.md#AgentSessionMessage.details), [`AgentSessionMessage`](../../../core/agent-messages.ts.md#AgentSessionMessage), [`agentMessageSummaryLine`](agent-message.ts.md#agentMessageSummaryLine), [`fromRelationship`](../../../core/agent-messages.ts.md#AgentSessionMessageDetails.fromRelationship), [`agentMessagePreview`](agent-message.ts.md#agentMessagePreview), [`from`](../../../core/agent-messages.ts.md#AgentSessionMessageDetails.from), [`message`](../../../core/agent-messages.ts.md#AgentSessionMessageDetails.message), [`<constructor>`](agent-message.ts.md#AgentMessageBodyComponent.-constructor)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`startAssistantStreamingMessage`](../interactive-mode.ts.md#InteractiveMode.startAssistantStreamingMessage), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`isCompactAgentMessageNeighbor`](conversation-components.ts.md#isCompactAgentMessageNeighbor), [`expansionStateFor`](../interactive-mode.ts.md#InteractiveMode.expansionStateFor)  (3 test-only)

## Functions
- `agentMessageBodyLines(message: string, width: number)` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L34) — `╰─`-guttered message body lines shared by received and sent agent-message UI.
- `agentMessagePreview(prefixWidth: number, message: string)` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L29) — Single-line message preview sized to fit after the summary-line prefix.
- `agentMessageSummaryLine(label: string, participant: string, preview?: string | undefined)` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L20) — `◆ <label> · <participant>[ · <preview>]` summary line shared by received and sent agent-message UI.
- `collapseText(text: string)` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/agent-message.ts#L15)

