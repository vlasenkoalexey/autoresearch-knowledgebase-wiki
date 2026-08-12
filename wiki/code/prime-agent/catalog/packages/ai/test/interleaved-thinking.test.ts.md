---
title: 'Module: packages/ai/test/interleaved-thinking.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/interleaved-thinking.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`interleaved-thinking.test.ts`/
symbols:
  assertSecondToolCallWithInterleavedThinking: assertSecondToolCallWithInterleavedThinking().
  asCalculatorArguments: asCalculatorArguments().
  evaluateCalculatorCall: evaluateCalculatorCall().
  calculatorTool: calculatorTool.
  calculatorSchema: calculatorSchema.
  CalculatorArguments.typeLiteral6.operation: CalculatorArguments#typeLiteral6:operation.
  CalculatorArguments.typeLiteral6.a: CalculatorArguments#typeLiteral6:a.
  CalculatorArguments.typeLiteral6.b: CalculatorArguments#typeLiteral6:b.
  CalculatorOperation: CalculatorOperation#
  CalculatorArguments: CalculatorArguments#
  hasAnthropicCredentials: hasAnthropicCredentials.
---
# Module: [`packages/ai/test/interleaved-thinking.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts)

## Classes
### `CalculatorArguments`
- def: [`packages/ai/test/interleaved-thinking.test.ts:26`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L26)
- signature: `type CalculatorArguments`
- members:
  - `a` — [`L27`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L27)
  - `b` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L28)
  - `operation` — [`L29`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L29)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `CalculatorOperation`
- def: [`packages/ai/test/interleaved-thinking.test.ts:24`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L24)
- signature: `type CalculatorOperation`
- used by: (1 test-only callers)

## Functions
- `asCalculatorArguments(args: Record<string, any>)` — [`L32`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L32)
- `assertSecondToolCallWithInterleavedThinking(llm: Model<TApi>, reasoning: "high" | "xhigh")` — [`L64`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L64)
- `evaluateCalculatorCall(toolCall: ToolCall)` — [`L50`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L50)

## Module values
- `calculatorSchema` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L10)
- `calculatorTool` — [`L18`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L18)
- `hasAnthropicCredentials` — [`L121`](../../../../../../../raw/code/prime-agent/packages/ai/test/interleaved-thinking.test.ts#L121)

