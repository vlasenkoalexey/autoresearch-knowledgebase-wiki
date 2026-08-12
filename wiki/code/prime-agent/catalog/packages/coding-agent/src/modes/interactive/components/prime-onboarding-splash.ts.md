---
title: 'Module: packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`prime-onboarding-splash.ts`/
symbols:
  PrimeOnboardingSplashComponent.drawLabField: PrimeOnboardingSplashComponent#drawLabField().
  PrimeOnboardingSplashComponent.render: PrimeOnboardingSplashComponent#render().
  PrimeOnboardingSplashComponent.renderCells: PrimeOnboardingSplashComponent#renderCells().
  PrimeOnboardingSplashComponent.drawStyledText: PrimeOnboardingSplashComponent#drawStyledText().
  PrimeOnboardingSplashComponent.-constructor: PrimeOnboardingSplashComponent#`<constructor>`().
  PrimeOnboardingSplashComponent.put: PrimeOnboardingSplashComponent#put().
  PrimeOnboardingSplashComponent.renderPanel: PrimeOnboardingSplashComponent#renderPanel().
  PrimeOnboardingSplashComponent.formatContinueHint: PrimeOnboardingSplashComponent#formatContinueHint().
  PrimeOnboardingSplashComponent.renderBackdrop: PrimeOnboardingSplashComponent#renderBackdrop().
  PrimeOnboardingSplashComponent.labCell: PrimeOnboardingSplashComponent#labCell().
  PrimeOnboardingSplashComponent.centerParts: PrimeOnboardingSplashComponent#centerParts().
  PrimeOnboardingSplashComponent.formatBrandLine: PrimeOnboardingSplashComponent#formatBrandLine().
  PrimeOnboardingSplashComponent.renderLogoBlock: PrimeOnboardingSplashComponent#renderLogoBlock().
  PrimeOnboardingSplashComponent.isInsideQuietZone: PrimeOnboardingSplashComponent#isInsideQuietZone().
  StyledText.tone: StyledText#tone.
  PrimeOnboardingSplashComponent.handleInput: PrimeOnboardingSplashComponent#handleInput().
  PanelTextLine: PanelTextLine#
  PrimeOnboardingSplashComponent.showProgress: PrimeOnboardingSplashComponent#showProgress().
  StyledText.text: StyledText#text.
  SplashCell.tone: SplashCell#tone.
  PrimeOnboardingSplashComponent.visiblePartsWidth: PrimeOnboardingSplashComponent#visiblePartsWidth().
  PrimeOnboardingSplashComponent.logoQuietZone: PrimeOnboardingSplashComponent#logoQuietZone().
  LOGO_WIDTH: LOGO_WIDTH.
  SplashCell: SplashCell#
  SplashTone: SplashTone#
  PrimeOnboardingSplashComponent.mod: PrimeOnboardingSplashComponent#mod().
  PrimeOnboardingSplashComponent: PrimeOnboardingSplashComponent#
  PrimeOnboardingSplashComponent.dispose: PrimeOnboardingSplashComponent#dispose().
  LOGO_LINES: LOGO_LINES.
  PanelLine: PanelLine#
  LAB_FIELD_HEIGHT: LAB_FIELD_HEIGHT.
  SplashCell.priority: SplashCell#priority.
  PanelLine.left: PanelLine#left.
  PanelLine.parts: PanelLine#parts.
  SplashCell.char: SplashCell#char.
  QuietZone: QuietZone#
  PrimeOnboardingSplashComponent.animationInterval: PrimeOnboardingSplashComponent#animationInterval.
  PrimeOnboardingSplashComponent.progressMessage: PrimeOnboardingSplashComponent#progressMessage.
  PrimeOnboardingSplashComponent.getTargetRows: PrimeOnboardingSplashComponent#getTargetRows().
  PrimeOnboardingSplashOptions.requestRender: PrimeOnboardingSplashOptions#requestRender.
  StyledText.bold: StyledText#bold.
  LAB_FIELD_MIN_WIDTH: LAB_FIELD_MIN_WIDTH.
  SplashCell.bold: SplashCell#bold.
  SplashCell.italic: SplashCell#italic.
  StyledText.italic: StyledText#italic.
  QuietZone.top: QuietZone#top.
  PrimeOnboardingSplashComponent.frame: PrimeOnboardingSplashComponent#frame.
  PrimeOnboardingSplashOptions: PrimeOnboardingSplashOptions#
  PrimeOnboardingSplashOptions.getRows: PrimeOnboardingSplashOptions#getRows.
  PrimeOnboardingSplashOptions.animationIntervalMs: PrimeOnboardingSplashOptions#animationIntervalMs.
  PrimeOnboardingSplashOptions.continueActionLabel: PrimeOnboardingSplashOptions#continueActionLabel.
  ANIMATION_INTERVAL_MS: ANIMATION_INTERVAL_MS.
  LAB_FIELD_MAX_WIDTH: LAB_FIELD_MAX_WIDTH.
  StyledText: StyledText#
  StyledText.transparentSpaces: StyledText#transparentSpaces.
  QuietZone.left: QuietZone#left.
  QuietZone.right: QuietZone#right.
  QuietZone.bottom: QuietZone#bottom.
  PrimeOnboardingSplashComponent.invalidate: PrimeOnboardingSplashComponent#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts)

