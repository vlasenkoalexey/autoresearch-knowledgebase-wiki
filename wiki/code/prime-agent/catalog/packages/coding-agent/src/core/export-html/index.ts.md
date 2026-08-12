---
title: 'Module: packages/coding-agent/src/core/export-html/index.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/export-html/index.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/export-html/`index.ts`/
symbols:
  preRenderCustomTools: preRenderCustomTools().
  exportSessionToHtml: exportSessionToHtml().
  exportFromFile: exportFromFile().
  generateHtml: generateHtml().
  generateThemeVars: generateThemeVars().
  deriveExportColors: deriveExportColors().
  SessionData.header: SessionData#header.
  SessionData.entries: SessionData#entries.
  adjustBrightness: adjustBrightness().
  deriveExportColors.typeLiteral32.pageBg: deriveExportColors().typeLiteral32:pageBg.
  deriveExportColors.typeLiteral32.cardBg: deriveExportColors().typeLiteral32:cardBg.
  deriveExportColors.typeLiteral32.infoBg: deriveExportColors().typeLiteral32:infoBg.
  ExportOptions.toolRenderer: ExportOptions#toolRenderer.
  SessionData.tools: SessionData#tools.
  ToolHtmlRenderer: ToolHtmlRenderer#
  RenderedToolHtml: RenderedToolHtml#
  ExportOptions: ExportOptions#
  ExportOptions.outputPath: ExportOptions#outputPath.
  SessionData.renderedTools: SessionData#renderedTools.
  SessionData: SessionData#
  ExportOptions.themeName: ExportOptions#themeName.
  parseColor: parseColor().
  SessionData.leafId: SessionData#leafId.
  SessionData.systemPrompt: SessionData#systemPrompt.
  TEMPLATE_RENDERED_TOOLS: TEMPLATE_RENDERED_TOOLS.
  ToolHtmlRenderer.renderCall: ToolHtmlRenderer#renderCall().
  ToolHtmlRenderer.renderResult: ToolHtmlRenderer#renderResult().
  RenderedToolHtml.callHtml: RenderedToolHtml#callHtml.
  RenderedToolHtml.resultHtmlCollapsed: RenderedToolHtml#resultHtmlCollapsed.
  RenderedToolHtml.resultHtmlExpanded: RenderedToolHtml#resultHtmlExpanded.
  getLuminance: getLuminance().
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral0.type: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral0:type.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral0.text: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral0:text.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral0.data: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral0:data.
  ToolHtmlRenderer.renderResult.result-Array.typeLiteral0.mimeType: ToolHtmlRenderer#renderResult().(result)Array:typeLiteral0:mimeType.
---
# Module: [`packages/coding-agent/src/core/export-html/index.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts)

## Classes
### `ExportOptions`
- def: [`packages/coding-agent/src/core/export-html/index.ts:34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L34)
- signature: `interface ExportOptions`
- members:
  - `outputPath` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L35)
  - `themeName` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L36)
  - `toolRenderer` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L38) — Optional tool renderer for custom tools
- uses (calls/refs, reference-scoped): [`ToolHtmlRenderer`](index.ts.md#ToolHtmlRenderer)
- used by: [`exportSessionToHtml`](index.ts.md#exportSessionToHtml), [`exportFromFile`](index.ts.md#exportFromFile)

### `RenderedToolHtml`
- def: [`packages/coding-agent/src/core/export-html/index.ts:28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L28)
- doc: Pre-rendered HTML for a custom tool call and result
- signature: `interface RenderedToolHtml`
- members:
  - `callHtml` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L29)
  - `resultHtmlCollapsed` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L30)
  - `resultHtmlExpanded` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L31)
- used by: [`preRenderCustomTools`](index.ts.md#preRenderCustomTools), [`exportSessionToHtml`](index.ts.md#exportSessionToHtml), [`renderedTools`](index.ts.md#SessionData.renderedTools)

### `SessionData`
- def: [`packages/coding-agent/src/core/export-html/index.ts:129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L129)
- signature: `interface SessionData`
- members:
  - `entries` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L131)
  - `header` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L130)
  - `leafId` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L132)
  - `renderedTools` — [`L136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L136) — Pre-rendered HTML for custom tool calls/results, keyed by tool call ID
  - `systemPrompt` — [`L133`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L133)
  - `tools` — [`L134`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L134)
- uses (calls/refs, reference-scoped): [`SessionManager`](../session-manager.ts.md#SessionManager), [`getEntries`](../session-manager.ts.md#SessionManager.getEntries), [`getHeader`](../session-manager.ts.md#SessionManager.getHeader), [`ToolDefinition`](../extensions/types.ts.md#ToolDefinition), [`RenderedToolHtml`](index.ts.md#RenderedToolHtml)
- used by: [`exportSessionToHtml`](index.ts.md#exportSessionToHtml), [`exportFromFile`](index.ts.md#exportFromFile), [`generateHtml`](index.ts.md#generateHtml)

### `ToolHtmlRenderer`
- def: [`packages/coding-agent/src/core/export-html/index.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L14)
- doc: Interface for rendering custom tools to HTML.
- signature: `interface ToolHtmlRenderer`
- members:
  - `renderCall(method)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L16) — Render a tool call to HTML. Returns undefined if tool has no custom renderer.
  - `renderResult(method)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L18) — Render a tool result to HTML. Returns collapsed/expanded or undefined if tool has no custom renderer.
  - `data` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L21)
  - `mimeType` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L21)
  - `text` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L21)
  - `type` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L21)
- used by: [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`preRenderCustomTools`](index.ts.md#preRenderCustomTools), [`exportToHtml`](../agent-session.ts.md#AgentSession.exportToHtml), [`toolRenderer`](index.ts.md#ExportOptions.toolRenderer)

## Functions
- `adjustBrightness(color: string, factor: number)` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L72) — Adjust color brightness. Factor > 1 lightens, < 1 darkens.
- `deriveExportColors(baseColor: string)` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L80) — Derive export background colors from a base color (e.g., userMessageBg).
- `exportFromFile(inputPath: string, options?: string | ExportOptions | undefined)` — [`L287`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L287) — Export session file to HTML (standalone, without AgentState).
- `exportSessionToHtml(sm: SessionManager, state?: AgentState | undefined, options?: string | ExportOptions | undefined)` — [`L235`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L235) — Export session to HTML using SessionManager and AgentState.
- `generateHtml(sessionData: SessionData, themeName?: string | undefined)` — [`L142`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L142) — Core HTML generation logic shared by both export functions.
- `generateThemeVars(themeName?: string | undefined)` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L110) — Generate CSS custom property declarations from theme colors.
- `getLuminance(r: number, g: number, b: number)` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L63) — Calculate relative luminance of a color (0-1, higher = lighter).
- `parseColor(color: string)` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L42) — Parse a color string to RGB values. Supports hex (#RRGGBB) and rgb(r,g,b) formats.
- `preRenderCustomTools(entries: SessionEntry[], toolRenderer: ToolHtmlRenderer)` — [`L182`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L182) — Pre-render custom tools to HTML using their TUI renderers.

## Module values
- `TEMPLATE_RENDERED_TOOLS` — [`L177`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L177) — Tools rendered directly by the HTML template (not pre-rendered via TUI→ANSI→HTML pipeline)
- `cardBg` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L80)
- `infoBg` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L80)
- `pageBg` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/export-html/index.ts#L80)

