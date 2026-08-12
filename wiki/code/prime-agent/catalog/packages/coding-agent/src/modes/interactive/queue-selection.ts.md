---
title: 'Module: packages/coding-agent/src/modes/interactive/queue-selection.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/queue-selection.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`queue-selection.ts`/
symbols:
  QueueSelection.move: QueueSelection#move().
  QueueSelection.sync: QueueSelection#sync().
  QueueSelection.reset: QueueSelection#reset().
  QueueSelection.-get-selected: QueueSelection#`<get>selected`().
  QueueSelection: QueueSelection#
  QueueSelectionItem.text: QueueSelectionItem#text.
  QueueSelectionItem.lane: QueueSelectionItem#lane.
  QueueSelection.items: QueueSelection#items.
  QueueSelection.-get-isBrowsing: QueueSelection#`<get>isBrowsing`().
  flatten: flatten().
  QueueSelection.cursor: QueueSelection#cursor.
  QueueSelection.replaceDraft: QueueSelection#replaceDraft().
  QueueSelectionItem.index: QueueSelectionItem#index.
  QueueSelection.-get-hasDraft: QueueSelection#`<get>hasDraft`().
  QueueSelection.hasStashedDraft: QueueSelection#hasStashedDraft.
  QueueSelection.draft: QueueSelection#draft.
  QueueSelectionItem: QueueSelectionItem#
  QueueLane: QueueLane#
---
# Module: [`packages/coding-agent/src/modes/interactive/queue-selection.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts)

## Classes
### `QueueLane`
- def: [`packages/coding-agent/src/modes/interactive/queue-selection.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L3)
- signature: `type QueueLane`
- used by: [`lane`](queue-selection.ts.md#QueueSelectionItem.lane)

### `QueueSelection`
- def: [`packages/coding-agent/src/modes/interactive/queue-selection.ts:18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L18)
- doc: Tracks which queued message the user is browsing/editing with alt+up/alt+down.
- signature: `class QueueSelection`
- members:
  - `<get>hasDraft` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L32)
  - `<get>isBrowsing` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L28)
  - `<get>selected` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L24)
  - `move(method)` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L42) — Move the cursor. -1 browses older, +1 newer. Returns the text to show, or undefined for a boundary noop.
  - `replaceDraft(method)` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L36)
  - `reset(method)` — [`L85`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L85) — Called after a mutation or submit resolved the selection. Returns the stashed draft.
  - `sync(method)` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L70) — Track queue changes while browsing: keep the selection when its text is
  - `cursor` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L20)
  - `draft` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L21)
  - `hasStashedDraft` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L22)
  - `items` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L19)
- uses (calls/refs, reference-scoped): [`AgentConnectionQueueState`](../agent-connection/types.ts.md#AgentConnectionQueueState), [`steering`](../agent-connection/types.ts.md#AgentConnectionQueueState.steering), [`text`](queue-selection.ts.md#QueueSelectionItem.text), [`lane`](queue-selection.ts.md#QueueSelectionItem.lane), [`flatten`](queue-selection.ts.md#flatten), [`index`](queue-selection.ts.md#QueueSelectionItem.index), [`QueueSelectionItem`](queue-selection.ts.md#QueueSelectionItem)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`setupEditorSubmitHandler`](interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`resetCurrentSessionRenderState`](interactive-mode.ts.md#InteractiveMode.resetCurrentSessionRenderState), [`applyQueueSelection`](interactive-mode.ts.md#InteractiveMode.applyQueueSelection), [`moveQueueSelection`](interactive-mode.ts.md#InteractiveMode.moveQueueSelection), [`handleFollowUp`](interactive-mode.ts.md#InteractiveMode.handleFollowUp), [`replaceConnectionQueue`](interactive-mode.ts.md#InteractiveMode.replaceConnectionQueue), [`browseQueueSelection`](interactive-mode.ts.md#InteractiveMode.browseQueueSelection), [`queueSelection`](interactive-mode.ts.md#InteractiveMode.queueSelection), [`clearInputBar`](interactive-mode.ts.md#InteractiveMode.clearInputBar), [`getQueueSelectionHeader`](interactive-mode.ts.md#InteractiveMode.getQueueSelectionHeader)  (7 test-only)

### `QueueSelectionItem`
- def: [`packages/coding-agent/src/modes/interactive/queue-selection.ts:5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L5)
- signature: `interface QueueSelectionItem`
- members:
  - `index` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L7)
  - `lane` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L6)
  - `text` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L8)
- uses (calls/refs, reference-scoped): [`QueueLane`](queue-selection.ts.md#QueueLane)
- used by: [`applyQueueSelection`](interactive-mode.ts.md#InteractiveMode.applyQueueSelection), [`moveQueueSelection`](interactive-mode.ts.md#InteractiveMode.moveQueueSelection), [`move`](queue-selection.ts.md#QueueSelection.move), [`sync`](queue-selection.ts.md#QueueSelection.sync), [`<get>selected`](queue-selection.ts.md#QueueSelection.-get-selected), [`items`](queue-selection.ts.md#QueueSelection.items), [`getQueueSelectionHeader`](interactive-mode.ts.md#InteractiveMode.getQueueSelectionHeader), [`flatten`](queue-selection.ts.md#flatten)

## Functions
- `flatten(queue: AgentConnectionQueueState)` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/queue-selection.ts#L94)

