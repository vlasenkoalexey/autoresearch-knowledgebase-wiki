---
title: 'Module: packages/coding-agent/src/modes/interactive/components/user-message-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/user-message-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`user-message-selector.ts`/UserMessage
symbols:
  UserMessageSelectorComponent.-constructor: SelectorComponent#`<constructor>`().
  UserMessageList.render: List#render().
  UserMessageList.handleInput: List#handleInput().
  UserMessageList.messages: List#messages.
  UserMessageList.selectedIndex: List#selectedIndex.
  UserMessageList.-constructor: List#`<constructor>`().
  UserMessageSelectorComponent.messageList: SelectorComponent#messageList.
  UserMessageSelectorComponent.getMessageList: SelectorComponent#getMessageList().
  UserMessageSelectorComponent: SelectorComponent#
  UserMessageList: List#
  UserMessageItem: Item#
  UserMessageList.onSelect: List#onSelect.
  UserMessageList.onCancel: List#onCancel.
  UserMessageList.maxVisible: List#maxVisible.
  UserMessageItem.id: Item#id.
  UserMessageItem.text: Item#text.
  UserMessageItem.timestamp: Item#timestamp.
  UserMessageList.invalidate: List#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/user-message-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts)

## Classes
### `UserMessageItem`
- def: [`packages/coding-agent/src/modes/interactive/components/user-message-selector.ts:5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L5)
- signature: `interface UserMessageItem`
- members:
  - `id` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L6)
  - `text` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L7)
  - `timestamp` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L8)
- used by: [`<constructor>`](user-message-selector.ts.md#UserMessageSelectorComponent.-constructor), [`render`](user-message-selector.ts.md#UserMessageList.render), [`handleInput`](user-message-selector.ts.md#UserMessageList.handleInput), [`messages`](user-message-selector.ts.md#UserMessageList.messages), [`<constructor>`](user-message-selector.ts.md#UserMessageList.-constructor)

### `UserMessageList`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/user-message-selector.ts:14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L14)
- doc: Custom user message list component with selection
- signature: `class UserMessageList`
- members:
  - `<constructor>(messages: UserMessageItem[], initialSelectedId?: string | undefined)` — [`L21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L21) — Custom user message list component with selection
  - `handleInput(method)` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L81) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L29) — Invalidate any cached rendering state.
  - `render(method)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L33) — Render the component to lines for the given viewport width
  - `maxVisible` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L19)
  - `messages` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L15)
  - `onCancel` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L18)
  - `onSelect` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L17)
  - `selectedIndex` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L16)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`bold`](../theme/theme.ts.md#Theme.bold), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`UserMessageItem`](user-message-selector.ts.md#UserMessageItem), [`id`](user-message-selector.ts.md#UserMessageItem.id), [`text`](user-message-selector.ts.md#UserMessageItem.text)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`<constructor>`](user-message-selector.ts.md#UserMessageSelectorComponent.-constructor), [`messageList`](user-message-selector.ts.md#UserMessageSelectorComponent.messageList), [`getMessageList`](user-message-selector.ts.md#UserMessageSelectorComponent.getMessageList)

### `UserMessageSelectorComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/modes/interactive/components/user-message-selector.ts:110`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L110)
- doc: Component that renders a user message selector for branching
- signature: `class UserMessageSelectorComponent`
- members:
  - `<constructor>(messages: UserMessageItem[], onSelect: (entryId: string) => void, onCancel: () => void, initialSelectedId?: string | undefined)` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L113) — Component that renders a user message selector for branching
  - `getMessageList(method)` — [`L152`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L152)
  - `messageList` — [`L111`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/user-message-selector.ts#L111)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`bold`](../theme/theme.ts.md#Theme.bold), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`<constructor>`](user-message-selector.ts.md#UserMessageList.-constructor), [`UserMessageList`](user-message-selector.ts.md#UserMessageList), [`UserMessageItem`](user-message-selector.ts.md#UserMessageItem), [`onCancel`](user-message-selector.ts.md#UserMessageList.onCancel), [`onSelect`](user-message-selector.ts.md#UserMessageList.onSelect)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`showUserMessageSelector`](../interactive-mode.ts.md#InteractiveMode.showUserMessageSelector)

