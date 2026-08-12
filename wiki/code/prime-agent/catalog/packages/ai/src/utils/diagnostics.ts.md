---
title: 'Module: packages/ai/src/utils/diagnostics.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/diagnostics.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`diagnostics.ts`/
symbols:
  createAssistantMessageDiagnostic: createAssistantMessageDiagnostic().
  extractDiagnosticError: extractDiagnosticError().
  appendAssistantMessageDiagnostic: appendAssistantMessageDiagnostic().
  AssistantMessageDiagnostic.type: AssistantMessageDiagnostic#type.
  AssistantMessageDiagnostic.details: AssistantMessageDiagnostic#details.
  AssistantMessageDiagnostic: AssistantMessageDiagnostic#
  AssistantMessageDiagnostic.timestamp: AssistantMessageDiagnostic#timestamp.
  formatThrownValue: formatThrownValue().
  AssistantMessageDiagnostic.error: AssistantMessageDiagnostic#error.
  DiagnosticErrorInfo: DiagnosticErrorInfo#
  DiagnosticErrorInfo.name: DiagnosticErrorInfo#name.
  DiagnosticErrorInfo.message: DiagnosticErrorInfo#message.
  appendAssistantMessageDiagnostic.T-typeLiteral9.diagnostics: appendAssistantMessageDiagnostic().[T]typeLiteral9:diagnostics.
  DiagnosticErrorInfo.stack: DiagnosticErrorInfo#stack.
  DiagnosticErrorInfo.code: DiagnosticErrorInfo#code.
---
# Module: [`packages/ai/src/utils/diagnostics.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts)

## Classes
### `AssistantMessageDiagnostic`
- def: [`packages/ai/src/utils/diagnostics.ts:8`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L8)
- signature: `interface AssistantMessageDiagnostic`
- members:
  - `details` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L12)
  - `error` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L11)
  - `timestamp` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L10)
  - `type` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L9)
- uses (calls/refs, reference-scoped): [`DiagnosticErrorInfo`](diagnostics.ts.md#DiagnosticErrorInfo)
- used by: [`types.ts`](../types.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-types.ts), [`recordStreamFailure`](stream-failure.ts.md#recordStreamFailure), [`createAssistantMessageDiagnostic`](diagnostics.ts.md#createAssistantMessageDiagnostic), [`_getProviderStreamFailureDetails`](../../../coding-agent/src/core/agent-session.ts.md#AgentSession._getProviderStreamFailureDetails), [`diagnostics`](../types.ts.md#AssistantMessage.diagnostics), [`appendAssistantMessageDiagnostic`](diagnostics.ts.md#appendAssistantMessageDiagnostic), [`_isAgentLifecycleFailure`](../../../coding-agent/src/core/agent-session.ts.md#AgentSession._isAgentLifecycleFailure)  (4 test-only)

### `DiagnosticErrorInfo`
- def: [`packages/ai/src/utils/diagnostics.ts:1`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L1)
- signature: `interface DiagnosticErrorInfo`
- members:
  - `code` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L5)
  - `message` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L3)
  - `name` — [`L2`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L2)
  - `stack` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L4)
- used by: [`extractDiagnosticError`](diagnostics.ts.md#extractDiagnosticError), [`error`](diagnostics.ts.md#AssistantMessageDiagnostic.error)

## Functions
- `appendAssistantMessageDiagnostic(message: T, diagnostic: AssistantMessageDiagnostic)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L40)
- `createAssistantMessageDiagnostic(type: string, error: unknown, details?: Record<string, unknown> | undefined)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L32)
- `extractDiagnosticError(error: unknown)` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L21)
- `formatThrownValue(value: unknown)` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L15)

## Module values
- `diagnostics` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/diagnostics.ts#L40)

