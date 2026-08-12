---
title: 'Module: packages/coding-agent/src/modes/interactive/components/user-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/user-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`user-message.ts`/
symbols:
  UserMessageComponent.-constructor: UserMessageComponent#`<constructor>`().
  SlashCommandMarkdown.-constructor: SlashCommandMarkdown#`<constructor>`().
  UserMessageComponent.render: UserMessageComponent#render().
  SlashCommandMarkdown.render: SlashCommandMarkdown#render().
  UserMessageComponent: UserMessageComponent#
  SlashCommandMarkdown.markdown: SlashCommandMarkdown#markdown.
  UserMessageComponent.contentBox: UserMessageComponent#contentBox.
  SlashCommandMarkdown.invalidate: SlashCommandMarkdown#invalidate().
  SlashCommandMarkdown.commandGraphemes: SlashCommandMarkdown#commandGraphemes.
  SlashCommandMarkdown: SlashCommandMarkdown#
  OSC133_ZONE_START: OSC133_ZONE_START.
  OSC133_ZONE_END: OSC133_ZONE_END.
  OSC133_ZONE_FINAL: OSC133_ZONE_FINAL.
  COMMAND_MASK_BASE: COMMAND_MASK_BASE.
  COMMAND_MASK_EXTRA_WIDTH: COMMAND_MASK_EXTRA_WIDTH.
  COMMAND_MASK_ZERO_WIDTH: COMMAND_MASK_ZERO_WIDTH.
  COMMAND_MASK_PATTERN: COMMAND_MASK_PATTERN.
  graphemeSegmenter: graphemeSegmenter.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/user-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts)

## Classes
### `SlashCommandMarkdown`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/user-message.ts:15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L15)
- signature: `class SlashCommandMarkdown`
- members:
  - `<constructor>(text: string, markdownTheme: MarkdownTheme)` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L19)
  - `invalidate(method)` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L51) — Invalidate any cached rendering state.
  - `render(method)` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L36) — Render the component to lines for the given viewport width
  - `commandGraphemes` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L17)
  - `markdown` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L16)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`render`](../../../../../tui/src/components/markdown.ts.md#Markdown.render), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`parseSlashCommand`](../../../core/slash-commands.ts.md#parseSlashCommand), [`Markdown`](../../../../../tui/src/components/markdown.ts.md#Markdown), [`name`](../../../core/slash-commands.ts.md#ParsedSlashCommand.name), [`invalidate`](../../../../../tui/src/components/markdown.ts.md#Markdown.invalidate), [`COMMAND_MASK_BASE`](user-message.ts.md#COMMAND_MASK_BASE), [`COMMAND_MASK_EXTRA_WIDTH`](user-message.ts.md#COMMAND_MASK_EXTRA_WIDTH), [`COMMAND_MASK_PATTERN`](user-message.ts.md#COMMAND_MASK_PATTERN), [`COMMAND_MASK_ZERO_WIDTH`](user-message.ts.md#COMMAND_MASK_ZERO_WIDTH), [`graphemeSegmenter`](user-message.ts.md#graphemeSegmenter)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`<constructor>`](user-message.ts.md#UserMessageComponent.-constructor)

### `UserMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/user-message.ts:59`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L59)
- doc: Component that renders a user message
- signature: `class UserMessageComponent`
- members:
  - `<constructor>(text: string, markdownTheme?: MarkdownTheme, isRecognizedSlashCommand?: (name: string) => boolean)` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L62) — Component that renders a user message
  - `render(method)` — [`L79`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L79) — Render the component to lines for the given viewport width
  - `contentBox` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L60)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`<constructor>`](user-message.ts.md#SlashCommandMarkdown.-constructor), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor), [`isLeadingSlashCommand`](slash-command-message.ts.md#isLeadingSlashCommand), [`OSC133_ZONE_END`](user-message.ts.md#OSC133_ZONE_END), [`OSC133_ZONE_FINAL`](user-message.ts.md#OSC133_ZONE_FINAL), [`OSC133_ZONE_START`](user-message.ts.md#OSC133_ZONE_START)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`render`](../../../../../tui/src/tui.ts.md#Container.render), [`echoLocalCommand`](../interactive-mode.ts.md#InteractiveMode.echoLocalCommand)  (1 test-only)

## Module values
- `COMMAND_MASK_BASE` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L9)
- `COMMAND_MASK_EXTRA_WIDTH` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L10)
- `COMMAND_MASK_PATTERN` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L12)
- `COMMAND_MASK_ZERO_WIDTH` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L11)
- `OSC133_ZONE_END` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L7)
- `OSC133_ZONE_FINAL` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L8)
- `OSC133_ZONE_START` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L6)
- `graphemeSegmenter` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message.ts#L13)

