---
title: 'Module: packages/ai/src/providers/transform-messages.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/transform-messages.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`transform-messages.ts`/
symbols:
  transformMessages: transformMessages().
  downgradeUnsupportedImages: downgradeUnsupportedImages().
  replaceImagesWithPlaceholder: replaceImagesWithPlaceholder().
  NON_VISION_USER_IMAGE_PLACEHOLDER: NON_VISION_USER_IMAGE_PLACEHOLDER.
  NON_VISION_TOOL_IMAGE_PLACEHOLDER: NON_VISION_TOOL_IMAGE_PLACEHOLDER.
---
# Module: [`packages/ai/src/providers/transform-messages.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts)

## Functions
- `downgradeUnsupportedImages(messages: Message[], model: Model<TApi>)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts#L35)
- `replaceImagesWithPlaceholder(content: (TextContent | ImageContent)[], placeholder: string)` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts#L15)
- `transformMessages(messages: Message[], model: Model<TApi>, normalizeToolCallId?: ((id: string, model: Model<TApi>, source: AssistantMessage) => string) | undefined)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts#L64) — Normalize tool call ID for cross-provider compatibility.

## Module values
- `NON_VISION_TOOL_IMAGE_PLACEHOLDER` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts#L13)
- `NON_VISION_USER_IMAGE_PLACEHOLDER` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/transform-messages.ts#L12)

