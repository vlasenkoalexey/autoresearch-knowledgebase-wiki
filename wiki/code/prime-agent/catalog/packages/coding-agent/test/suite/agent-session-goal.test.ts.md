---
title: 'Module: packages/coding-agent/test/suite/agent-session-goal.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/agent-session-goal.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`agent-session-goal.test.ts`/
symbols:
  createWaitingTool: createWaitingTool().
  currentAgentContext: currentAgentContext().
  goalContextMessages: goalContextMessages().
  createFauxIpythonTool: createFauxIpythonTool().
  assistantWithUsage: assistantWithUsage().
  visibleAssistantTexts: visibleAssistantTexts().
  COMPLETE_GOAL_CELL: COMPLETE_GOAL_CELL.
  createWaitingTool.typeLiteral53.tool: createWaitingTool().typeLiteral53:tool.
  createWaitingTool.typeLiteral53.waitForStart: createWaitingTool().typeLiteral53:waitForStart.
  createWaitingTool.typeLiteral53.release: createWaitingTool().typeLiteral53:release.
  waitForCondition: waitForCondition().
  createFauxIpythonTool.sessionRef-typeLiteral18.current: createFauxIpythonTool().(sessionRef)typeLiteral18:current.
---
# Module: [`packages/coding-agent/test/suite/agent-session-goal.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts)

## Functions
- `assistantWithUsage(message: string | AssistantMessage, usage: Partial<Usage>)` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L17)
- `createFauxIpythonTool(sessionRef: { current?: AgentSession | undefined; })` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L69) — Stand-in for the real ipython tool. Goal calls reach the host over the
- `createWaitingTool()` — [`L98`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L98)
- `currentAgentContext(harness: Harness)` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L42)
- `goalContextMessages(harness: Harness)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L32)
- `visibleAssistantTexts(harness: Harness)` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L38)
- `waitForCondition(predicate: () => boolean)` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L51)

## Module values
- `COMPLETE_GOAL_CELL` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L96)
- `current` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L69)
- `release` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L100)
- `tool` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L99)
- `waitForStart` — [`L101`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/agent-session-goal.test.ts#L101)

