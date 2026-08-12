---
title: 'Module: packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`slash-command-result-message.ts`/SlashCommandResultMessageComponent#
symbols:
  SlashCommandResultMessageComponent.-constructor: '`<constructor>`().'
  SlashCommandResultMessageComponent: ''
  SlashCommandResultMessageComponent.setExpanded: setExpanded().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts)

## Classes
### `SlashCommandResultMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts:6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts#L6)
- doc: Renders a durable session-command outcome with user-message spacing.
- signature: `class SlashCommandResultMessageComponent`
- members:
  - `<constructor>(message: SessionSlashCommandResultMessage)` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts#L7) — Renders a durable session-command outcome with user-message spacing.
  - `setExpanded(method)` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-result-message.ts#L14)
- uses (calls/refs, reference-scoped): [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`SessionSlashCommandResultMessage`](../../../core/messages.ts.md#SessionSlashCommandResultMessage), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor), [`content`](../../../core/messages.ts.md#SessionSlashCommandResultMessage.content)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts)  (1 test-only)

