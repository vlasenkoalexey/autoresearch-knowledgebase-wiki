---
title: 'Module: packages/coding-agent/src/modes/interactive/feature-hints.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/feature-hints.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`feature-hints.ts`/F
symbols:
  FeatureHintDeck.next: eatureHintDeck#next().
  FEATURE_HINTS: EATURE_HINTS.
  FeatureHintDefinition.id: eatureHintDefinition#id.
  FeatureHintDefinition.getText: eatureHintDefinition#getText().
  FeatureHintDeck.refill: eatureHintDeck#refill().
  FeatureHintContext.getKeybinding: eatureHintContext#getKeybinding().
  FeatureHint.id: eatureHint#id.
  FeatureHint.text: eatureHint#text.
  FeatureHintDeck.remaining: eatureHintDeck#remaining.
  FeatureHintContext.isResidentSession: eatureHintContext#isResidentSession.
  FeatureHintDeck.-constructor: eatureHintDeck#`<constructor>`().
  FeatureHintDefinition: eatureHintDefinition#
  FeatureHintContext: eatureHintContext#
  FeatureHint: eatureHint#
  FeatureHintDeck: eatureHintDeck#
  FeatureHintDeck.previousId: eatureHintDeck#previousId.
---
# Module: [`packages/coding-agent/src/modes/interactive/feature-hints.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts)

## Classes
### `FeatureHint`
- def: [`packages/coding-agent/src/modes/interactive/feature-hints.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L13)
- signature: `interface FeatureHint`
- members:
  - `id` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L14)
  - `text` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L15)
- used by: [`showFeatureHint`](interactive-mode.ts.md#InteractiveMode.showFeatureHint), [`next`](feature-hints.ts.md#FeatureHintDeck.next), [`remaining`](feature-hints.ts.md#FeatureHintDeck.remaining)  (1 test-only)

### `FeatureHintContext`
- def: [`packages/coding-agent/src/modes/interactive/feature-hints.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L3)
- signature: `interface FeatureHintContext`
- members:
  - `getKeybinding(method)` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L4)
  - `isResidentSession` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L5)
- uses (calls/refs, reference-scoped): [`AppKeybinding`](../../core/keybindings.ts.md#AppKeybinding)
- used by: [`showFeatureHint`](interactive-mode.ts.md#InteractiveMode.showFeatureHint), [`next`](feature-hints.ts.md#FeatureHintDeck.next), [`FEATURE_HINTS`](feature-hints.ts.md#FEATURE_HINTS), [`refill`](feature-hints.ts.md#FeatureHintDeck.refill), [`FeatureHintDefinition`](feature-hints.ts.md#FeatureHintDefinition)  (1 test-only)

### `FeatureHintDeck`
- def: [`packages/coding-agent/src/modes/interactive/feature-hints.ts:104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L104)
- signature: `class FeatureHintDeck`
- members:
  - `<constructor>(random?: () => number)` — [`L108`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L108)
  - `next(method)` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L110)
  - `refill(method)` — [`L121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L121)
  - `previousId` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L106)
  - `remaining` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L105)
- uses (calls/refs, reference-scoped): [`FEATURE_HINTS`](feature-hints.ts.md#FEATURE_HINTS), [`getText`](feature-hints.ts.md#FeatureHintDefinition.getText), [`id`](feature-hints.ts.md#FeatureHintDefinition.id), [`id`](feature-hints.ts.md#FeatureHint.id), [`FeatureHintContext`](feature-hints.ts.md#FeatureHintContext), [`FeatureHint`](feature-hints.ts.md#FeatureHint)
- used by: [`interactive-mode.ts`](interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`showFeatureHint`](interactive-mode.ts.md#InteractiveMode.showFeatureHint), [`featureHintDeck`](interactive-mode.ts.md#InteractiveMode.featureHintDeck)  (1 test-only)

### `FeatureHintDefinition`
- def: [`packages/coding-agent/src/modes/interactive/feature-hints.ts:8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L8)
- signature: `interface FeatureHintDefinition`
- members:
  - `getText(method)` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L10)
  - `id` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L9)
- uses (calls/refs, reference-scoped): [`FeatureHintContext`](feature-hints.ts.md#FeatureHintContext)
- used by: [`FEATURE_HINTS`](feature-hints.ts.md#FEATURE_HINTS), [`refill`](feature-hints.ts.md#FeatureHintDeck.refill)  (1 test-only)

## Module values
- `FEATURE_HINTS` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/feature-hints.ts#L18)

