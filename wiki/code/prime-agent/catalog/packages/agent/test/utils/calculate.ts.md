---
title: 'Module: packages/agent/test/utils/calculate.ts'
type: catalog
provenance: extracted
module: packages/agent/test/utils/calculate.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-agent-core 0.7.2 test/utils/`calculate.ts`/
symbols:
  calculate: calculate().
  CalculateResult: CalculateResult#
  CalculateParams: CalculateParams#
  calculateSchema: calculateSchema.
  calculateTool: calculateTool.
  CalculateResult.content: CalculateResult#content.
  CalculateResult.content.Array.typeLiteral0.type: CalculateResult#content.Array:typeLiteral0:type.
  CalculateResult.content.Array.typeLiteral0.text: CalculateResult#content.Array:typeLiteral0:text.
  CalculateResult.details: CalculateResult#details.
---
# Module: [`packages/agent/test/utils/calculate.ts`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts)

## Classes
### `CalculateParams`
- def: [`packages/agent/test/utils/calculate.ts:22`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L22)
- signature: `type CalculateParams`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `CalculateResult`
- def: [`packages/agent/test/utils/calculate.ts:4`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L4)
- signature: `interface CalculateResult`
- members:
  - `content` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L5) — Text or image content returned to the model.
  - `details` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L6) — Arbitrary structured details for logs or UI rendering.
  - `text` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L5)
  - `type` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L5)
- uses (calls/refs, reference-scoped): [`AgentToolResult`](../../src/types.ts.md#AgentToolResult)
- used by: (1 test-only callers)

## Functions
- `calculate(expression: string)` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L9)

## Module values
- `calculateSchema` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L18)
- `calculateTool` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/agent/test/utils/calculate.ts#L24)

