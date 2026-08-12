---
title: 'Module: packages/coding-agent/src/modes/interactive/components/feature-hint.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/feature-hint.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`feature-hint.ts`/
symbols:
  FeatureHintComponent.render: FeatureHintComponent#render().
  renderLabelShimmer: renderLabelShimmer().
  FeatureHintComponent: FeatureHintComponent#
  FEATURE_HINT_ANIMATION_INTERVAL_MS: FEATURE_HINT_ANIMATION_INTERVAL_MS.
  FeatureHintComponent.advance: FeatureHintComponent#advance().
  SHIMMER_RADIUS: SHIMMER_RADIUS.
  LABEL: LABEL.
  FeatureHintComponent.frame: FeatureHintComponent#frame.
  SHIMMER_PAUSE_FRAMES: SHIMMER_PAUSE_FRAMES.
  FeatureHintComponent.-constructor: FeatureHintComponent#`<constructor>`().
  FeatureHintComponent.invalidate: FeatureHintComponent#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/feature-hint.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts)

## Classes
### `FeatureHintComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/feature-hint.ts:23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L23)
- signature: `class FeatureHintComponent`
- members:
  - `<constructor>(text: string)` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L26)
  - `advance(method)` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L28)
  - `invalidate(method)` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L32) — Invalidate any cached rendering state.
  - `render(method)` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L34) — Render the component to lines for the given viewport width
  - `frame` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L24)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`renderLabelShimmer`](feature-hint.ts.md#renderLabelShimmer), [`LABEL`](feature-hint.ts.md#LABEL)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`showFeatureHint`](../interactive-mode.ts.md#InteractiveMode.showFeatureHint), [`featureHintComponent`](../interactive-mode.ts.md#InteractiveMode.featureHintComponent)

## Functions
- `renderLabelShimmer(characters: string[], frame: number)` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L10)

## Module values
- `FEATURE_HINT_ANIMATION_INTERVAL_MS` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L8)
- `LABEL` — [`L4`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L4)
- `SHIMMER_PAUSE_FRAMES` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L6)
- `SHIMMER_RADIUS` — [`L5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/feature-hint.ts#L5)

