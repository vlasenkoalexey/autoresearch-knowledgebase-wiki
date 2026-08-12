---
title: 'Module: packages/coding-agent/src/utils/clipboard-image.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/clipboard-image.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`clipboard-image.ts`/
symbols:
  readClipboardImage: readClipboardImage().
  runCommand.typeLiteral42.ok: runCommand().typeLiteral42:ok.
  readClipboardImageViaXclip: readClipboardImageViaXclip().
  readClipboardImageViaWlPaste: readClipboardImageViaWlPaste().
  readClipboardImageViaPowerShell: readClipboardImageViaPowerShell().
  readClipboardImageViaNativeClipboard: readClipboardImageViaNativeClipboard().
  runCommand.typeLiteral42.stdout: runCommand().typeLiteral42:stdout.
  ClipboardImage.typeLiteral0.bytes: ClipboardImage#typeLiteral0:bytes.
  ClipboardImage.typeLiteral0.mimeType: ClipboardImage#typeLiteral0:mimeType.
  selectPreferredImageMimeType: selectPreferredImageMimeType().
  ClipboardImage: ClipboardImage#
  isSupportedImageMimeType: isSupportedImageMimeType().
  runCommand: runCommand().
  baseMimeType: baseMimeType().
  SUPPORTED_IMAGE_MIME_TYPES: SUPPORTED_IMAGE_MIME_TYPES.
  convertToPng: convertToPng().
  DEFAULT_LIST_TIMEOUT_MS: DEFAULT_LIST_TIMEOUT_MS.
  isWaylandSession: isWaylandSession().
  extensionForImageMimeType: extensionForImageMimeType().
  DEFAULT_READ_TIMEOUT_MS: DEFAULT_READ_TIMEOUT_MS.
  DEFAULT_POWERSHELL_TIMEOUT_MS: DEFAULT_POWERSHELL_TIMEOUT_MS.
  DEFAULT_MAX_BUFFER_BYTES: DEFAULT_MAX_BUFFER_BYTES.
  runCommand.options-typeLiteral41.timeoutMs: runCommand().(options)typeLiteral41:timeoutMs.
  runCommand.options-typeLiteral41.maxBufferBytes: runCommand().(options)typeLiteral41:maxBufferBytes.
  runCommand.options-typeLiteral41.env: runCommand().(options)typeLiteral41:env.
  isWSL: isWSL().
  readClipboardImage.options-typeLiteral130.env: readClipboardImage().(options)typeLiteral130:env.
  readClipboardImage.options-typeLiteral130.platform: readClipboardImage().(options)typeLiteral130:platform.
---
# Module: [`packages/coding-agent/src/utils/clipboard-image.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts)

## Classes
### `ClipboardImage`
- def: [`packages/coding-agent/src/utils/clipboard-image.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L10)
- signature: `type ClipboardImage`
- members:
  - `bytes` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L11)
  - `mimeType` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L12)
- used by: [`handleClipboardImagePaste`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleClipboardImagePaste), [`readClipboardImage`](clipboard-image.ts.md#readClipboardImage), [`readClipboardImageViaXclip`](clipboard-image.ts.md#readClipboardImageViaXclip), [`readClipboardImageViaWlPaste`](clipboard-image.ts.md#readClipboardImageViaWlPaste), [`readClipboardImageViaPowerShell`](clipboard-image.ts.md#readClipboardImageViaPowerShell), [`readClipboardImageViaNativeClipboard`](clipboard-image.ts.md#readClipboardImageViaNativeClipboard)  (2 test-only)

## Functions
- `baseMimeType(mimeType: string)` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L26)
- `convertToPng(bytes: Uint8Array<ArrayBufferLike>)` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L71) — Convert unsupported image formats to PNG using Photon.
- `extensionForImageMimeType(mimeType: string)` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L30)
- `isSupportedImageMimeType(mimeType: string)` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L62)
- `isWSL(env?: ProcessEnv)` — [`L143`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L143)
- `isWaylandSession(env?: ProcessEnv)` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L22)
- `readClipboardImage(options?: { env?: ProcessEnv | undefined; platform?: Platform | undefined; } | undefined)` — [`L254`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L254)
- `readClipboardImageViaNativeClipboard()` — [`L240`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L240)
- `readClipboardImageViaPowerShell()` — [`L161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L161) — On WSL, the Linux clipboard (Wayland/X11) does not receive image data from
- `readClipboardImageViaWlPaste()` — [`L118`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L118)
- `readClipboardImageViaXclip()` — [`L213`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L213)
- `runCommand(command: string, args: string[], options?: { timeoutMs?: number | undefined; maxBufferBytes?: number | undefined; env?: ProcessEnv | undefined; } | undefined)` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L89)
- `selectPreferredImageMimeType(mimeTypes: string[])` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L45)

## Module values
- `DEFAULT_LIST_TIMEOUT_MS` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L17)
- `DEFAULT_MAX_BUFFER_BYTES` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L20)
- `DEFAULT_POWERSHELL_TIMEOUT_MS` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L19)
- `DEFAULT_READ_TIMEOUT_MS` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L18)
- `SUPPORTED_IMAGE_MIME_TYPES` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L15)
- `env` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L92)
- `env` — [`L255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L255)
- `maxBufferBytes` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L92)
- `ok` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L93)
- `platform` — [`L256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L256)
- `stdout` — [`L93`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L93)
- `timeoutMs` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard-image.ts#L92)

