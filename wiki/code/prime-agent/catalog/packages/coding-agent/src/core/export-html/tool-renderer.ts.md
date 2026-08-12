---
title: 'Module: packages/coding-agent/src/core/export-html/tool-renderer.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/export-html/tool-renderer.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/export-html/`tool-renderer.ts`/
symbols:
  createToolHtmlRenderer: createToolHtmlRenderer().
  ToolHtmlRendererDeps.getToolDefinition: ToolHtmlRendererDeps#getToolDefinition.
  ToolHtmlRendererDeps.theme: ToolHtmlRendererDeps#theme.
  isBlankRenderedLine: isBlankRenderedLine().
  trimRenderedResultLines: trimRenderedResultLines().
  ToolHtmlRendererDeps.cwd: ToolHtmlRendererDeps#cwd.
  ToolHtmlRenderer.renderResult: ToolHtmlRenderer#renderResult().
  ToolHtmlRendererDeps: ToolHtmlRendererDeps#
  ToolHtmlRendererDeps.width: ToolHtmlRendererDeps#width.
  ToolHtmlRenderer: ToolHtmlRenderer#
  ToolHtmlRenderer.renderCall: ToolHtmlRenderer#renderCall().
  ANSI_ESCAPE_REGEX: ANSI_ESCAPE_REGEX.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral2.type: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral2:type.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral2.text: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral2:text.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral2.data: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral2:data.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral2.mimeType: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral2:mimeType.
---
# Module: [`packages/coding-agent/src/core/export-html/tool-renderer.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts)

## Classes
### `ToolHtmlRenderer`
- def: [`packages/coding-agent/src/core/export-html/tool-renderer.ts:25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L25)
- signature: `interface ToolHtmlRenderer`
- members:
  - `renderCall(method)` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L27) — Render a tool call to HTML. Returns undefined if tool has no custom renderer.
  - `renderResult(method)` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L29) — Render a tool result to collapsed/expanded HTML. Returns undefined if tool has no custom renderer.
  - `data` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L32)
  - `mimeType` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L32)
  - `text` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L32)
  - `type` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L32)
- used by: [`createToolHtmlRenderer`](tool-renderer.ts.md#createToolHtmlRenderer)  (1 test-only)

### `ToolHtmlRendererDeps`
- def: [`packages/coding-agent/src/core/export-html/tool-renderer.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L14)
- signature: `interface ToolHtmlRendererDeps`
- members:
  - `cwd` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L20) — Working directory for render context
  - `getToolDefinition` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L16) — Function to look up tool definition by name
  - `theme` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L18) — Theme for styling
  - `width` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L22) — Terminal width for rendering (default: 100)
- uses (calls/refs, reference-scoped): [`Theme`](../../modes/interactive/theme/theme.ts.md#Theme), [`ToolDefinition`](../extensions/types.ts.md#ToolDefinition)
- used by: [`createToolHtmlRenderer`](tool-renderer.ts.md#createToolHtmlRenderer), [`exportToHtml`](../agent-session.ts.md#AgentSession.exportToHtml)  (1 test-only)

## Functions
- `createToolHtmlRenderer(deps: ToolHtmlRendererDeps)` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L58)
- `isBlankRenderedLine(line: string)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L46)
- `trimRenderedResultLines(lines: string[])` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L50)

## Module values
- `ANSI_ESCAPE_REGEX` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/tool-renderer.ts#L44) — Create a tool HTML renderer.