## Classes
### `PanelLine`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L39)
- signature: `interface PanelLine`
- members:
  - `left` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L40)
  - `parts` — [`L41`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L41)
- uses (calls/refs, reference-scoped): [`PanelTextLine`](prime-onboarding-splash.ts.md#PanelTextLine)
- used by: [`render`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.render), [`renderPanel`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderPanel), [`centerParts`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.centerParts)

### `PanelTextLine`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L37)
- signature: `type PanelTextLine`
- uses (calls/refs, reference-scoped): [`StyledText`](prime-onboarding-splash.ts.md#StyledText)
- used by: [`drawStyledText`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.drawStyledText), [`formatContinueHint`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.formatContinueHint), [`centerParts`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.centerParts), [`formatBrandLine`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.formatBrandLine), [`renderLogoBlock`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderLogoBlock), [`visiblePartsWidth`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.visiblePartsWidth), [`PanelLine`](prime-onboarding-splash.ts.md#PanelLine)

### `PrimeOnboardingSplashComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L51)
- signature: `class PrimeOnboardingSplashComponent`
- members:
  - `<constructor>(onSelect: () => void, onCancel: () => void, options?: PrimeOnboardingSplashOptions)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L56)
  - `centerParts(method)` — [`L363`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L363)
  - `dispose(method)` — [`L73`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L73)
  - `drawLabField(method)` — [`L167`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L167)
  - `drawStyledText(method)` — [`L270`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L270)
  - `formatBrandLine(method)` — [`L126`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L126)
  - `formatContinueHint(method)` — [`L114`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L114)
  - `getTargetRows(method)` — [`L368`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L368)
  - `handleInput(method)` — [`L100`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L100) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L69) — Invalidate any cached rendering state.
  - `isInsideQuietZone(method)` — [`L260`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L260)
  - `labCell(method)` — [`L193`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L193)
  - `logoQuietZone(method)` — [`L349`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L349)
  - `mod(method)` — [`L341`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L341)
  - `put(method)` — [`L289`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L289)
  - `render(method)` — [`L87`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L87) — Render the component to lines for the given viewport width
  - `renderBackdrop(method)` — [`L157`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L157)
  - `renderCells(method)` — [`L306`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L306)
  - `renderLogoBlock(method)` — [`L149`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L149)
  - `renderPanel(method)` — [`L134`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L134)
  - `showProgress(method)` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L81)
  - `visiblePartsWidth(method)` — [`L345`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L345)
  - `animationInterval` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L53)
  - `frame` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L52)
  - `progressMessage` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L54)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`bold`](../theme/theme.ts.md#Theme.bold), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`tone`](prime-onboarding-splash.ts.md#StyledText.tone), [`PanelTextLine`](prime-onboarding-splash.ts.md#PanelTextLine), [`text`](prime-onboarding-splash.ts.md#StyledText.text), [`tone`](prime-onboarding-splash.ts.md#SplashCell.tone), [`SplashCell`](prime-onboarding-splash.ts.md#SplashCell), [`LOGO_WIDTH`](prime-onboarding-splash.ts.md#LOGO_WIDTH), [`SplashTone`](prime-onboarding-splash.ts.md#SplashTone), [`PanelLine`](prime-onboarding-splash.ts.md#PanelLine), [`LOGO_LINES`](prime-onboarding-splash.ts.md#LOGO_LINES), [`LAB_FIELD_HEIGHT`](prime-onboarding-splash.ts.md#LAB_FIELD_HEIGHT), [`left`](prime-onboarding-splash.ts.md#PanelLine.left), [`parts`](prime-onboarding-splash.ts.md#PanelLine.parts), [`priority`](prime-onboarding-splash.ts.md#SplashCell.priority), [`QuietZone`](prime-onboarding-splash.ts.md#QuietZone), [`char`](prime-onboarding-splash.ts.md#SplashCell.char), [`italic`](../theme/theme.ts.md#Theme.italic), [`bold`](prime-onboarding-splash.ts.md#StyledText.bold), [`requestRender`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashOptions.requestRender), [`LAB_FIELD_MIN_WIDTH`](prime-onboarding-splash.ts.md#LAB_FIELD_MIN_WIDTH), [`bold`](prime-onboarding-splash.ts.md#SplashCell.bold), [`italic`](prime-onboarding-splash.ts.md#SplashCell.italic), [`italic`](prime-onboarding-splash.ts.md#StyledText.italic), [`top`](prime-onboarding-splash.ts.md#QuietZone.top), [`PrimeOnboardingSplashOptions`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashOptions), [`ANIMATION_INTERVAL_MS`](prime-onboarding-splash.ts.md#ANIMATION_INTERVAL_MS), [`LAB_FIELD_MAX_WIDTH`](prime-onboarding-splash.ts.md#LAB_FIELD_MAX_WIDTH), [`animationIntervalMs`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashOptions.animationIntervalMs), [`bottom`](prime-onboarding-splash.ts.md#QuietZone.bottom), [`continueActionLabel`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashOptions.continueActionLabel), [`getRows`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashOptions.getRows), [`left`](prime-onboarding-splash.ts.md#QuietZone.left), [`right`](prime-onboarding-splash.ts.md#QuietZone.right)  (+1 more)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`showOnboardingSplash`](../interactive-mode.ts.md#InteractiveMode.showOnboardingSplash)  (1 test-only)

### `PrimeOnboardingSplashOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L5)
- signature: `interface PrimeOnboardingSplashOptions`
- members:
  - `animationIntervalMs` — [`L8`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L8)
  - `continueActionLabel` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L9)
  - `getRows` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L6)
  - `requestRender` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L7)
