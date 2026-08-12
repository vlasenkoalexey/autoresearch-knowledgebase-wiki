---
title: 'Module: packages/coding-agent/src/modes/interactive/components/slash-command-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/slash-command-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`slash-command-message.ts`/
symbols:
  SlashCommandMessageComponent.-constructor: SlashCommandMessageComponent#`<constructor>`().
  styleSlashCommandText: styleSlashCommandText().
  SlashCommandMessageComponent.render: SlashCommandMessageComponent#render().
  isLeadingSlashCommand: isLeadingSlashCommand().
  SlashCommandMessageComponent: SlashCommandMessageComponent#
  SlashCommandMessageComponent.contentBox: SlashCommandMessageComponent#contentBox.
  OSC133_ZONE_START: OSC133_ZONE_START.
  OSC133_ZONE_END: OSC133_ZONE_END.
  OSC133_ZONE_FINAL: OSC133_ZONE_FINAL.
  SlashCommandMessageComponent.setExpanded: SlashCommandMessageComponent#setExpanded().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/slash-command-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts)

## Classes
### `SlashCommandMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/slash-command-message.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L21)
- doc: Renders a durable session command with the same layout as a user message.
- signature: `class SlashCommandMessageComponent`
- members:
  - `<constructor>(text: string)` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L24) — Renders a durable session command with the same layout as a user message.
  - `render(method)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L33) — Render the component to lines for the given viewport width
  - `setExpanded(method)` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L31)
  - `contentBox` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L22)
- uses (calls/refs, reference-scoped): [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`styleSlashCommandText`](slash-command-message.ts.md#styleSlashCommandText), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor), [`OSC133_ZONE_END`](slash-command-message.ts.md#OSC133_ZONE_END), [`OSC133_ZONE_FINAL`](slash-command-message.ts.md#OSC133_ZONE_FINAL), [`OSC133_ZONE_START`](slash-command-message.ts.md#OSC133_ZONE_START)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`render`](../../../../../tui/src/tui.ts.md#Container.render)  (1 test-only)

## Functions
- `isLeadingSlashCommand(text: string, isRecognized: (name: string) => boolean)` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L9)
- `styleSlashCommandText(text: string, styleRest?: (rest: string) => string)` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L14)

## Module values
- `OSC133_ZONE_END` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L6)
- `OSC133_ZONE_FINAL` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L7)
- `OSC133_ZONE_START` — [`L5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/slash-command-message.ts#L5)

