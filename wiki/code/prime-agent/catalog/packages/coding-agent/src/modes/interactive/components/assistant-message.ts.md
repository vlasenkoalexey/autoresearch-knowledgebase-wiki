---
title: 'Module: packages/coding-agent/src/modes/interactive/components/assistant-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/assistant-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`assistant-message.ts`/
symbols:
  AssistantMessageComponent.rebuild: AssistantMessageComponent#rebuild().
  AssistantMessageComponent.-constructor: AssistantMessageComponent#`<constructor>`().
  AssistantMessageComponent.render: AssistantMessageComponent#render().
  getThinkingMarkdownTheme: getThinkingMarkdownTheme().
  AssistantMessageComponent.computeSignature: AssistantMessageComponent#computeSignature().
  AssistantMessageComponent.reconcile: AssistantMessageComponent#reconcile().
  AssistantMessageComponent.createErrorComponent: AssistantMessageComponent#createErrorComponent().
  AssistantMessageComponent.updateContent: AssistantMessageComponent#updateContent().
  AssistantMessageComponent: AssistantMessageComponent#
  AssistantMessageComponent.contentContainer: AssistantMessageComponent#contentContainer.
  formatInlineLoginRecoveryMessage: formatInlineLoginRecoveryMessage().
  CollapsedThinkingRow.render: CollapsedThinkingRow#render().
  AssistantMessageComponent.setHideThinkingBlock: AssistantMessageComponent#setHideThinkingBlock().
  AssistantMessageComponent.invalidate: AssistantMessageComponent#invalidate().
  AssistantMessageComponent.dirty: AssistantMessageComponent#dirty.
  AssistantMessageComponent.setHiddenThinkingLabel: AssistantMessageComponent#setHiddenThinkingLabel().
  thinkingRecap: thinkingRecap().
  AssistantMessageComponent.blockMarkdowns: AssistantMessageComponent#blockMarkdowns.
  AssistantMessageComponent.hiddenThinkingLabel: AssistantMessageComponent#hiddenThinkingLabel.
  AssistantMessageComponent.setExpanded: AssistantMessageComponent#setExpanded().
  AssistantMessageComponent.markdownTheme: AssistantMessageComponent#markdownTheme.
  AssistantMessageComponent.lastMessage: AssistantMessageComponent#lastMessage.
  AssistantMessageComponent.hideThinkingBlock: AssistantMessageComponent#hideThinkingBlock.
  AssistantMessageComponent.expanded: AssistantMessageComponent#expanded.
  AssistantMessageComponent.lastBlockTexts: AssistantMessageComponent#lastBlockTexts.
  LOGIN_RECOVERY_SUFFIX: LOGIN_RECOVERY_SUFFIX.
  AssistantMessageComponent.lastSignature: AssistantMessageComponent#lastSignature.
  CollapsedThinkingRow: CollapsedThinkingRow#
  AssistantMessageComponent.hasToolCalls: AssistantMessageComponent#hasToolCalls.
  AssistantMessageComponent.precededByToolActivity: AssistantMessageComponent#precededByToolActivity.
  OSC133_ZONE_START: OSC133_ZONE_START.
  OSC133_ZONE_END: OSC133_ZONE_END.
  OSC133_ZONE_FINAL: OSC133_ZONE_FINAL.
  AssistantMessageComponentOptions: AssistantMessageComponentOptions#
  AssistantMessageComponentOptions.expanded: AssistantMessageComponentOptions#expanded.
  AssistantMessageComponentOptions.precededByToolActivity: AssistantMessageComponentOptions#precededByToolActivity.
  CollapsedThinkingRow.-constructor: CollapsedThinkingRow#`<constructor>`().
  CollapsedThinkingRow.invalidate: CollapsedThinkingRow#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/assistant-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts)

