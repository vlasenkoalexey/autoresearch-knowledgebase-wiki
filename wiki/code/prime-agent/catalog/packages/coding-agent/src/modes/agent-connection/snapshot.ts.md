---
title: 'Module: packages/coding-agent/src/modes/agent-connection/snapshot.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/agent-connection/snapshot.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/agent-connection/`snapshot.ts`/
symbols:
  createAgentConnectionState: createAgentConnectionState().
  createAgentConnectionResourceSnapshot: createAgentConnectionResourceSnapshot().
  createAgentConnectionCommands: createAgentConnectionCommands().
  createAgentConnectionSnapshot: createAgentConnectionSnapshot().
  createArtifactReference: createArtifactReference().
  toConnectionModel: toConnectionModel().
  createArtifactPathInfo: createArtifactPathInfo().
  createArtifactPathInfo.typeLiteral74.logicalPath: createArtifactPathInfo().typeLiteral74:logicalPath.
  persistedRecap: persistedRecap().
  createArtifactPathInfo.typeLiteral74.relativePath: createArtifactPathInfo().typeLiteral74:relativePath.
  persistedRecap.sessionManager-typeLiteral0.getLatestAgentStatus: persistedRecap().(sessionManager)typeLiteral0:getLatestAgentStatus.
  toPosixPath: toPosixPath().
---
# Module: [`packages/coding-agent/src/modes/agent-connection/snapshot.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts)

## Functions
- `createAgentConnectionCommands(session: AgentSession)` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L80)
- `createAgentConnectionResourceSnapshot(session: AgentSession)` — [`L105`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L105)
- `createAgentConnectionSnapshot(runtime: AgentSessionRuntime, activeSessionId?: string | undefined)` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L62)
- `createAgentConnectionState(runtime: AgentSessionRuntime, activeSessionId?: string | undefined)` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L22)
- `createArtifactPathInfo(filePath: string, cwd: string)` — [`L180`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L180)
- `createArtifactReference(session: AgentSession, type: AgentConnectionArtifactType, filePath: string | undefined)` — [`L161`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L161)
- `persistedRecap(sessionManager: { getLatestAgentStatus?: (() => { summary: string; } | undefined) | undefined; })` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L16)
- `toConnectionModel(model: Model<Api>)` — [`L155`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L155)
- `toPosixPath(path: string)` — [`L195`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L195)

## Module values
- `getLatestAgentStatus` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L17)
- `logicalPath` — [`L180`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L180)
- `relativePath` — [`L180`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/agent-connection/snapshot.ts#L180)

