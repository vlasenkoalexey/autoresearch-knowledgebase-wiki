---
title: 'Module: packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4531-agent-message-ui.test.ts`/
symbols:
  createPayload: createPayload().
  render: render().
  stripAnsi: stripAnsi().
  LateSentAgentMessageHost.typeLiteral0._lateIpythonSentAgentMessages: LateSentAgentMessageHost#typeLiteral0:_lateIpythonSentAgentMessages.
  LateSentAgentMessageHost.typeLiteral0._recordLateIpythonSentAgentMessage: LateSentAgentMessageHost#typeLiteral0:_recordLateIpythonSentAgentMessage.
  LateSentAgentMessageHost.typeLiteral0._restoreLateIpythonSentAgentMessages: LateSentAgentMessageHost#typeLiteral0:_restoreLateIpythonSentAgentMessages.
  LateSentAgentMessageHost: LateSentAgentMessageHost#
  LateSentAgentMessageHost.typeLiteral0._agentEventQueue: LateSentAgentMessageHost#typeLiteral0:_agentEventQueue.
---
# Module: [`packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts)

## Classes
### `LateSentAgentMessageHost`
- def: [`packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts:54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L54)
- signature: `type LateSentAgentMessageHost`
- protocol/private: `_agentEventQueue`[`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L56), `_lateIpythonSentAgentMessages`[`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L57), `_recordLateIpythonSentAgentMessage`[`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L55), `_restoreLateIpythonSentAgentMessages`[`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L58)
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](../../../src/core/kernel/index.ts.md#KernelSentAgentMessage)
- used by: (1 test-only callers)

## Functions
- `createPayload(message: string)` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L28)
- `render(component: AgentMessageComponent)` — [`L50`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L50)
- `stripAnsi(text: string)` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4531-agent-message-ui.test.ts#L46)

