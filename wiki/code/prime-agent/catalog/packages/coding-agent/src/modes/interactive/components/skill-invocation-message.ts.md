---
title: 'Module: packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`skill-invocation-message.ts`/SkillInvocationMessageComponent#
symbols:
  SkillInvocationMessageComponent.updateDisplay: updateDisplay().
  SkillInvocationMessageComponent.-constructor: '`<constructor>`().'
  SkillInvocationMessageComponent.skillBlock: skillBlock.
  SkillInvocationMessageComponent.setExpanded: setExpanded().
  SkillInvocationMessageComponent: ''
  SkillInvocationMessageComponent.invalidate: invalidate().
  SkillInvocationMessageComponent.markdownTheme: markdownTheme.
  SkillInvocationMessageComponent.expanded: expanded.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts)

## Classes
### `SkillInvocationMessageComponent`  ·  implements/extends Box, Component
- def: [`packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts:11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L11)
- doc: Component that renders a skill invocation message with collapsed/expanded state.
- signature: `class SkillInvocationMessageComponent`
- members:
  - `<constructor>(skillBlock: ParsedSkillBlock, markdownTheme?: MarkdownTheme)` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L16) — Component that renders a skill invocation message with collapsed/expanded state.
  - `invalidate(method)` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L28) — Invalidate any cached rendering state.
  - `setExpanded(method)` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L23)
  - `updateDisplay(method)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L33)
  - `expanded` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L12)
  - `markdownTheme` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L14)
  - `skillBlock` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/skill-invocation-message.ts#L13)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`bg`](../theme/theme.ts.md#Theme.bg), [`MarkdownTheme`](../../../../../tui/src/components/markdown.ts.md#MarkdownTheme), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`invalidate`](../../../../../tui/src/components/box.ts.md#Box.invalidate), [`clear`](../../../../../tui/src/components/box.ts.md#Box.clear), [`ParsedSkillBlock`](../../../core/skill-blocks.ts.md#ParsedSkillBlock), [`name`](../../../core/skill-blocks.ts.md#ParsedSkillBlock.name), [`content`](../../../core/skill-blocks.ts.md#ParsedSkillBlock.content)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`invalidate`](../../../../../tui/src/components/box.ts.md#Box.invalidate)