- used by: [`<constructor>`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.-constructor), [`formatContinueHint`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.formatContinueHint), [`showProgress`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.showProgress), [`getTargetRows`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.getTargetRows)

### `QuietZone`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L44)
- signature: `interface QuietZone`
- members:
  - `bottom` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L48)
  - `left` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L45)
  - `right` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L46)
  - `top` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L47)
- used by: [`drawLabField`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.drawLabField), [`renderBackdrop`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderBackdrop), [`isInsideQuietZone`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.isInsideQuietZone), [`logoQuietZone`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.logoQuietZone)

### `SplashCell`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L21)
- signature: `interface SplashCell`
- members:
  - `bold` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L25)
  - `char` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L22)
  - `italic` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L26)
  - `priority` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L24)
  - `tone` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L23)
- uses (calls/refs, reference-scoped): [`SplashTone`](prime-onboarding-splash.ts.md#SplashTone)
- used by: [`drawLabField`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.drawLabField), [`renderCells`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderCells), [`drawStyledText`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.drawStyledText), [`put`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.put), [`labCell`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.labCell), [`renderBackdrop`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderBackdrop)

### `SplashTone`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L19)
- signature: `type SplashTone`
- uses (calls/refs, reference-scoped): [`ThemeColor`](../theme/theme.ts.md#ThemeColor)
- used by: [`renderCells`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.renderCells), [`put`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.put), [`labCell`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.labCell), [`tone`](prime-onboarding-splash.ts.md#StyledText.tone), [`tone`](prime-onboarding-splash.ts.md#SplashCell.tone)

### `StyledText`
- def: [`packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts:29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L29)
- signature: `interface StyledText`
- members:
  - `bold` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L32)
  - `italic` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L33)
  - `text` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L30)
  - `tone` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L31)
  - `transparentSpaces` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L34)
- uses (calls/refs, reference-scoped): [`SplashTone`](prime-onboarding-splash.ts.md#SplashTone)
- used by: [`drawStyledText`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.drawStyledText), [`formatContinueHint`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.formatContinueHint), [`formatBrandLine`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.formatBrandLine), [`PanelTextLine`](prime-onboarding-splash.ts.md#PanelTextLine), [`visiblePartsWidth`](prime-onboarding-splash.ts.md#PrimeOnboardingSplashComponent.visiblePartsWidth)

## Module values
- `ANIMATION_INTERVAL_MS` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L14)
- `LAB_FIELD_HEIGHT` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L15)
- `LAB_FIELD_MAX_WIDTH` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L17)
- `LAB_FIELD_MIN_WIDTH` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L16)
- `LOGO_LINES` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L12)
- `LOGO_WIDTH` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/prime-onboarding-splash.ts#L13)

