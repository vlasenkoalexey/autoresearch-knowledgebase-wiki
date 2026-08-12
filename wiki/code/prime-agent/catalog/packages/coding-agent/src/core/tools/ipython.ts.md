---
title: 'Module: packages/coding-agent/src/core/tools/ipython.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/ipython.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`ipython.ts`/
symbols:
  createIpythonToolDefinition: createIpythonToolDefinition().
  IpythonKernelProvisioner.startKernel: IpythonKernelProvisioner#startKernel().
  IpythonKernelProvisioner.ensure: IpythonKernelProvisioner#ensure().
  IpythonKernelProvisioner.-constructor: IpythonKernelProvisioner#`<constructor>`().
  applyShellSettingsToBashMagicCell: applyShellSettingsToBashMagicCell().
  IpythonKernelProvisioner.dispose: IpythonKernelProvisioner#dispose().
  createIpythonTool: createIpythonTool().
  IpythonKernelProvisioner: IpythonKernelProvisioner#
  imageBlocksFromAttachments: imageBlocksFromAttachments().
  chooseBusyKernelAction: chooseBusyKernelAction().
  buildRlmBootstrapCode: buildRlmBootstrapCode().
  IpythonKernelProvisioner.managerPromise: IpythonKernelProvisioner#managerPromise.
  IpythonKernelProvisioner.kill: IpythonKernelProvisioner#kill().
  executeWithBusyKernelChoice.Promise.typeLiteral149.kernelRestarted: executeWithBusyKernelChoice().Promise:typeLiteral149:kernelRestarted.
  executeWithBusyKernelChoice: executeWithBusyKernelChoice().
  IpythonKernelProvisioner.listNamespaceNames: IpythonKernelProvisioner#listNamespaceNames().
  IpythonKernelProvisioner.startedManager: IpythonKernelProvisioner#startedManager.
  IpythonKernelProvisioner.-get-manager: IpythonKernelProvisioner#`<get>manager`().
  IpythonKernelProvisioner.emitStartupProgress: IpythonKernelProvisioner#emitStartupProgress().
  setWorkingMessage: setWorkingMessage().
  IpythonToolOptions: IpythonToolOptions#
  IpythonToolOptions.kernelManagerRef: IpythonToolOptions#kernelManagerRef.
  IpythonToolDetails: IpythonToolDetails#
  IpythonKernelProvisioner.-get-hasRunningKernel: IpythonKernelProvisioner#`<get>hasRunningKernel`().
  IpythonKernelProvisioner.settleStartup: IpythonKernelProvisioner#settleStartup().
  IpythonToolInput: IpythonToolInput#
  IpythonToolOptions.kernelManagerRef.typeLiteral55.current: IpythonToolOptions#kernelManagerRef.typeLiteral55:current.
  IpythonKernelProvisioner.startupListeners: IpythonKernelProvisioner#startupListeners.
  IpythonKernelProvisioner.prewarm: IpythonKernelProvisioner#prewarm().
  createLinkedAbortSignal: createLinkedAbortSignal().
  raceWithAbort: raceWithAbort().
  IpythonToolDetails.status: IpythonToolDetails#status.
  IpythonKernelProvisioner.-get-lastRestore: IpythonKernelProvisioner#`<get>lastRestore`().
  IpythonToolDetails.diffs: IpythonToolDetails#diffs.
  IpythonToolOptions.pythonSkills: IpythonToolOptions#pythonSkills.
  IpythonKernelProvisioner._lastRestore: IpythonKernelProvisioner#_lastRestore.
  ipythonSchema: ipythonSchema.
  IpythonKernelProvisioner.lastStartupMessage: IpythonKernelProvisioner#lastStartupMessage.
  IpythonToolDetails.attachments: IpythonToolDetails#attachments.
  IpythonToolDetails.sentAgentMessages: IpythonToolDetails#sentAgentMessages.
  IpythonToolOptions.hostHandlers: IpythonToolOptions#hostHandlers.
  IpythonToolOptions.onRestore: IpythonToolOptions#onRestore.
  IpythonToolOptions.onLateSentAgentMessage: IpythonToolOptions#onLateSentAgentMessage.
  IpythonToolOptions.provisioner: IpythonToolOptions#provisioner.
  executeWithBusyKernelChoice.Promise.typeLiteral149.result: executeWithBusyKernelChoice().Promise:typeLiteral149:result.
  createAbortError: createAbortError().
  IpythonToolDetails.kernelRestarted: IpythonToolDetails#kernelRestarted.
  RLM_BOOTSTRAP_BASE_CODE: RLM_BOOTSTRAP_BASE_CODE.
  BUSY_KERNEL_WAIT_CHOICE: BUSY_KERNEL_WAIT_CHOICE.
  BUSY_KERNEL_KILL_CHOICE: BUSY_KERNEL_KILL_CHOICE.
  KERNEL_RESTART_NOTICE: KERNEL_RESTART_NOTICE.
  createLinkedAbortSignal.typeLiteral35.signal: createLinkedAbortSignal().typeLiteral35:signal.
  createLinkedAbortSignal.typeLiteral35.cleanup: createLinkedAbortSignal().typeLiteral35:cleanup.
  IpythonToolOptions.readyGate: IpythonToolOptions#readyGate.
  IpythonKernelProvisioner.disposeController: IpythonKernelProvisioner#disposeController.
  BUSY_KERNEL_PROMPT: BUSY_KERNEL_PROMPT.
  IpythonToolDetails.durationMs: IpythonToolDetails#durationMs.
  IpythonToolDetails.errorEname: IpythonToolDetails#errorEname.
  IpythonToolDetails.stdout: IpythonToolDetails#stdout.
  IpythonToolDetails.stderr: IpythonToolDetails#stderr.
  IpythonToolDetails.result: IpythonToolDetails#result.
  IpythonToolDetails.error: IpythonToolDetails#error.
  IpythonToolOptions.python: IpythonToolOptions#python.
  IpythonToolOptions.env: IpythonToolOptions#env.
  IpythonToolOptions.commandPrefix: IpythonToolOptions#commandPrefix.
  IpythonToolOptions.shellPath: IpythonToolOptions#shellPath.
  IpythonToolOptions.sessionId: IpythonToolOptions#sessionId.
  IpythonToolOptions.snapshotDir: IpythonToolOptions#snapshotDir.
  quoteScriptMagicArgument: quoteScriptMagicArgument().
  IpythonToolDetails.error.typeLiteral54.ename: IpythonToolDetails#error.typeLiteral54:ename.
  IpythonToolDetails.error.typeLiteral54.evalue: IpythonToolDetails#error.typeLiteral54:evalue.
  IpythonToolDetails.error.typeLiteral54.traceback: IpythonToolDetails#error.typeLiteral54:traceback.
