---
title: 'Module: packages/coding-agent/test/telemetry.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/telemetry.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`telemetry.test.ts`/
symbols:
  assistantMessage: assistantMessage().
  FakeAgentSession.emit: FakeAgentSession#emit().
  FakeTelemetrySink.capture: FakeTelemetrySink#capture().
  FakeTelemetrySink.events: FakeTelemetrySink#events.
  FakeTelemetrySink: FakeTelemetrySink#
  FakeTelemetrySink.events.Array.typeLiteral3.name: FakeTelemetrySink#events.Array:typeLiteral3:name.
  uuidGenerator: uuidGenerator().
  FakeAgentSession.listener: FakeAgentSession#listener.
  FakeTelemetrySink.events.Array.typeLiteral3.properties: FakeTelemetrySink#events.Array:typeLiteral3:properties.
  FakeAgentSession.subscribe: FakeAgentSession#subscribe().
  FakeAgentSession: FakeAgentSession#
  FakeAgentSession.dispose: FakeAgentSession#dispose().
  FakeAgentSession.disposeAsync: FakeAgentSession#disposeAsync().
  FakeTelemetrySink.flushCount: FakeTelemetrySink#flushCount.
  FakeAgentSession.disposeCallback: FakeAgentSession#disposeCallback.
  FakeTelemetrySink.flush: FakeTelemetrySink#flush().
  FakeAgentSession.registerDisposeCallback: FakeAgentSession#registerDisposeCallback().
---
# Module: [`packages/coding-agent/test/telemetry.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts)

## Classes
### `FakeAgentSession`
- def: [`packages/coding-agent/test/telemetry.test.ts:70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L70)
- signature: `class FakeAgentSession`
- members:
  - `dispose(method)` — [`L89`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L89)
  - `disposeAsync(method)` — [`L93`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L93)
  - `emit(method)` — [`L85`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L85)
  - `registerDisposeCallback(method)` — [`L81`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L81)
  - `subscribe(method)` — [`L74`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L74)
  - `disposeCallback` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L72)
  - `listener` — [`L71`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L71)
- uses (calls/refs, reference-scoped): [`AgentSessionEvent`](../src/core/agent-session.ts.md#AgentSessionEvent)
- used by: (1 test-only callers)

### `FakeTelemetrySink`  ·  implements/extends TelemetrySink
- def: [`packages/coding-agent/test/telemetry.test.ts:56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L56)
- signature: `class FakeTelemetrySink`
- members:
  - `capture(method)` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L61)
  - `flush(method)` — [`L65`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L65)
  - `events` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L57)
  - `flushCount` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L59)
  - `name` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L57)
  - `properties` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L57)
- uses (calls/refs, reference-scoped): [`TelemetrySink`](../src/core/telemetry.ts.md#TelemetrySink), [`TelemetryEventName`](../src/core/telemetry.ts.md#TelemetryEventName)
- used by: [`capture`](../src/core/telemetry.ts.md#TelemetrySink.capture), [`TelemetrySink`](../src/core/telemetry.ts.md#TelemetrySink), [`flush`](../src/core/telemetry.ts.md#TelemetrySink.flush)  (1 test-only)

## Functions
- `assistantMessage(overrides?: Partial<AssistantMessage>)` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L29)
- `uuidGenerator()` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/telemetry.test.ts#L21)

