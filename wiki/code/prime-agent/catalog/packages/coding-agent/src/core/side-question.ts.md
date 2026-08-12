---
title: 'Module: packages/coding-agent/src/core/side-question.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/side-question.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`side-question.ts`/
symbols:
  startSideQuestion: startSideQuestion().
  readAssistantText: readAssistantText().
  SideQuestionRun.done: SideQuestionRun#done.
  SideQuestionEvent: SideQuestionEvent#
  SideQuestionRun.abort: SideQuestionRun#abort().
  SideQuestionRun: SideQuestionRun#
  SideQuestionEvent.status: SideQuestionEvent#status.
  sideQuestionPrompt: sideQuestionPrompt().
  SideQuestionStatus: SideQuestionStatus#
  SideQuestionEvent.id: SideQuestionEvent#id.
  SideQuestionTurn.question: SideQuestionTurn#question.
  SideQuestionTurn.answer: SideQuestionTurn#answer.
  SideQuestionEvent.question: SideQuestionEvent#question.
  SideQuestionEvent.answer: SideQuestionEvent#answer.
  SideQuestionEvent.errorMessage: SideQuestionEvent#errorMessage.
  SideQuestionTurn: SideQuestionTurn#
  SIDE_QUESTION_INSTRUCTION: SIDE_QUESTION_INSTRUCTION.
---
# Module: [`packages/coding-agent/src/core/side-question.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts)

## Classes
### `SideQuestionEvent`
- def: [`packages/coding-agent/src/core/side-question.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L6)
- signature: `interface SideQuestionEvent`
- members:
  - `answer` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L9)
  - `errorMessage` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L11)
  - `id` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L7)
  - `question` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L8)
  - `status` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L10)
- uses (calls/refs, reference-scoped): [`SideQuestionStatus`](side-question.ts.md#SideQuestionStatus)
- used by: [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`startSideQuestion`](side-question.ts.md#startSideQuestion)  (1 test-only)

### `SideQuestionRun`
- def: [`packages/coding-agent/src/core/side-question.ts:19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L19)
- signature: `interface SideQuestionRun`
- members:
  - `abort(method)` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L21)
  - `done` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L20)
- used by: [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`startSideQuestion`](side-question.ts.md#startSideQuestion), [`startSideQuestion`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.startSideQuestion), [`sideQuestionRuns`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sideQuestionRuns), [`abortSideQuestionsFor`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.abortSideQuestionsFor), [`sideQuestionRuns`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.sideQuestionRuns), [`abortAllSideQuestions`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.abortAllSideQuestions), [`abortSideQuestion`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.abortSideQuestion)  (2 test-only)

### `SideQuestionStatus`
- def: [`packages/coding-agent/src/core/side-question.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L4)
- signature: `type SideQuestionStatus`
- used by: [`startSideQuestion`](side-question.ts.md#startSideQuestion), [`status`](side-question.ts.md#SideQuestionEvent.status)

### `SideQuestionTurn`
- def: [`packages/coding-agent/src/core/side-question.ts:14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L14)
- signature: `interface SideQuestionTurn`
- members:
  - `answer` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L16)
  - `question` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L15)
- used by: [`startSideQuestion`](side-question.ts.md#startSideQuestion)  (1 test-only)

## Functions
- `readAssistantText(message: AgentMessage)` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L32)
- `sideQuestionPrompt(question: string, isFirstTurn: boolean)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L27)
- `startSideQuestion(parent: Agent, id: string, question: string, onEvent: (event: SideQuestionEvent) => void | Promise<void>, previousTurns?: SideQuestionTurn[])` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L42)

## Module values
- `SIDE_QUESTION_INSTRUCTION` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/side-question.ts#L24)

