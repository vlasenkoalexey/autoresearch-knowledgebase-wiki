---
title: 'Module: packages/coding-agent/src/core/context-tree.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/context-tree.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`context-tree.ts`/
symbols:
  loadContextTreeChildFromDisk: loadContextTreeChildFromDisk().
  computeOwnAndTotalUsage: computeOwnAndTotalUsage().
  computeContextUsageFromEntries: computeContextUsageFromEntries().
  isAssistantEntry: isAssistantEntry().
  sessionEntriesFromFile: sessionEntriesFromFile().
  ContextTreeNode: ContextTreeNode#
  loadContextTreeChildrenFromDisk: loadContextTreeChildrenFromDisk().
  ContextTreeNode.ownUsage: ContextTreeNode#ownUsage.
  ContextTreeNode.totalUsage: ContextTreeNode#totalUsage.
  ContextTreeNode.children: ContextTreeNode#children.
  ContextTreeNode.status: ContextTreeNode#status.
  ContextTreeNode.contextUsage: ContextTreeNode#contextUsage.
  ContextTreeNode.id: ContextTreeNode#id.
  statusFromBranch: statusFromBranch().
  ContextTreeNode.label: ContextTreeNode#label.
  branchEntries: branchEntries().
  ContextTreeNode.model: ContextTreeNode#model.
  computeOwnAndTotalUsage.typeLiteral40.ownUsage: computeOwnAndTotalUsage().typeLiteral40:ownUsage.
  ContextWindowResolver: ContextWindowResolver#
  computeOwnAndTotalUsage.typeLiteral40.totalUsage: computeOwnAndTotalUsage().typeLiteral40:totalUsage.
  ContextTreeNode.model.typeLiteral109.provider: ContextTreeNode#model.typeLiteral109:provider.
  ContextTreeNode.model.typeLiteral109.id: ContextTreeNode#model.typeLiteral109:id.
  readUserMessageText: readUserMessageText().
  compactLabel: compactLabel().
  findSessionFile: findSessionFile().
  listChildSessionDirs: listChildSessionDirs().
---
# Module: [`packages/coding-agent/src/core/context-tree.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts)

## Classes
### `ContextTreeNode`
- def: [`packages/coding-agent/src/core/context-tree.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L21)
- doc: One agent in the context overview: the main session or an RLM (sub-)agent.
- signature: `interface ContextTreeNode`
- members:
  - `children` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L30)
  - `contextUsage` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L29)
  - `id` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L23) — "root" for the session itself, the RLM child node id (sub-xxxx) otherwise.
  - `id` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L26)
  - `label` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L24)
  - `model` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L26)
  - `ownUsage` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L27)
  - `provider` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L26)
  - `status` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L25)
  - `totalUsage` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L28)
- uses (calls/refs, reference-scoped): [`Usage`](../../../ai/src/types.ts.md#Usage), [`ContextUsage`](extensions/types.ts.md#ContextUsage), [`RlmChildAgentStatus`](agent-session.ts.md#RlmChildAgentStatus)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`daemon-agent-connection.ts`](../modes/agent-connection/daemon-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-daemon-agent-connection.ts), [`in-process-agent-connection.ts`](../modes/agent-connection/in-process-agent-connection.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-in-process-agent-connection.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`formatContextTree`](../modes/interactive/components/context-tree-format.ts.md#formatContextTree), [`getContextTree`](agent-session.ts.md#AgentSession.getContextTree), [`context-tree-format.ts`](../modes/interactive/components/context-tree-format.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-context-tree-format.ts), [`loadContextTreeChildrenFromDisk`](context-tree.ts.md#loadContextTreeChildrenFromDisk), [`sumOwnUsage`](../modes/interactive/components/context-tree-format.ts.md#sumOwnUsage), [`flattenContextTree`](../modes/interactive/components/context-tree-format.ts.md#flattenContextTree), [`node`](../modes/interactive/components/context-tree-format.ts.md#ContextTreeRow.node), [`statusIcon`](../modes/interactive/components/context-tree-format.ts.md#statusIcon), [`countNodes`](../modes/interactive/components/context-tree-format.ts.md#countNodes), [`getContextTree`](../modes/agent-connection/types.ts.md#AgentConnection.getContextTree), [`getContextTree`](../modes/agent-connection/in-process-agent-connection.ts.md#InProcessAgentConnection.getContextTree), [`getContextTree`](../modes/agent-connection/daemon-agent-connection.ts.md#DaemonAgentConnection.getContextTree)  (1 test-only)

### `ContextWindowResolver`
- def: [`packages/coding-agent/src/core/context-tree.ts:11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L11)
- doc: Resolves a model's context window so disk-only nodes can report utilization.
- signature: `type ContextWindowResolver`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`loadContextTreeChildrenFromDisk`](context-tree.ts.md#loadContextTreeChildrenFromDisk), [`_contextWindowResolver`](agent-session.ts.md#AgentSession._contextWindowResolver)

## Functions
- `branchEntries(entries: SessionEntry[])` — [`L164`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L164) — Entries on the current branch, root to leaf, mirroring
- `compactLabel(text: string, maxLength?: number)` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L60) — Compact a prompt into a one-line label, mirroring compactRlmText in agent-session.ts.
- `computeContextUsageFromEntries(allEntries: SessionEntry[], branch: SessionEntry[], contextWindow: number | undefined)` — [`L109`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L109) — Current context utilization from persisted entries, mirroring
- `computeOwnAndTotalUsage(branch: SessionEntry[], allEntries: SessionEntry[])` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L81) — Usage totals for one agent: `totalUsage` sums the branch's assistant usage
- `findSessionFile(dir: string)` — [`L201`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L201)
- `isAssistantEntry(entry: SessionEntry)` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L33)
- `listChildSessionDirs(rlmSessionDir: string)` — [`L220`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L220)
- `loadContextTreeChildFromDisk(childSessionDir: string, resolveContextWindow: ContextWindowResolver)` — [`L253`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L253) — Build a context node for a completed RLM child from its persisted session
- `loadContextTreeChildrenFromDisk(rlmSessionDir: string | undefined, resolveContextWindow: ContextWindowResolver, skipIds?: ReadonlySet<string> | undefined)` — [`L305`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L305) — Build context nodes for all persisted RLM children under an RLM session
- `readUserMessageText(content: unknown)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L40)
- `sessionEntriesFromFile(file: string)` — [`L154`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L154)
- `statusFromBranch(entries: SessionEntry[])` — [`L184`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L184) — Terminal status for a persisted child, inferred from how its last assistant

## Module values
- `ownUsage` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L84)
- `totalUsage` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/context-tree.ts#L84)