---
# Module: [`packages/coding-agent/src/core/tools/ipython.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts)

## Classes
### `IpythonKernelProvisioner`
- def: [`packages/coding-agent/src/core/tools/ipython.ts:329`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L329)
- doc: Owns the lazy create+start+runtime-bootstrap of one session's IPython kernel.
- signature: `class IpythonKernelProvisioner`
- members:
  - `<constructor>(cwd: string, options?: Omit<IpythonToolOptions, "provisioner"> | undefined)` — [`L337`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L337) — Owns the lazy create+start+runtime-bootstrap of one session's IPython kernel.
  - `<get>hasRunningKernel` — [`L362`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L362) — Whether a kernel has finished starting and is currently running.
  - `<get>lastRestore` — [`L352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L352) — Result of reviving a prior session's namespace on the last kernel start, if any.
  - `<get>manager` — [`L347`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L347) — The kernel manager, once a startup has completed successfully.
  - `dispose(method)` — [`L373`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L373) — Dispose the kernel owned by this provisioner, including one still starting up.
  - `emitStartupProgress(method)` — [`L456`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L456)
  - `ensure(method)` — [`L409`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L409)
  - `kill(method)` — [`L393`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L393)
  - `listNamespaceNames(method)` — [`L367`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L367) — Live user-defined names in the kernel namespace, or null if listing failed / no kernel.
  - `prewarm(method)` — [`L357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L357) — Start the kernel in the background. Failures are swallowed here and surface on the next ensure().
  - `settleStartup(method)` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L451)
  - `startKernel(method)` — [`L463`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L463)
  - `disposeController` — [`L335`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L335)
  - `lastStartupMessage` — [`L333`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L333)
  - `managerPromise` — [`L330`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L330)
  - `startedManager` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L331)
  - `startupListeners` — [`L332`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L332)
