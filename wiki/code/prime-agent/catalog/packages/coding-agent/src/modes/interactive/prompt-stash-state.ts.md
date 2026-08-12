---
title: 'Module: packages/coding-agent/src/modes/interactive/prompt-stash-state.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/prompt-stash-state.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`prompt-stash-state.ts`/
symbols:
  PromptStashState.stash: PromptStashState#stash.
  ClientPromptStashStore.forSession: ClientPromptStashStore#forSession().
  ClientPromptStashStore: ClientPromptStashStore#
  PromptStashState: PromptStashState#
  PromptStashState.queuedStashes: PromptStashState#queuedStashes.
  PromptStash.text: PromptStash#text.
  PromptStash.pasteSnapshot: PromptStash#pasteSnapshot.
  PromptStash: PromptStash#
  ClientPromptStashStore.release: ClientPromptStashStore#release().
  PromptStash.images: PromptStash#images.
  ClientPromptStashStore.states: ClientPromptStashStore#states.
  PromptStash.expandedText: PromptStash#expandedText.
---
# Module: [`packages/coding-agent/src/modes/interactive/prompt-stash-state.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts)

## Classes
### `ClientPromptStashStore`
- def: [`packages/coding-agent/src/modes/interactive/prompt-stash-state.ts:16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L16)
- signature: `class ClientPromptStashStore`
- members:
  - `forSession(method)` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L19)
  - `release(method)` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L28)
  - `states` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L17)
- uses (calls/refs, reference-scoped): [`stash`](prompt-stash-state.ts.md#PromptStashState.stash), [`PromptStashState`](prompt-stash-state.ts.md#PromptStashState), [`queuedStashes`](prompt-stash-state.ts.md#PromptStashState.queuedStashes)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main`](../../main.ts.md#main), [`main.ts`](../../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`agents-view-mode.ts`](../agents-view/agents-view-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agents-view-agents-view-mode.ts), [`<constructor>`](interactive-mode.ts.md#InteractiveMode.-constructor), [`runAgentsViewMode`](../agents-view/agents-view-mode.ts.md#runAgentsViewMode), [`releasePromptStashSession`](interactive-mode.ts.md#InteractiveMode.releasePromptStashSession), [`bindPromptStashSession`](interactive-mode.ts.md#InteractiveMode.bindPromptStashSession), [`promptStashStore`](interactive-mode.ts.md#InteractiveMode.promptStashStore), [`completeDeferredPromptStashRelease`](interactive-mode.ts.md#InteractiveMode.completeDeferredPromptStashRelease), [`promptStashStore`](interactive-mode.ts.md#InteractiveModeOptions.promptStashStore), [`promptStashStore`](../agents-view/agents-view-mode.ts.md#AgentsViewModeOptions.promptStashStore)  (4 test-only)

### `PromptStash`
- def: [`packages/coding-agent/src/modes/interactive/prompt-stash-state.ts:4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L4)
- signature: `interface PromptStash`
- members:
  - `expandedText` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L6)
  - `images` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L8)
  - `pasteSnapshot` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L7)
  - `text` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L5)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`EditorPasteSnapshot`](../../../../tui/src/editor-component.ts.md#EditorPasteSnapshot)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`setupEditorSubmitHandler`](interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`setCustomEditorComponent`](interactive-mode.ts.md#InteractiveMode.setCustomEditorComponent), [`retainStartupPromptDrafts`](interactive-mode.ts.md#InteractiveMode.retainStartupPromptDrafts), [`stash`](prompt-stash-state.ts.md#PromptStashState.stash), [`restorePromptStashIfEditorEmpty`](interactive-mode.ts.md#InteractiveMode.restorePromptStashIfEditorEmpty), [`liveImageMarkerIds`](interactive-mode.ts.md#InteractiveMode.liveImageMarkerIds), [`snapshotPromptStashFrom`](interactive-mode.ts.md#InteractiveMode.snapshotPromptStashFrom), [`hydratePromptStash`](interactive-mode.ts.md#InteractiveMode.hydratePromptStash), [`PromptStashState`](prompt-stash-state.ts.md#PromptStashState), [`<get>promptStash`](interactive-mode.ts.md#InteractiveMode.-get-promptStash), [`<set>promptStash`](interactive-mode.ts.md#InteractiveMode.-set-promptStash), [`retainSubmittedDraft`](interactive-mode.ts.md#InteractiveMode.retainSubmittedDraft), [`snapshotPromptStash`](interactive-mode.ts.md#InteractiveMode.snapshotPromptStash), [`latestEditorPromptStash`](interactive-mode.ts.md#InteractiveMode.latestEditorPromptStash), [`pendingSubmittedPromptStash`](interactive-mode.ts.md#InteractiveMode.pendingSubmittedPromptStash), [`retainedSubmissionGenerations`](interactive-mode.ts.md#InteractiveMode.retainedSubmissionGenerations)  (2 test-only)

### `PromptStashState`
- def: [`packages/coding-agent/src/modes/interactive/prompt-stash-state.ts:11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L11)
- signature: `interface PromptStashState`
- members:
  - `queuedStashes` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L13)
  - `stash` — [`L12`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/prompt-stash-state.ts#L12)
- uses (calls/refs, reference-scoped): [`PromptStash`](prompt-stash-state.ts.md#PromptStash)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-index.ts), [`resetCurrentSessionRenderState`](interactive-mode.ts.md#InteractiveMode.resetCurrentSessionRenderState), [`retainStartupPromptDrafts`](interactive-mode.ts.md#InteractiveMode.retainStartupPromptDrafts), [`restorePromptStashIfEditorEmpty`](interactive-mode.ts.md#InteractiveMode.restorePromptStashIfEditorEmpty), [`liveImageMarkerIds`](interactive-mode.ts.md#InteractiveMode.liveImageMarkerIds), [`forSession`](prompt-stash-state.ts.md#ClientPromptStashStore.forSession), [`hydratePromptStash`](interactive-mode.ts.md#InteractiveMode.hydratePromptStash), [`promptStashState`](interactive-mode.ts.md#InteractiveMode.promptStashState), [`<get>promptStash`](interactive-mode.ts.md#InteractiveMode.-get-promptStash), [`<set>promptStash`](interactive-mode.ts.md#InteractiveMode.-set-promptStash), [`retainSubmittedDraft`](interactive-mode.ts.md#InteractiveMode.retainSubmittedDraft), [`release`](prompt-stash-state.ts.md#ClientPromptStashStore.release), [`pendingPromptStashReleases`](interactive-mode.ts.md#InteractiveMode.pendingPromptStashReleases), [`states`](prompt-stash-state.ts.md#ClientPromptStashStore.states)  (6 test-only)

