---
title: 'Module: packages/coding-agent/src/core/tools/edit.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/edit.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`edit.ts`/
symbols:
  createEditToolDefinition: createEditToolDefinition().
  formatEditResult: formatEditResult().
  buildEditCallComponent: buildEditCallComponent().
  createEditTool: createEditTool().
  formatEditCall: formatEditCall().
  getRenderablePreviewInput: getRenderablePreviewInput().
  setEditPreview: setEditPreview().
  EditToolInput: EditToolInput#
  getEditCallRenderComponent: getEditCallRenderComponent().
  EditToolDetails: EditToolDetails#
  EditCallRenderComponent: EditCallRenderComponent#
  defaultEditOperations: defaultEditOperations.
  validateEditInput: validateEditInput().
  getEditHeaderBg: getEditHeaderBg().
  EditPreview: EditPreview#
  createEditCallRenderComponent: createEditCallRenderComponent().
  editSchema: editSchema.
  RenderableEditArgs: RenderableEditArgs#
  EditToolOptions: EditToolOptions#
  RenderableEditArgs.typeLiteral48.edits: RenderableEditArgs#typeLiteral48:edits.
  EditOperations: EditOperations#
  prepareEditArguments: prepareEditArguments().
  EditRenderState: EditRenderState#
  EditRenderState.typeLiteral0.callComponent: EditRenderState#typeLiteral0:callComponent.
  EditToolDetails.diff: EditToolDetails#diff.
  EditToolResultLike: EditToolResultLike#
  RenderableEditArgs.typeLiteral48.path: RenderableEditArgs#typeLiteral48:path.
  RenderableEditArgs.typeLiteral48.file_path: RenderableEditArgs#typeLiteral48:file_path.
  LegacyEditToolInput: LegacyEditToolInput#
  EditOperations.readFile: EditOperations#readFile.
  EditOperations.writeFile: EditOperations#writeFile.
  EditOperations.access: EditOperations#access.
  EditToolResultLike.typeLiteral49.details: EditToolResultLike#typeLiteral49:details.
  validateEditInput.typeLiteral47.path: validateEditInput().typeLiteral47:path.
  validateEditInput.typeLiteral47.edits: validateEditInput().typeLiteral47:edits.
  RenderableEditArgs.typeLiteral48.oldText: RenderableEditArgs#typeLiteral48:oldText.
  RenderableEditArgs.typeLiteral48.newText: RenderableEditArgs#typeLiteral48:newText.
  replaceEditSchema: replaceEditSchema.
  EditToolDetails.firstChangedLine: EditToolDetails#firstChangedLine.
  EditToolOptions.operations: EditToolOptions#operations.
  EditToolResultLike.typeLiteral49.content: EditToolResultLike#typeLiteral49:content.
  EditToolResultLike.typeLiteral49.content.Array.typeLiteral50.type: EditToolResultLike#typeLiteral49:content.Array:typeLiteral50:type.
  EditToolResultLike.typeLiteral49.content.Array.typeLiteral50.text: EditToolResultLike#typeLiteral49:content.Array:typeLiteral50:text.
  EditToolResultLike.typeLiteral49.content.Array.typeLiteral50.data: EditToolResultLike#typeLiteral49:content.Array:typeLiteral50:data.
  EditToolResultLike.typeLiteral49.content.Array.typeLiteral50.mimeType: EditToolResultLike#typeLiteral49:content.Array:typeLiteral50:mimeType.
---
# Module: [`packages/coding-agent/src/core/tools/edit.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts)

