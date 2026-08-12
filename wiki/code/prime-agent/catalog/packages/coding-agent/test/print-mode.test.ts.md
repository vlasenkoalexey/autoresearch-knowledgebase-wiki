---
title: 'Module: packages/coding-agent/test/print-mode.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/print-mode.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`print-mode.test.ts`/
symbols:
  createRuntimeHost: createRuntimeHost().
  createAssistantMessage.options-typeLiteral11.errorMessage: createAssistantMessage().(options)typeLiteral11:errorMessage.
  FakeSession.typeLiteral6.prompt: FakeSession#typeLiteral6:prompt.
  createAssistantMessage: createAssistantMessage().
  FakeRuntimeHost.typeLiteral10.session: FakeRuntimeHost#typeLiteral10:session.
  output: output.
  FakeSession.typeLiteral6.extensionRunner: FakeSession#typeLiteral6:extensionRunner.
  FakeExtensionRunner.typeLiteral0.emit: FakeExtensionRunner#typeLiteral0:emit.
  FakeSession.typeLiteral6.getAutonomousStatus: FakeSession#typeLiteral6:getAutonomousStatus.
  FakeSession.typeLiteral6.recordHostAutonomousContinuation: FakeSession#typeLiteral6:recordHostAutonomousContinuation.
  createAssistantMessage.options-typeLiteral11.stopReason: createAssistantMessage().(options)typeLiteral11:stopReason.
  FakeSession.typeLiteral6.state.typeLiteral9.messages: FakeSession#typeLiteral6:state.typeLiteral9:messages.
  FakeSession.typeLiteral6.waitForIdle: FakeSession#typeLiteral6:waitForIdle.
  FakeSession.typeLiteral6.promptAndWait: FakeSession#typeLiteral6:promptAndWait.
  FakeExtensionRunner: FakeExtensionRunner#
  FakeSession.typeLiteral6.state: FakeSession#typeLiteral6:state.
  EmitEvent: EmitEvent#
  FakeSession.typeLiteral6.messages: FakeSession#typeLiteral6:messages.
  FakeSession.typeLiteral6.refreshAutonomousGates: FakeSession#typeLiteral6:refreshAutonomousGates.
  FakeSession: FakeSession#
  FakeRuntimeHost.typeLiteral10.dispose: FakeRuntimeHost#typeLiteral10:dispose.
  createAssistantMessage.options-typeLiteral11.text: createAssistantMessage().(options)typeLiteral11:text.
  FakeExtensionRunner.typeLiteral0.hasHandlers: FakeExtensionRunner#typeLiteral0:hasHandlers.
  FakeSession.typeLiteral6.sessionManager: FakeSession#typeLiteral6:sessionManager.
  FakeSession.typeLiteral6.sessionManager.typeLiteral7.getHeader: FakeSession#typeLiteral6:sessionManager.typeLiteral7:getHeader.
  FakeSession.typeLiteral6.agent: FakeSession#typeLiteral6:agent.
  FakeSession.typeLiteral6.agent.typeLiteral8.waitForIdle: FakeSession#typeLiteral6:agent.typeLiteral8:waitForIdle.
  FakeSession.typeLiteral6.bindExtensions: FakeSession#typeLiteral6:bindExtensions.
  FakeSession.typeLiteral6.subscribe: FakeSession#typeLiteral6:subscribe.
  FakeSession.typeLiteral6.reload: FakeSession#typeLiteral6:reload.
  FakeRuntimeHost: FakeRuntimeHost#
  FakeRuntimeHost.typeLiteral10.newSession: FakeRuntimeHost#typeLiteral10:newSession.
  FakeRuntimeHost.typeLiteral10.fork: FakeRuntimeHost#typeLiteral10:fork.
  FakeRuntimeHost.typeLiteral10.switchSession: FakeRuntimeHost#typeLiteral10:switchSession.
  FakeRuntimeHost.typeLiteral10.setRebindSession: FakeRuntimeHost#typeLiteral10:setRebindSession.
---
# Module: [`packages/coding-agent/test/print-mode.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts)

## Classes
### `EmitEvent`
- def: [`packages/coding-agent/test/print-mode.test.ts:23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L23)
- signature: `type EmitEvent`
- uses (calls/refs, reference-scoped): [`SessionShutdownEvent`](../src/core/extensions/types.ts.md#SessionShutdownEvent)
- used by: (1 test-only callers)

### `FakeExtensionRunner`
- def: [`packages/coding-agent/test/print-mode.test.ts:25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L25)
- signature: `type FakeExtensionRunner`
- members:
  - `emit` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L27)
  - `hasHandlers` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L26)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

### `FakeRuntimeHost`
- def: [`packages/coding-agent/test/print-mode.test.ts:47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L47)
- signature: `type FakeRuntimeHost`
- members:
  - `dispose` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L52)
  - `fork` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L50)
  - `newSession` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L49)
  - `session` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L48)
  - `setRebindSession` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L53)
  - `switchSession` — [`L51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L51)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `FakeSession`
- def: [`packages/coding-agent/test/print-mode.test.ts:30`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L30)
- signature: `type FakeSession`
- members:
  - `agent` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L32)
  - `bindExtensions` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L37)
  - `extensionRunner` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L36)
  - `getAutonomousStatus` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L42)
  - `getHeader` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L31)
  - `messages` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L34)
  - `messages` — [`L35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L35)
  - `prompt` — [`L39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L39)
  - `promptAndWait` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L40)
  - `recordHostAutonomousContinuation` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L43)
  - `refreshAutonomousGates` — [`L44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L44)
  - `reload` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L41)
  - `sessionManager` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L31)
  - `state` — [`L34`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L34)
  - `subscribe` — [`L38`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L38)
  - `waitForIdle` — [`L32`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L32)
  - `waitForIdle` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L33)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../agent/src/types.ts.md#AgentMessage)  (1 test-only)
- used by: (3 test-only callers)

## Functions
- `createAssistantMessage(options?: { text?: string | undefined; stopReason?: StopReason | undefined; errorMessage?: string | undefined; } | undefined)` — [`L56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L56)
- `createRuntimeHost(assistantMessage: AgentMessage | AgentMessage[], autonomousStatus?: AgentAutonomousStatus)` — [`L81`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L81)

## Module values
- `errorMessage` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L59)
- `output` — [`L14`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L14)
- `stopReason` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L58)
- `text` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/print-mode.test.ts#L57)

