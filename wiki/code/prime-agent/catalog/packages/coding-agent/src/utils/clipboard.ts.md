---
title: 'Module: packages/coding-agent/src/utils/clipboard.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/clipboard.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`clipboard.ts`/
symbols:
  copyToClipboard: copyToClipboard().
  copyToX11Clipboard: copyToX11Clipboard().
  emitOsc52: emitOsc52().
  NativeClipboardExecOptions: NativeClipboardExecOptions#
  NativeClipboardExecOptions.typeLiteral0.input: NativeClipboardExecOptions#typeLiteral0:input.
  NativeClipboardExecOptions.typeLiteral0.timeout: NativeClipboardExecOptions#typeLiteral0:timeout.
  NativeClipboardExecOptions.typeLiteral0.stdio: NativeClipboardExecOptions#typeLiteral0:stdio.
  MAX_OSC52_ENCODED_LENGTH: MAX_OSC52_ENCODED_LENGTH.
  isRemoteSession: isRemoteSession().
---
# Module: [`packages/coding-agent/src/utils/clipboard.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts)

## Classes
### `NativeClipboardExecOptions`
- def: [`packages/coding-agent/src/utils/clipboard.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L6)
- signature: `type NativeClipboardExecOptions`
- members:
  - `input` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L7)
  - `stdio` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L9)
  - `timeout` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L8)
- used by: [`copyToClipboard`](clipboard.ts.md#copyToClipboard), [`copyToX11Clipboard`](clipboard.ts.md#copyToX11Clipboard)

## Functions
- `copyToClipboard(text: string)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L35)
- `copyToX11Clipboard(options: NativeClipboardExecOptions)` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L12)
- `emitOsc52(text: string)` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L26)
- `isRemoteSession(env?: ProcessEnv)` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L22)

## Module values
- `MAX_OSC52_ENCODED_LENGTH` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/clipboard.ts#L20)