## Classes
### `AssistantMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/assistant-message.ts:113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L113)
- doc: Component that renders a complete assistant message.
- signature: `class AssistantMessageComponent`
- members:
  - `<constructor>(message?: AssistantMessage | undefined, hideThinkingBlock?: boolean, markdownTheme?: MarkdownTheme, hiddenThinkingLabel?: string, options?: AssistantMessageComponentOptions)` — [`L127`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L127) — Component that renders a complete assistant message.
  - `computeSignature(method)` — [`L202`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L202) — Everything that affects child component identity/order, but not the text
  - `createErrorComponent(method)` — [`L347`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L347)
  - `invalidate(method)` — [`L151`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L151) — Invalidate any cached rendering state.
  - `rebuild(method)` — [`L259`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L259)
  - `reconcile(method)` — [`L230`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L230)
  - `render(method)` — [`L175`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L175) — Render the component to lines for the given viewport width
  - `setExpanded(method)` — [`L168`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L168)
  - `setHiddenThinkingLabel(method)` — [`L163`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L163)
  - `setHideThinkingBlock(method)` — [`L158`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L158)
  - `updateContent(method)` — [`L192`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L192)
  - `blockMarkdowns` — [`L123`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L123)
  - `contentContainer` — [`L114`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L114)
  - `dirty` — [`L121`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L121)
  - `expanded` — [`L120`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L120)
  - `hasToolCalls` — [`L119`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L119)
  - `hiddenThinkingLabel` — [`L117`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L117)
  - `hideThinkingBlock` — [`L115`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L115)
  - `lastBlockTexts` — [`L124`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L124)
  - `lastMessage` — [`L118`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L118)
  - `lastSignature` — [`L122`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L122)
  - `markdownTheme` — [`L116`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L116)
  - `precededByToolActivity` — [`L125`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L125)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`type`](../../../../../ai/src/types.ts.md#TextContent.type), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`content`](../../../../../ai/src/types.ts.md#AssistantMessage.content), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`type`](../../../../../ai/src/types.ts.md#ToolCall.type), [`type`](../../../../../ai/src/types.ts.md#ThinkingContent.type), [`AssistantMessage`](../../../../../ai/src/types.ts.md#AssistantMessage), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`stopReason`](../../../../../ai/src/types.ts.md#AssistantMessage.stopReason), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`errorMessage`](../../../../../ai/src/types.ts.md#AssistantMessage.errorMessage), [`text`](../../../../../ai/src/types.ts.md#TextContent.text), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`bold`](../theme/theme.ts.md#Theme.bold), [`thinking`](../../../../../ai/src/types.ts.md#ThinkingContent.thinking), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`getThinkingMarkdownTheme`](assistant-message.ts.md#getThinkingMarkdownTheme), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`Markdown`](../../../../../tui/src/components/markdown.ts.md#Markdown), [`setText`](../../../../../tui/src/components/markdown.ts.md#Markdown.setText), [`summarizeErrorDetails`](collapsible-error.ts.md#summarizeErrorDetails), [`formatInlineLoginRecoveryMessage`](assistant-message.ts.md#formatInlineLoginRecoveryMessage), [`<constructor>`](collapsible-error.ts.md#CollapsibleErrorComponent.-constructor), [`shouldCollapseErrorDetails`](collapsible-error.ts.md#shouldCollapseErrorDetails), [`thinkingRecap`](assistant-message.ts.md#thinkingRecap), [`expanded`](collapsible-error.ts.md#CollapsibleErrorOptions.expanded), [`summary`](collapsible-error.ts.md#CollapsibleErrorOptions.summary), [`text`](collapsible-error.ts.md#CollapsibleErrorOptions.text), [`AssistantMessageComponentOptions`](assistant-message.ts.md#AssistantMessageComponentOptions), [`<constructor>`](assistant-message.ts.md#CollapsedThinkingRow.-constructor), [`OSC133_ZONE_END`](assistant-message.ts.md#OSC133_ZONE_END), [`OSC133_ZONE_FINAL`](assistant-message.ts.md#OSC133_ZONE_FINAL), [`OSC133_ZONE_START`](assistant-message.ts.md#OSC133_ZONE_START)  (+2 more)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`showSettingsSelector`](../interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`startAssistantStreamingMessage`](../interactive-mode.ts.md#InteractiveMode.startAssistantStreamingMessage), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`toggleThinkingBlockVisibility`](../interactive-mode.ts.md#InteractiveMode.toggleThinkingBlockVisibility), [`setHiddenThinkingLabel`](../interactive-mode.ts.md#InteractiveMode.setHiddenThinkingLabel), [`streamingComponent`](../interactive-mode.ts.md#InteractiveMode.streamingComponent), [`ensureAssistantStreamingComponent`](../interactive-mode.ts.md#InteractiveMode.ensureAssistantStreamingComponent)  (8 test-only)

### `AssistantMessageComponentOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/assistant-message.ts:27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L27)
- signature: `interface AssistantMessageComponentOptions`
- members:
  - `expanded` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L28)
  - `precededByToolActivity` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L29)
- used by: [`<constructor>`](assistant-message.ts.md#AssistantMessageComponent.-constructor)

### `CollapsedThinkingRow`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/assistant-message.ts:51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L51)
- doc: Single collapsed-thinking row that truncates the recap to the render width instead of wrapping.
- signature: `class CollapsedThinkingRow`
- members:
  - `<constructor>(label: string, recap: string, hint: string)` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L52) — Single collapsed-thinking row that truncates the recap to the render width instead of wrapping.
  - `invalidate(method)` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L67) — Invalidate any cached rendering state.
  - `render(method)` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L58) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`rebuild`](assistant-message.ts.md#AssistantMessageComponent.rebuild)

## Functions
- `formatInlineLoginRecoveryMessage(message: string)` — [`L93`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L93)
- `getThinkingMarkdownTheme(baseTheme: MarkdownTheme)` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L32)
- `thinkingRecap(thinking: string, fallback: string, maxWidth?: number)` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L75) — One-line recap for a collapsed thinking block: the last bold section header

## Module values
- `LOGIN_RECOVERY_SUFFIX` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L25)
- `OSC133_ZONE_END` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L23)
- `OSC133_ZONE_FINAL` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L24)
- `OSC133_ZONE_START` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/assistant-message.ts#L22)

