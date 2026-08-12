---
title: 'Module: packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`compaction-outcome-message.ts`/
symbols:
  CompactionOutcomeMessageComponent.-constructor: CompactionOutcomeMessageComponent#`<constructor>`().
  MalformedCompactionOutcomeMessageComponent.-constructor: MalformedCompactionOutcomeMessageComponent#`<constructor>`().
  CompactionOutcomeMessageComponent: CompactionOutcomeMessageComponent#
  MalformedCompactionOutcomeMessageComponent: MalformedCompactionOutcomeMessageComponent#
  CompactionOutcomeMessageComponent.setExpanded: CompactionOutcomeMessageComponent#setExpanded().
  MalformedCompactionOutcomeMessageComponent.setExpanded: MalformedCompactionOutcomeMessageComponent#setExpanded().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts)

## Classes
### `CompactionOutcomeMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts:6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L6)
- doc: Renders a durable unsuccessful automatic-compaction outcome.
- signature: `class CompactionOutcomeMessageComponent`
- members:
  - `<constructor>(message: CompactionOutcomeMessage)` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L7) — Renders a durable unsuccessful automatic-compaction outcome.
  - `setExpanded(method)` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L15)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`CompactionOutcomeMessage`](../../../core/messages.ts.md#CompactionOutcomeMessage), [`outcome`](../../../core/messages.ts.md#CompactionOutcomeDetails.outcome), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor), [`details`](../../../core/messages.ts.md#CompactionOutcomeMessage.details), [`content`](../../../core/messages.ts.md#CompactionOutcomeMessage.content)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts)  (1 test-only)

### `MalformedCompactionOutcomeMessageComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts:18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L18)
- signature: `class MalformedCompactionOutcomeMessageComponent`
- members:
  - `<constructor>()` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L19)
  - `setExpanded(method)` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/compaction-outcome-message.ts#L26)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`addMessageToChat`](../interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](conversation-components.ts.md#buildConversationComponents), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts)

