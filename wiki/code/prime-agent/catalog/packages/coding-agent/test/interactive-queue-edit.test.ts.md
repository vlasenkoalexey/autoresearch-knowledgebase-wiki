---
title: 'Module: packages/coding-agent/test/interactive-queue-edit.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-queue-edit.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-queue-edit.test.ts`/
symbols:
  Harness.typeLiteral0.editor: Harness#typeLiteral0:editor.
  createHarness: createHarness().
  Harness.typeLiteral0.browseQueueSelection: Harness#typeLiteral0:browseQueueSelection.
  Harness.typeLiteral0.agentConnection: Harness#typeLiteral0:agentConnection.
  Harness.typeLiteral0.editor.typeLiteral2.setText: Harness#typeLiteral0:editor.typeLiteral2:setText.
  Harness.typeLiteral0.agentConnection.typeLiteral12.mutateQueuedMessage: Harness#typeLiteral0:agentConnection.typeLiteral12:mutateQueuedMessage.
  createHarness.queue-typeLiteral36.steering: createHarness().(queue)typeLiteral36:steering.
  createHarness.queue-typeLiteral36.followUp: createHarness().(queue)typeLiteral36:followUp.
  Harness.typeLiteral0.applyQueueSelection: Harness#typeLiteral0:applyQueueSelection.
  Harness.typeLiteral0.editor.typeLiteral2.getText: Harness#typeLiteral0:editor.typeLiteral2:getText.
  Harness.typeLiteral0.queueSelection: Harness#typeLiteral0:queueSelection.
  proto: proto.
  Harness.typeLiteral0.connectionQueue: Harness#typeLiteral0:connectionQueue.
  Harness.typeLiteral0.connectionQueue.typeLiteral1.steering: Harness#typeLiteral0:connectionQueue.typeLiteral1:steering.
  Harness.typeLiteral0.connectionQueue.typeLiteral1.followUp: Harness#typeLiteral0:connectionQueue.typeLiteral1:followUp.
  Harness.typeLiteral0.moveQueueSelection: Harness#typeLiteral0:moveQueueSelection.
  Harness.typeLiteral0.showStatus: Harness#typeLiteral0:showStatus.
  Harness.typeLiteral0.queueMutationChain: Harness#typeLiteral0:queueMutationChain.
  Harness: Harness#
  Harness.typeLiteral0.sessionEventGeneration: Harness#typeLiteral0:sessionEventGeneration.
  Harness.typeLiteral0.pendingQueueEdit: Harness#typeLiteral0:pendingQueueEdit.
  Harness.typeLiteral0.replaceConnectionQueue: Harness#typeLiteral0:replaceConnectionQueue.
  Harness.typeLiteral0.editor.typeLiteral2.addToHistory: Harness#typeLiteral0:editor.typeLiteral2:addToHistory.
  Harness.typeLiteral0.pastedImages: Harness#typeLiteral0:pastedImages.
  Harness.typeLiteral0.agentConnection.typeLiteral12.getQueue: Harness#typeLiteral0:agentConnection.typeLiteral12:getQueue.
  Harness.typeLiteral0.inputSubmissionGeneration: Harness#typeLiteral0:inputSubmissionGeneration.
  Harness.typeLiteral0.refreshConnectionQueue: Harness#typeLiteral0:refreshConnectionQueue.
  Harness.typeLiteral0.setEditorTextFromQueueSelection: Harness#typeLiteral0:setEditorTextFromQueueSelection.
  Harness.typeLiteral0.collectQueueReplaceImages: Harness#typeLiteral0:collectQueueReplaceImages.
  Harness.typeLiteral0.isApplyingQueueSelectionText: Harness#typeLiteral0:isApplyingQueueSelectionText.
  Harness.typeLiteral0.updatePendingMessagesDisplay: Harness#typeLiteral0:updatePendingMessagesDisplay.
  Harness.typeLiteral0.showError: Harness#typeLiteral0:showError.
  Harness.typeLiteral0.ui: Harness#typeLiteral0:ui.
  Harness.typeLiteral0.ui.typeLiteral11.requestRender: Harness#typeLiteral0:ui.typeLiteral11:requestRender.
  Harness.typeLiteral0.agentConnection.typeLiteral12.abort: Harness#typeLiteral0:agentConnection.typeLiteral12:abort.
  Harness.typeLiteral0.enqueueQueueMutation: Harness#typeLiteral0:enqueueQueueMutation.
---
# Module: [`packages/coding-agent/test/interactive-queue-edit.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts)

## Classes
### `Harness`
- def: [`packages/coding-agent/test/interactive-queue-edit.test.ts:5`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L5)
- signature: `type Harness`
- members:
  - `abort` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L18)
  - `addToHistory` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L8)
  - `agentConnection` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L15)
  - `applyQueueSelection` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L25)
  - `browseQueueSelection` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L26)
  - `collectQueueReplaceImages` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L31)
  - `connectionQueue` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L7)
  - `editor` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L8)
  - `enqueueQueueMutation` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L24)
  - `followUp` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L7)
  - `getQueue` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L17)
  - `getText` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L8)
  - `inputSubmissionGeneration` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L21)
  - `isApplyingQueueSelectionText` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L9)
  - `moveQueueSelection` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L27)
  - `mutateQueuedMessage` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L16)
  - `pastedImages` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L10)
  - `pendingQueueEdit` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L22)
  - `queueMutationChain` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L23)
  - `queueSelection` — [`L6`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L6)
  - `refreshConnectionQueue` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L28)
  - `replaceConnectionQueue` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L29)
  - `requestRender` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L14)
  - `sessionEventGeneration` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L20)
  - `setEditorTextFromQueueSelection` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L30)
  - `setText` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L8)
  - `showError` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L13)
  - `showStatus` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L12)
  - `steering` — [`L7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L7)
  - `ui` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L14)
  - `updatePendingMessagesDisplay` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L11)
- uses (calls/refs, reference-scoped): [`QueueSelection`](../src/modes/interactive/queue-selection.ts.md#QueueSelection)
- used by: (2 test-only callers)

## Functions
- `createHarness(queue: { steering: string[]; followUp: string[]; }, mutateResult?: string)` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L36)

## Module values
- `followUp` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L36)
- `proto` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L34)
- `steering` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-queue-edit.test.ts#L36)