- protocol/private: `_lastRestore`[`L334`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L334)
- uses (calls/refs, reference-scoped): [`execute`](../kernel/index.ts.md#KernelManager.execute), [`status`](../kernel/index.ts.md#ExecuteResult.status), [`<constructor>`](../kernel/index.ts.md#KernelManager.-constructor), [`restoreState`](../kernel/index.ts.md#KernelManager.restoreState), [`dispose`](../kernel/index.ts.md#KernelManager.dispose), [`listNamespaceNames`](../kernel/index.ts.md#KernelManager.listNamespaceNames), [`KernelManager`](../kernel/index.ts.md#KernelManager), [`start`](../kernel/index.ts.md#KernelManager.start), [`cwd`](../kernel/index.ts.md#KernelManagerOptions.cwd), [`python`](../kernel/index.ts.md#KernelManagerOptions.python), [`buildRlmBootstrapCode`](ipython.ts.md#buildRlmBootstrapCode), [`snapshot`](../kernel/index.ts.md#KernelManagerOptions.snapshot), [`RestoreResult`](../kernel/state-snapshot.ts.md#RestoreResult), [`withKernelBootPermit`](../kernel/boot-gate.ts.md#withKernelBootPermit), [`hostHandlers`](../kernel/index.ts.md#KernelManagerOptions.hostHandlers), [`snapshotPathIn`](../kernel/state-snapshot.ts.md#snapshotPathIn), [`KernelBootstrapProgressHandler`](../kernel/bootstrap.ts.md#KernelBootstrapProgressHandler), [`error`](../kernel/index.ts.md#ExecuteResult.error), [`stderr`](../kernel/index.ts.md#ExecuteResult.stderr), [`kill`](../kernel/index.ts.md#KernelManager.kill), [`IpythonToolOptions`](ipython.ts.md#IpythonToolOptions), [`env`](../kernel/index.ts.md#KernelManagerOptions.env), [`kernelManagerRef`](ipython.ts.md#IpythonToolOptions.kernelManagerRef), [`current`](ipython.ts.md#IpythonToolOptions.kernelManagerRef.typeLiteral55.current), [`manifestPathIn`](../kernel/state-snapshot.ts.md#manifestPathIn), [`pythonSkills`](../kernel/index.ts.md#KernelManagerOptions.pythonSkills), [`createLinkedAbortSignal`](ipython.ts.md#createLinkedAbortSignal), [`raceWithAbort`](ipython.ts.md#raceWithAbort), [`<get>isRunning`](../kernel/index.ts.md#KernelManager.-get-isRunning), [`sessionId`](../kernel/index.ts.md#KernelManagerOptions.sessionId), [`pythonSkills`](ipython.ts.md#IpythonToolOptions.pythonSkills), [`hostHandlers`](ipython.ts.md#IpythonToolOptions.hostHandlers), [`onRestore`](ipython.ts.md#IpythonToolOptions.onRestore), [`createAbortError`](ipython.ts.md#createAbortError), [`cleanup`](ipython.ts.md#createLinkedAbortSignal.typeLiteral35.cleanup), [`readyGate`](ipython.ts.md#IpythonToolOptions.readyGate), [`signal`](ipython.ts.md#createLinkedAbortSignal.typeLiteral35.signal), [`traceback`](../kernel/index.ts.md#ExecuteResult.error.typeLiteral11.traceback), [`env`](ipython.ts.md#IpythonToolOptions.env), [`python`](ipython.ts.md#IpythonToolOptions.python)  (+2 more)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`createIpythonToolDefinition`](ipython.ts.md#createIpythonToolDefinition), [`_buildRuntime`](../agent-session.ts.md#AgentSession._buildRuntime), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`_notifyKernelStateAfterCompaction`](../agent-session.ts.md#AgentSession._notifyKernelStateAfterCompaction), [`_disposeAsyncOnce`](../agent-session.ts.md#AgentSession._disposeAsyncOnce), [`kernelRestarted`](ipython.ts.md#executeWithBusyKernelChoice.Promise.typeLiteral149.kernelRestarted), [`executeWithBusyKernelChoice`](ipython.ts.md#executeWithBusyKernelChoice), [`_ipythonKernelProvisioner`](../agent-session.ts.md#AgentSession._ipythonKernelProvisioner), [`provisioner`](ipython.ts.md#IpythonToolOptions.provisioner)  (7 test-only)

### `IpythonToolDetails`
- def: [`packages/coding-agent/src/core/tools/ipython.ts:248`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L248)
- signature: `interface IpythonToolDetails`
- members:
  - `attachments` — [`L258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L258) — Media attachments loaded into context (e.g. by the attach-image skill).
  - `diffs` — [`L256`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L256) — Diffs streamed from file edits, rendered by the IPython cell.
  - `durationMs` — [`L249`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L249)
  - `ename` — [`L264`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L264)
  - `error` — [`L263`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L263)
  - `errorEname` — [`L251`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L251)
  - `evalue` — [`L265`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L265)
  - `kernelRestarted` — [`L262`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L262) — True when this result came after killing and restarting a busy kernel.
  - `result` — [`L254`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L254)
  - `sentAgentMessages` — [`L260`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L260) — Agent messages sent from this cell.
  - `status` — [`L250`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L250)
  - `stderr` — [`L253`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L253)
  - `stdout` — [`L252`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L252)
  - `traceback` — [`L266`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L266)
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](../kernel/index.ts.md#KernelSentAgentMessage), [`KernelAttachment`](../kernel/index.ts.md#KernelAttachment), [`KernelDiffDisplay`](../kernel/index.ts.md#KernelDiffDisplay)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createIpythonToolDefinition`](ipython.ts.md#createIpythonToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`edit-summary.ts`](../../modes/interactive/components/edit-summary.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-edit-summary.ts), [`isError`](../../modes/interactive/components/edit-summary.ts.md#getToolFileChanges.result-typeLiteral16.isError), [`IpythonToolResultEvent`](../extensions/types.ts.md#IpythonToolResultEvent)  (1 test-only)

### `IpythonToolInput`
- def: [`packages/coding-agent/src/core/tools/ipython.ts:246`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L246)
- signature: `type IpythonToolInput`
- uses (calls/refs, reference-scoped): [`ipythonSchema`](ipython.ts.md#ipythonSchema)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`IpythonToolCallEvent`](../extensions/types.ts.md#IpythonToolCallEvent)

### `IpythonToolOptions`
- def: [`packages/coding-agent/src/core/tools/ipython.ts:270`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L270)
- signature: `interface IpythonToolOptions`
- members:
  - `commandPrefix` — [`L275`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L275) — Command prefix prepended to every %%bash cell.
  - `current` — [`L288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L288)
  - `env` — [`L273`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L273)
  - `hostHandlers` — [`L280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L280) — Typed host request handlers for the kernel↔host bridge (rlm.run, goal.*, …).
  - `kernelManagerRef` — [`L288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L288) — Filled with the live KernelManager after the first kernel start; cleared on construction.
  - `onLateSentAgentMessage` — [`L294`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L294)
  - `onRestore` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L293) — Fires once per kernel start when a previous session's namespace was revived
  - `provisioner` — [`L296`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L296) — Shared provisioner owning the kernel lifecycle. When provided, the remaining options are ignored.
  - `python` — [`L272`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L272) — Python override. Must have `ipykernel` installed.
  - `pythonSkills` — [`L281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L281)
  - `readyGate` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L286) — Resolves before this kernel starts — e.g. the previous provisioner's dispose, so a
  - `sessionId` — [`L278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L278)
  - `shellPath` — [`L277`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L277) — Optional explicit shell path for bare %%bash cells.
  - `snapshotDir` — [`L283`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L283) — Per-session artifact dir where the kernel namespace snapshot is stored. Omit to disable snapshots.
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](../kernel/index.ts.md#KernelSentAgentMessage), [`KernelManager`](../kernel/index.ts.md#KernelManager), [`IpythonKernelProvisioner`](ipython.ts.md#IpythonKernelProvisioner), [`PythonSkillRuntimeInfo`](../skills.ts.md#PythonSkillRuntimeInfo), [`HostRequestHandlers`](../kernel/index.ts.md#HostRequestHandlers), [`RestoreResult`](../kernel/state-snapshot.ts.md#RestoreResult)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createIpythonToolDefinition`](ipython.ts.md#createIpythonToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`startKernel`](ipython.ts.md#IpythonKernelProvisioner.startKernel), [`<constructor>`](ipython.ts.md#IpythonKernelProvisioner.-constructor), [`applyShellSettingsToBashMagicCell`](ipython.ts.md#applyShellSettingsToBashMagicCell), [`dispose`](ipython.ts.md#IpythonKernelProvisioner.dispose), [`createIpythonTool`](ipython.ts.md#createIpythonTool), [`kill`](ipython.ts.md#IpythonKernelProvisioner.kill), [`ToolsOptions`](index.ts.md#ToolsOptions)

## Functions
- `applyShellSettingsToBashMagicCell(code: string, options: Pick<IpythonToolOptions, "shellPath" | "commandPrefix"> | undefined)` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L303)
- `buildRlmBootstrapCode(pythonSkills?: readonly PythonSkillRuntimeInfo[])` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L70)
- `chooseBusyKernelAction(ctx: ExtensionContext | undefined, signal: AbortSignal | undefined)` — [`L547`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L547)
- `createAbortError()` — [`L163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L163)
- `createIpythonTool(cwd: string, options?: IpythonToolOptions | undefined)` — [`L706`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L706)
- `createIpythonToolDefinition(cwd: string, options?: IpythonToolOptions | undefined)` — [`L619`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L619)
- `createLinkedAbortSignal(sources: readonly (AbortSignal | undefined)[])` — [`L209`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L209)
- `executeWithBusyKernelChoice(provisioner: IpythonKernelProvisioner, reportStartupProgress: KernelBootstrapProgressHandler, toolCallId: string, code: string, signal: AbortSignal | undefined, onStream: (chunk: string, name: "stdout" | "stderr") => void, onWorkingMessage: (message?: string | undefined) => void, onLateSentAgentMessage: ((toolCallId: string, message: KernelSentAgentMessage) => void) | undefined, ctx: ExtensionContext | undefined)` — [`L566`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L566)
- `imageBlocksFromAttachments(attachments: readonly KernelAttachment[] | undefined)` — [`L612`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L612) — Turn kernel image attachments into `ImageContent` blocks; non-image types are dropped.
- `quoteScriptMagicArgument(value: string)` — [`L299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L299)
- `raceWithAbort(promise: Promise<T>, signal: AbortSignal | undefined, onAbort?: (() => void) | undefined)` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L167)
- `setWorkingMessage(ctx: ExtensionContext | undefined, message?: string | undefined)` — [`L238`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L238)

## Module values
- `BUSY_KERNEL_KILL_CHOICE` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L151)
- `BUSY_KERNEL_PROMPT` — [`L152`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L152)
- `BUSY_KERNEL_WAIT_CHOICE` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L150)
- `KERNEL_RESTART_NOTICE` — [`L157`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L157)
- `RLM_BOOTSTRAP_BASE_CODE` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L24)
- `cleanup` — [`L211`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L211)
- `ipythonSchema` — [`L143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L143)
- `kernelRestarted` — [`L576`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L576)
- `result` — [`L576`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L576)
- `signal` — [`L210`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/ipython.ts#L210)

