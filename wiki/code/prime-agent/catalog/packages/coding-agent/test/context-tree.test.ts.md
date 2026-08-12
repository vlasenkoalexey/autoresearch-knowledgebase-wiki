---
title: 'Module: packages/coding-agent/test/context-tree.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/context-tree.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`context-tree.test.ts`/
symbols:
  createUsage: createUsage().
  createAssistantMessage: createAssistantMessage().
  writeChildSession.typeLiteral0.sessionManager: writeChildSession().typeLiteral0:sessionManager.
  model: model.
  makeTempDir: makeTempDir().
  writeChildSession: writeChildSession().
  resolveContextWindow: resolveContextWindow.
  createUserMessage: createUserMessage().
  writeChildSession.typeLiteral0.assistantEntryId: writeChildSession().typeLiteral0:assistantEntryId.
  tempDirs: tempDirs.
---
# Module: [`packages/coding-agent/test/context-tree.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts)

## Functions
- `createAssistantMessage(text: string, usage: Usage)` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L42)
- `createUsage(input: number, output: number, cost: number)` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L25)
- `createUserMessage(text: string)` — [`L55`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L55)
- `makeTempDir()` — [`L86`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L86)
- `writeChildSession(dir: string, prompt: string, assistantUsage: Usage)` — [`L68`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L68) — Write a child agent session into `dir` the way RLM child runs persist them:

## Module values
- `assistantEntryId` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L72)
- `model` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L19)
- `resolveContextWindow` — [`L82`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L82)
- `sessionManager` — [`L72`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L72)
- `tempDirs` — [`L84`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/context-tree.test.ts#L84)