## Classes
### `EditCallRenderComponent`
- def: [`packages/coding-agent/src/core/tools/edit.ts:139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L139)
- signature: `type EditCallRenderComponent`
- uses (calls/refs, reference-scoped): [`Box`](../../../../tui/src/components/box.ts.md#Box), [`EditPreview`](edit.ts.md#EditPreview)
- used by: [`buildEditCallComponent`](edit.ts.md#buildEditCallComponent), [`setEditPreview`](edit.ts.md#setEditPreview), [`getEditCallRenderComponent`](edit.ts.md#getEditCallRenderComponent), [`createEditCallRenderComponent`](edit.ts.md#createEditCallRenderComponent), [`EditRenderState`](edit.ts.md#EditRenderState)

### `EditOperations`
- def: [`packages/coding-agent/src/core/tools/edit.ts:71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L71)
- doc: Pluggable operations for the edit tool.
- signature: `interface EditOperations`
- members:
  - `access` — [`L77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L77) — Check if file is readable and writable (throw if not)
  - `readFile` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L73) — Read file contents as a Buffer
  - `writeFile` — [`L75`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L75) — Write content to a file
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`defaultEditOperations`](edit.ts.md#defaultEditOperations), [`EditToolOptions`](edit.ts.md#EditToolOptions)  (2 test-only)

### `EditPreview`
- def: [`packages/coding-agent/src/core/tools/edit.ts:26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L26)
- signature: `type EditPreview`
- uses (calls/refs, reference-scoped): [`EditDiffError`](edit-diff.ts.md#EditDiffError), [`EditDiffResult`](edit-diff.ts.md#EditDiffResult)
- used by: [`formatEditResult`](edit.ts.md#formatEditResult), [`setEditPreview`](edit.ts.md#setEditPreview), [`EditCallRenderComponent`](edit.ts.md#EditCallRenderComponent), [`getEditHeaderBg`](edit.ts.md#getEditHeaderBg), [`createEditCallRenderComponent`](edit.ts.md#createEditCallRenderComponent)

### `EditRenderState`
- def: [`packages/coding-agent/src/core/tools/edit.ts:28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L28)
- signature: `type EditRenderState`
- members:
  - `callComponent` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L29)
- uses (calls/refs, reference-scoped): [`EditCallRenderComponent`](edit.ts.md#EditCallRenderComponent)
- used by: [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`getEditCallRenderComponent`](edit.ts.md#getEditCallRenderComponent)

### `EditToolDetails`
- def: [`packages/coding-agent/src/core/tools/edit.ts:60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L60)
- signature: `interface EditToolDetails`
- members:
  - `diff` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L62) — Unified diff of the changes made
  - `firstChangedLine` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L64) — Line number of the first change in the new file (for editor navigation)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`edit-summary.ts`](../../modes/interactive/components/edit-summary.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-edit-summary.ts), [`isError`](../../modes/interactive/components/edit-summary.ts.md#getToolFileChanges.result-typeLiteral16.isError), [`formatEditResult`](edit.ts.md#formatEditResult), [`EditToolResultEvent`](../extensions/types.ts.md#EditToolResultEvent), [`EditToolResultLike`](edit.ts.md#EditToolResultLike)  (1 test-only)

### `EditToolInput`
- def: [`packages/coding-agent/src/core/tools/edit.ts:54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L54)
- signature: `type EditToolInput`
- uses (calls/refs, reference-scoped): [`editSchema`](edit.ts.md#editSchema)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`validateEditInput`](edit.ts.md#validateEditInput), [`EditToolCallEvent`](../extensions/types.ts.md#EditToolCallEvent), [`prepareEditArguments`](edit.ts.md#prepareEditArguments), [`LegacyEditToolInput`](edit.ts.md#LegacyEditToolInput)

### `EditToolOptions`
- def: [`packages/coding-agent/src/core/tools/edit.ts:86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L86)
- signature: `interface EditToolOptions`
- members:
  - `operations` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L88) — Custom operations for file editing. Default: local filesystem
- uses (calls/refs, reference-scoped): [`EditOperations`](edit.ts.md#EditOperations)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`createEditTool`](edit.ts.md#createEditTool)

### `EditToolResultLike`
- def: [`packages/coding-agent/src/core/tools/edit.ts:134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L134)
- signature: `type EditToolResultLike`
- members:
  - `content` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L135)
  - `data` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L135)
  - `details` — [`L136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L136)
  - `mimeType` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L135)
  - `text` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L135)
  - `type` — [`L135`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L135)
- uses (calls/refs, reference-scoped): [`EditToolDetails`](edit.ts.md#EditToolDetails)
- used by: [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`formatEditResult`](edit.ts.md#formatEditResult)

### `LegacyEditToolInput`
- def: [`packages/coding-agent/src/core/tools/edit.ts:55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L55)
- signature: `type LegacyEditToolInput`
- uses (calls/refs, reference-scoped): [`EditToolInput`](edit.ts.md#EditToolInput)
- used by: [`prepareEditArguments`](edit.ts.md#prepareEditArguments)

### `RenderableEditArgs`
- def: [`packages/coding-agent/src/core/tools/edit.ts:126`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L126)
- signature: `type RenderableEditArgs`
- members:
  - `edits` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L129)
  - `file_path` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L128)
  - `newText` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L131)
  - `oldText` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L130)
  - `path` — [`L127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L127)
- uses (calls/refs, reference-scoped): [`Edit`](edit-diff.ts.md#Edit)
- used by: [`createEditToolDefinition`](edit.ts.md#createEditToolDefinition), [`formatEditResult`](edit.ts.md#formatEditResult), [`buildEditCallComponent`](edit.ts.md#buildEditCallComponent), [`formatEditCall`](edit.ts.md#formatEditCall), [`getRenderablePreviewInput`](edit.ts.md#getRenderablePreviewInput)

## Functions
- `buildEditCallComponent(component: EditCallRenderComponent, args: RenderableEditArgs | undefined, theme: Theme, expanded: boolean, showExpandHint: boolean)` — [`L251`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L251)
- `createEditCallRenderComponent()` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L146)
- `createEditTool(cwd: string, options?: EditToolOptions | undefined)` — [`L499`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L499)
- `createEditToolDefinition(cwd: string, options?: EditToolOptions | undefined)` — [`L299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L299)
- `formatEditCall(args: RenderableEditArgs | undefined, theme: Theme)` — [`L194`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L194)
- `formatEditResult(args: RenderableEditArgs | undefined, preview: EditPreview | undefined, result: EditToolResultLike, theme: Theme, isError: boolean)` — [`L205`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L205)
- `getEditCallRenderComponent(state: EditRenderState, lastComponent: unknown)` — [`L155`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L155)
- `getEditHeaderBg(preview: EditPreview | undefined, settledError: boolean | undefined, theme: Theme)` — [`L234`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L234)
- `getRenderablePreviewInput(args: RenderableEditArgs | undefined)` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L169)
- `prepareEditArguments(input: unknown)` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L91)
- `setEditPreview(component: EditCallRenderComponent, preview: EditPreview, argsKey: string | undefined)` — [`L279`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L279)
- `validateEditInput(input: { path: string; edits: { oldText: string; newText: string; }[]; })` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L119)

## Module values
- `defaultEditOperations` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L80)
- `editSchema` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L43)
- `edits` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L119)
- `path` — [`L119`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L119)
- `replaceEditSchema` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/edit.ts#L32)

