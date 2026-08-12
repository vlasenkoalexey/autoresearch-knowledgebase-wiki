---
title: 'Module: packages/coding-agent/src/modes/interactive/components/footer.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/footer.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`footer.ts`/FooterComponent#
symbols:
  FooterComponent.invalidate: invalidate().
  FooterComponent: ''
  FooterComponent.-constructor: '`<constructor>`().'
  FooterComponent.setAutoCompactEnabled: setAutoCompactEnabled().
  FooterComponent.render: render().
  FooterComponent.dispose: dispose().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/footer.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts)

## Classes
### `FooterComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/footer.ts:12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L12)
- doc: Footer component for the prime brand TUI.
- signature: `class FooterComponent`
- members:
  - `<constructor>(footerData: ReadonlyFooterDataProvider)` — [`L13`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L13) — Footer component for the prime brand TUI.
  - `dispose(method)` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L33) — Clean up resources.
  - `invalidate(method)` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L25) — No-op: git branch caching now handled by provider.
  - `render(method)` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L37) — Render the component to lines for the given viewport width
  - `setAutoCompactEnabled(method)` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/footer.ts#L17)
- uses (calls/refs, reference-scoped): [`Component`](../../../../../tui/src/tui.ts.md#Component), [`ReadonlyFooterDataProvider`](../../../core/footer-data-provider.ts.md#ReadonlyFooterDataProvider)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`showSettingsSelector`](../interactive-mode.ts.md#InteractiveMode.showSettingsSelector), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`<constructor>`](../interactive-mode.ts.md#InteractiveMode.-constructor), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`limitTranscript`](../interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`resetExtensionUI`](../interactive-mode.ts.md#InteractiveMode.resetExtensionUI), [`applyRuntimeSettings`](../interactive-mode.ts.md#InteractiveMode.applyRuntimeSettings), [`stop`](../interactive-mode.ts.md#InteractiveMode.stop), [`createAuthFlows`](../interactive-mode.ts.md#InteractiveMode.createAuthFlows), [`applySelectedModel`](../interactive-mode.ts.md#InteractiveMode.applySelectedModel), [`handleFastCommand`](../interactive-mode.ts.md#InteractiveMode.handleFastCommand), [`applyConnectionStateSnapshot`](../interactive-mode.ts.md#InteractiveMode.applyConnectionStateSnapshot), [`applyThinkingLevel`](../interactive-mode.ts.md#InteractiveMode.applyThinkingLevel), [`footer`](../interactive-mode.ts.md#InteractiveMode.footer), [`applyAuthStaleEvent`](../interactive-mode.ts.md#InteractiveMode.applyAuthStaleEvent)  (1 test-only)

