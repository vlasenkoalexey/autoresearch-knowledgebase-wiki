---
title: 'Module: packages/coding-agent/src/core/tools/render-utils.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/render-utils.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`render-utils.ts`/
symbols:
  getTextOutput: getTextOutput().
  invalidArgText: invalidArgText().
  str: str().
  ToolRenderResultLike.typeLiteral49.content: ToolRenderResultLike#typeLiteral49:content.
  shortenPath: shortenPath().
  TextOutputOptions: TextOutputOptions#
  TextOutputOptions.includeImageDimensions: TextOutputOptions#includeImageDimensions.
  invalidArgText.theme-typeLiteral50.fg: invalidArgText().(theme)typeLiteral50:fg.
  replaceTabs: replaceTabs().
  normalizeDisplayText: normalizeDisplayText().
  ToolRenderResultLike: ToolRenderResultLike#
  ToolRenderResultLike.typeLiteral49.details: ToolRenderResultLike#typeLiteral49:details.
---
# Module: [`packages/coding-agent/src/core/tools/render-utils.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts)

## Classes
### `TextOutputOptions`
- def: [`packages/coding-agent/src/core/tools/render-utils.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L30)
- signature: `interface TextOutputOptions`
- members:
  - `includeImageDimensions` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L32) — Whether image fallbacks should parse image dimensions from base64 data.
- used by: [`getTextOutput`](render-utils.ts.md#getTextOutput)

### `ToolRenderResultLike`
- def: [`packages/coding-agent/src/core/tools/render-utils.ts:65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L65)
- signature: `type ToolRenderResultLike`
- members:
  - `content` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L66)
  - `details` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L67)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../../ai/src/types.ts.md#TextContent)

## Functions
- `getTextOutput(result: { content: { type: string; text?: string | undefined; data?: string | undefined; mimeType?: string | undefined; }[]; } | undefined, showImages: boolean, options?: TextOutputOptions)` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L35)
- `invalidArgText(theme: { fg: (name: any, text: string) => string; })` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L70)
- `normalizeDisplayText(text: string)` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L26)
- `replaceTabs(text: string)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L22)
- `shortenPath(path: unknown)` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L7)
- `str(value: unknown)` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L16)

## Module values
- `fg` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/render-utils.ts#L70)

