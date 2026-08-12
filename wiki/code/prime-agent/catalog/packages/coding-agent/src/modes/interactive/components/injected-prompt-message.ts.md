---
title: 'Module: packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`injected-prompt-message.ts`/
symbols:
  isInjectedPromptMessage: isInjectedPromptMessage().
  InjectedPromptMessageComponent.headerText: InjectedPromptMessageComponent#headerText().
  InjectedPromptMessageComponent.updateDisplay: InjectedPromptMessageComponent#updateDisplay().
  InjectedPromptMessageComponent.-constructor: InjectedPromptMessageComponent#`<constructor>`().
  InjectedPromptMessageComponent.heartbeatHeaderText: InjectedPromptMessageComponent#heartbeatHeaderText().
  InjectedPromptMessageComponent.metaText: InjectedPromptMessageComponent#metaText().
  InjectedPromptDetails: InjectedPromptDetails#
  readCustomText: readCustomText().
  InjectedPromptMessageComponent.setExpanded: InjectedPromptMessageComponent#setExpanded().
  InjectedPromptMessageComponent: InjectedPromptMessageComponent#
  InjectedPromptMessage: InjectedPromptMessage#
  InjectedPromptMessageComponent.content: InjectedPromptMessageComponent#content.
  goalLabel: goalLabel().
  InjectedPromptMessageComponent.expanded: InjectedPromptMessageComponent#expanded.
  InjectedPromptMessageComponent.invalidate: InjectedPromptMessageComponent#invalidate().
  InjectedPromptMessageComponent.header: InjectedPromptMessageComponent#header.
  heartbeatPromptSchedule: heartbeatPromptSchedule().
  collapseText: collapseText().
  compactHeartbeatSchedule: compactHeartbeatSchedule().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts)

## Classes
### `InjectedPromptDetails`
- def: [`packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts:26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L26)
- signature: `type InjectedPromptDetails`
- uses (calls/refs, reference-scoped): [`GoalContextDetails`](../../../core/goals.ts.md#GoalContextDetails), [`IpythonStateRestoredDetails`](../../../core/messages.ts.md#IpythonStateRestoredDetails), [`HeartbeatPromptDetails`](../../../core/messages.ts.md#HeartbeatPromptDetails), [`RlmChildFailureDetails`](../../../core/messages.ts.md#RlmChildFailureDetails), [`RlmChildTerminalNoticeDetails`](../../../core/messages.ts.md#RlmChildTerminalNoticeDetails)
- used by: [`InjectedPromptMessage`](injected-prompt-message.ts.md#InjectedPromptMessage)

### `InjectedPromptMessage`
- def: [`packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts:32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L32)
- signature: `type InjectedPromptMessage`
- uses (calls/refs, reference-scoped): [`CustomMessage`](../../../core/messages.ts.md#CustomMessage), [`InjectedPromptDetails`](injected-prompt-message.ts.md#InjectedPromptDetails)
- used by: [`isInjectedPromptMessage`](injected-prompt-message.ts.md#isInjectedPromptMessage), [`<constructor>`](injected-prompt-message.ts.md#InjectedPromptMessageComponent.-constructor)

### `InjectedPromptMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts:82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L82)
- signature: `class InjectedPromptMessageComponent`
- members:
  - `<constructor>(message: InjectedPromptMessage, markdownTheme?: MarkdownTheme)` — [`L87`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L87)
  - `headerText(method)` — [`L124`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L124)
  - `heartbeatHeaderText(method)` — [`L148`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L148)
  - `invalidate(method)` — [`L105`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L105) — Invalidate any cached rendering state.
  - `metaText(method)` — [`L156`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L156)
  - `setExpanded(method)` — [`L97`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L97)
  - `updateDisplay(method)` — [`L110`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L110)
  - `content` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L83)
  - `expanded` — [`L85`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L85)
  - `header` — [`L84`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L84)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`customType`](../../../core/messages.ts.md#CustomMessage.customType), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`details`](../../../core/messages.ts.md#CustomMessage.details), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`setText`](../../../../../tui/src/components/text.ts.md#Text.setText), [`readCustomText`](injected-prompt-message.ts.md#readCustomText), [`IPYTHON_STATE_RESTORED_CUSTOM_TYPE`](../../../core/messages.ts.md#IPYTHON_STATE_RESTORED_CUSTOM_TYPE), [`HEARTBEAT_PROMPT_CUSTOM_TYPE`](../../../core/messages.ts.md#HEARTBEAT_PROMPT_CUSTOM_TYPE), [`InjectedPromptMessage`](injected-prompt-message.ts.md#InjectedPromptMessage), [`GoalContextDetails`](../../../core/goals.ts.md#GoalContextDetails), [`goalLabel`](injected-prompt-message.ts.md#goalLabel), [`IpythonStateRestoredDetails`](../../../core/messages.ts.md#IpythonStateRestoredDetails), [`HeartbeatPromptDetails`](../../../core/messages.ts.md#HeartbeatPromptDetails), [`RLM_CHILD_FAILURE_CUSTOM_TYPE`](../../../core/messages.ts.md#RLM_CHILD_FAILURE_CUSTOM_TYPE), [`RLM_CHILD_TERMINAL_NOTICE_CUSTOM_TYPE`](../../../core/messages.ts.md#RLM_CHILD_TERMINAL_NOTICE_CUSTOM_TYPE), [`heartbeatPromptSchedule`](injected-prompt-message.ts.md#heartbeatPromptSchedule), [`objective`](../../../core/goals.ts.md#GoalContextDetails.objective), [`collapseText`](injected-prompt-message.ts.md#collapseText), [`restored`](../../../core/messages.ts.md#IpythonStateRestoredDetails.restored), [`schedule`](../../../core/messages.ts.md#HeartbeatPromptDetails.schedule)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate)  (4 test-only)

## Functions
- `collapseText(text: string)` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L52)
- `compactHeartbeatSchedule(schedule: string | undefined)` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L69)
- `goalLabel(details: GoalContextDetails | undefined)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L56)
- `heartbeatPromptSchedule(schedule: string | undefined)` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L77)
- `isInjectedPromptMessage(message: AgentMessage)` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L34)
- `readCustomText(message: CustomMessage<unknown>)` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/injected-prompt-message.ts#L45)

