---
title: 'Module: packages/coding-agent/src/cli/initial-message.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/initial-message.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`initial-message.ts`/
symbols:
  buildInitialMessage: buildInitialMessage().
  InitialMessageInput.parsed: InitialMessageInput#parsed.
  InitialMessageInput.stdinContent: InitialMessageInput#stdinContent.
  InitialMessageInput.fileImages: InitialMessageInput#fileImages.
  InitialMessageResult.initialMessage: InitialMessageResult#initialMessage.
  InitialMessageResult: InitialMessageResult#
  InitialMessageInput.fileText: InitialMessageInput#fileText.
  InitialMessageInput: InitialMessageInput#
  InitialMessageResult.initialImages: InitialMessageResult#initialImages.
---
# Module: [`packages/coding-agent/src/cli/initial-message.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts)

## Classes
### `InitialMessageInput`
- def: [`packages/coding-agent/src/cli/initial-message.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L4)
- signature: `interface InitialMessageInput`
- members:
  - `fileImages` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L7)
  - `fileText` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L6)
  - `parsed` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L5)
  - `stdinContent` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L8)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`Args`](args.ts.md#Args)
- used by: [`buildInitialMessage`](initial-message.ts.md#buildInitialMessage), [`initialImages`](../main.ts.md#prepareInitialMessage.Promise.typeLiteral38.initialImages)  (1 test-only)

### `InitialMessageResult`
- def: [`packages/coding-agent/src/cli/initial-message.ts:11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L11)
- signature: `interface InitialMessageResult`
- members:
  - `initialImages` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L13)
  - `initialMessage` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L12)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent)
- used by: [`buildInitialMessage`](initial-message.ts.md#buildInitialMessage)  (1 test-only)

## Functions
- `buildInitialMessage({ parsed, fileText, fileImages, stdinContent, }: InitialMessageInput)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/initial-message.ts#L20) — Combine stdin content,

