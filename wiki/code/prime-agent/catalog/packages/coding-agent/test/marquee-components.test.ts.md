---
title: 'Module: packages/coding-agent/test/marquee-components.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/marquee-components.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`marquee-components.test.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  EMPTY_USAGE: EMPTY_USAGE.
  renderInVirtualTerminal: renderInVirtualTerminal().
  HostComponent.-constructor: HostComponent#`<constructor>`().
  createFakeTui: createFakeTui().
  HostComponent: HostComponent#
  HostComponent.render: HostComponent#render().
  HostComponent.invalidate: HostComponent#invalidate().
---
# Module: [`packages/coding-agent/test/marquee-components.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts)

## Classes
### `HostComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/test/marquee-components.test.ts:12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L12)
- signature: `class HostComponent`
- members:
  - `<constructor>(child: Component)` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L13)
  - `invalidate(method)` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L19) — Invalidate any cached rendering state.
  - `render(method)` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L15) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`Component`](../../tui/src/tui.ts.md#Component), [`render`](../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../tui/src/tui.ts.md#Component.invalidate)
- used by: [`Component`](../../tui/src/tui.ts.md#Component), [`render`](../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../tui/src/tui.ts.md#Component.invalidate)  (1 test-only)

## Functions
- `createAssistantMessage(text: string, thinking?: string | undefined)` — [`L45`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L45)
- `createFakeTui()` — [`L24`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L24)
- `renderInVirtualTerminal(component: Component, width?: number, height?: number)` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L58)

## Module values
- `EMPTY_USAGE` — [`L30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/marquee-components.test.ts#L30)

