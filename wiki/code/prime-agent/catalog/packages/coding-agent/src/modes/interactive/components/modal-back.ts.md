---
title: 'Module: packages/coding-agent/src/modes/interactive/components/modal-back.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/modal-back.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`modal-back.ts`/
symbols:
  shouldTreatAsBack: shouldTreatAsBack().
  BackGuardInput: BackGuardInput#
  BackGuardInput.getCursor: BackGuardInput#getCursor().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/modal-back.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/modal-back.ts)

## Classes
### `BackGuardInput`
- def: [`packages/coding-agent/src/modes/interactive/components/modal-back.ts:15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/modal-back.ts#L15)
- doc: A text input whose cursor position can be inspected.
- signature: `interface BackGuardInput`
- members:
  - `getCursor(method)` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/modal-back.ts#L16)
- used by: [`shouldTreatAsBack`](modal-back.ts.md#shouldTreatAsBack)

## Functions
- `shouldTreatAsBack(data: string, input?: BackGuardInput | undefined)` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/modal-back.ts#L26) — Returns true when `data` should dismiss the current dialog (act like Esc).

