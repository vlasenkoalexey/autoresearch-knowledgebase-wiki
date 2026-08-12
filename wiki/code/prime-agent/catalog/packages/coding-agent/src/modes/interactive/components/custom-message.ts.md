---
title: 'Module: packages/coding-agent/src/modes/interactive/components/custom-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/custom-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`custom-message.ts`/CustomMessageComponent#
symbols:
  CustomMessageComponent.rebuild: rebuild().
  CustomMessageComponent.-constructor: '`<constructor>`().'
  CustomMessageComponent.box: box.
  CustomMessageComponent.message: message.
  CustomMessageComponent.customComponent: customComponent.
  CustomMessageComponent.setExpanded: setExpanded().
  CustomMessageComponent: ''
  CustomMessageComponent.customRenderer: customRenderer.
  CustomMessageComponent.invalidate: invalidate().
  CustomMessageComponent.markdownTheme: markdownTheme.
  CustomMessageComponent._expanded: _expanded.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/custom-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts)

## Classes
### `CustomMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/custom-message.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L12)
- doc: Component that renders a custom message entry from extensions.
- signature: `class CustomMessageComponent`
- members:
  - `<constructor>(message: CustomMessage<unknown>, customRenderer?: MessageRenderer | undefined, markdownTheme?: MarkdownTheme)` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L20) — Component that renders a custom message entry from extensions.
  - `invalidate(method)` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L45) — Invalidate any cached rendering state.
  - `rebuild(method)` — [`L50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L50)
  - `setExpanded(method)` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L38)
  - `box` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L15)
  - `customComponent` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L16)
  - `customRenderer` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L14)
  - `markdownTheme` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L17)
  - `message` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L13)
- protocol/private: `_expanded`[`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/custom-message.ts#L18)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`type`](../../../../../ai/src/types.ts.md#TextContent.type), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`type`](../../../../../ai/src/types.ts.md#ImageContent.type), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`text`](../../../../../ai/src/types.ts.md#TextContent.text), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`customType`](../../../core/messages.ts.md#CustomMessage.customType), [`TextContent`](../../../../../ai/src/types.ts.md#TextContent), [`content`](../../../core/messages.ts.md#CustomMessage.content), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`CustomMessage`](../../../core/messages.ts.md#CustomMessage), [`bg`](../theme/theme.ts.md#Theme.bg), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`MessageRenderer`](../../../core/extensions/types.ts.md#MessageRenderer), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`removeChild`](../../../../../tui/src/tui.ts.md#Container.removeChild), [`clear`](../../../../../tui/src/components/box.ts.md#Box.clear), [`expanded`](../../../core/extensions/types.ts.md#MessageRenderOptions.expanded)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`invalidate`](../../../../../tui/src/tui.ts.md#Container.invalidate)

