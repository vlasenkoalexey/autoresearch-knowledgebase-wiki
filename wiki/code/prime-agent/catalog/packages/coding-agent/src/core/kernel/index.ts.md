---
title: 'Module: packages/coding-agent/src/core/kernel/index.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/kernel/index.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/kernel/`index.ts`/
symbols:
  KernelManager.executeInner: KernelManager#executeInner().
  KernelManager.doStart: KernelManager#doStart().
  KernelManager.resolveExecution: KernelManager#resolveExecution().
  KernelManager.execute: KernelManager#execute().
  KernelManager.handleExecutionMessage: KernelManager#handleExecutionMessage().
  KernelManager.snapshotState: KernelManager#snapshotState().
  ExecuteResult.status: ExecuteResult#status.
  KernelManager.-constructor: KernelManager#`<constructor>`().
  KernelManager.restoreState: KernelManager#restoreState().
  ExecuteResult.stdout: ExecuteResult#stdout.
  KernelManager.probeReady: KernelManager#probeReady().
  KernelManager.cleanupResources: KernelManager#cleanupResources().
  KernelManager.listNamespaceNames: KernelManager#listNamespaceNames().
  KernelManager.dispose: KernelManager#dispose().
  KernelManager.shutdown: KernelManager#shutdown().
  makeConnection: makeConnection().
  buildMessage: buildMessage().
  KernelSentAgentMessage: KernelSentAgentMessage#
  KernelManager: KernelManager#
  KernelManager.runIopubPump: KernelManager#runIopubPump().
  KernelManager.state: KernelManager#state.
  KernelManager.start: KernelManager#start().
  KernelManager.sendCommMessage: KernelManager#sendCommMessage().
  KernelManager.enqueueExecute: KernelManager#enqueueExecute().
  ExecuteResult.attachments: ExecuteResult#attachments.
  KernelManager.options: KernelManager#options.
  KernelManagerOptions.cwd: KernelManagerOptions#cwd.
  encode: encode().
  KernelManager.interrupt: KernelManager#interrupt().
  KernelManagerOptions.python: KernelManagerOptions#python.
  KernelManager.startForkedLivenessMonitor: KernelManager#startForkedLivenessMonitor().
  KernelManager.handleCommMessage: KernelManager#handleCommMessage().
  KernelManager.activeExecution: KernelManager#activeExecution.
  KernelManager.appendKernelDiagnostic: KernelManager#appendKernelDiagnostic().
  KernelManager.waitForResolvedConnection: KernelManager#waitForResolvedConnection().
  KernelManager.waitForActiveExecutionToClearForReuse: KernelManager#waitForActiveExecutionToClearForReuse().
  KernelManager.startHostRequestFromComm: KernelManager#startHostRequestFromComm().
  KernelManager.handleHostRequest: KernelManager#handleHostRequest().
  KernelManager.scheduleSnapshot: KernelManager#scheduleSnapshot().
  KernelManagerOptions.snapshot: KernelManagerOptions#snapshot.
  liveKernels: liveKernels.
  parseSentAgentMessage: parseSentAgentMessage().
  KernelManager.flushSnapshotForDispose: KernelManager#flushSnapshotForDispose().
  HostRequestHandlers: HostRequestHandlers#
  KernelManager.connection: KernelManager#connection.
  KernelManager.restart: KernelManager#restart().
  ActiveExecution.maxChars: ActiveExecution#maxChars.
  signalHandlersInstalled: signalHandlersInstalled.
  KernelManagerOptions.hostHandlers: KernelManagerOptions#hostHandlers.
  KernelSentAgentMessage.id: KernelSentAgentMessage#id.
  ExecuteResult: ExecuteResult#
  ActiveExecution.status: ActiveExecution#status.
  createDeferred: createDeferred().
  installSignalHandlersOnce: installSignalHandlersOnce().
  KernelManager.snapshotTimer: KernelManager#snapshotTimer.
  KernelManager.finishActiveExecution: KernelManager#finishActiveExecution().
  KernelManager.lateSentAgentMessageHandlers: KernelManager#lateSentAgentMessageHandlers.
  KernelManager.disposeSync: KernelManager#disposeSync().
  ExecuteOptions.signal: ExecuteOptions#signal.
  KernelAttachment.mimeType: KernelAttachment#mimeType.
  ExecuteResult.stderr: ExecuteResult#stderr.
  ExecuteResult.error: ExecuteResult#error.
  JupyterMessage.header: JupyterMessage#header.
  JupyterMessage.content: JupyterMessage#content.
  KernelManager.rejectActiveExecution: KernelManager#rejectActiveExecution().
  KernelAttachment: KernelAttachment#
  KernelAttachment.data: KernelAttachment#data.
  ActiveExecution.stderr: ActiveExecution#stderr.
  errorMessage: errorMessage().
  KernelManager.control: KernelManager#control.
  ExecuteResult.diffs: ExecuteResult#diffs.
  ExecuteResult.sentAgentMessages: ExecuteResult#sentAgentMessages.
  parseAttachmentDisplay: parseAttachmentDisplay().
  KernelManager.registerLateSentAgentMessageHandler: KernelManager#registerLateSentAgentMessageHandler().
  KernelManager.kill: KernelManager#kill().
  HostRequestHandler: HostRequestHandler#
  KernelManagerOptions.env: KernelManagerOptions#env.
  ConnectionInfo: ConnectionInfo#
  KernelManager.kernelPid: KernelManager#kernelPid.
  ActiveExecution.opts: ActiveExecution#opts.
  KernelManagerOptions.username: KernelManagerOptions#username.
  JupyterMessage.header.typeLiteral63.msg_type: JupyterMessage#header.typeLiteral63:msg_type.
  ActiveExecution.stdout: ActiveExecution#stdout.
  ActiveExecution.error: ActiveExecution#error.
  decode: decode().
  KernelManager.shell: KernelManager#shell.
  KernelManager.iopub: KernelManager#iopub.
  KernelManager.kernelStderr: KernelManager#kernelStderr.
  KernelManager.dispatchLateSentAgentMessage: KernelManager#dispatchLateSentAgentMessage().
  KernelManagerOptions.pythonSkills: KernelManagerOptions#pythonSkills.
  ActiveExecution.diffs: ActiveExecution#diffs.
  ActiveExecution.attachments: ActiveExecution#attachments.
  ActiveExecution.sentAgentMessages: ActiveExecution#sentAgentMessages.
  KernelManager.forkedKernelDied: KernelManager#forkedKernelDied().
  parseDiffDisplay: parseDiffDisplay().
  ConnectionInfo.key: ConnectionInfo#key.
  isRecord: isRecord().
  hasResolvedPorts: hasResolvedPorts().
  parseConnectionInfo: parseConnectionInfo().
  readConnectionInfo: readConnectionInfo().
  KernelManager.kernel: KernelManager#kernel.
  KernelManager.-get-ownerSessionId: KernelManager#`<get>ownerSessionId`().
  KernelManager.startIopubPump: KernelManager#startIopubPump().
  KernelManager.waitForActiveExecutionToClear: KernelManager#waitForActiveExecutionToClear().
  KernelBusyAfterInterruptError.-constructor: KernelBusyAfterInterruptError#`<constructor>`().
  KernelStartOptions.onBootstrapProgress: KernelStartOptions#onBootstrapProgress.
  KernelManagerOptions.sessionId: KernelManagerOptions#sessionId.
  AGENT_MESSAGE_DISPLAY_MIME: AGENT_MESSAGE_DISPLAY_MIME.
  KernelDiffDisplay: KernelDiffDisplay#
  KernelDiffDisplay.path: KernelDiffDisplay#path.
  KernelSentAgentMessage.target: KernelSentAgentMessage#target.
  KernelSentAgentMessage.target.typeLiteral10.sessionId: KernelSentAgentMessage#target.typeLiteral10:sessionId.
  JupyterMessage: JupyterMessage#
  KernelManager.session: KernelManager#session.
  KernelManager.forkedLivenessTimer: KernelManager#forkedLivenessTimer.
  KernelManager.tempDir: KernelManager#tempDir.
  KernelManager.startPromise: KernelManager#startPromise.
  KernelManager.-get-isRunning: KernelManager#`<get>isRunning`().
  ExecuteOptions.onLateSentAgentMessage: ExecuteOptions#onLateSentAgentMessage.
  ActiveExecution.resolve: ActiveExecution#resolve.
  KernelManager.notifyActiveExecutionIdle: KernelManager#notifyActiveExecutionIdle().
  KernelSnapshotConfig.path: KernelSnapshotConfig#path.
  ExecuteOptions: ExecuteOptions#
  ExecuteOptions.maxOutputChars: ExecuteOptions#maxOutputChars.
  ExecuteOptions.internal: ExecuteOptions#internal.
  KernelSentAgentMessage.deliveryStatus: KernelSentAgentMessage#deliveryStatus.
  KernelSentAgentMessage.target.typeLiteral10.activeSessionId: KernelSentAgentMessage#target.typeLiteral10:activeSessionId.
  KernelSentAgentMessage.target.typeLiteral10.sessionName: KernelSentAgentMessage#target.typeLiteral10:sessionName.
  ExecuteResult.result: ExecuteResult#result.
  ConnectionInfo.ip: ConnectionInfo#ip.
  ConnectionInfo.transport: ConnectionInfo#transport.
  JupyterMessage.parent_header: JupyterMessage#parent_header.
  ActiveExecution: ActiveExecution#
  ActiveExecution.settled: ActiveExecution#settled.
  makeConnection.typeLiteral123.path: makeConnection().typeLiteral123:path.
  makeConnection.typeLiteral123.tempDir: makeConnection().typeLiteral123:tempDir.
  KernelManager.iopubPumpPromise: KernelManager#iopubPumpPromise.
  KernelManager.executionQueue: KernelManager#executionQueue.
  KernelManager.activeExecutionIdleWaiters: KernelManager#activeExecutionIdleWaiters.
  KernelManager.resolveExecution.options-typeLiteral318.clearActive: KernelManager#resolveExecution().(options)typeLiteral318:clearActive.
  raceStartupWithAbort: raceStartupWithAbort().
  makeConnection.typeLiteral123.info: makeConnection().typeLiteral123:info.
  KernelManager.waitForHostRequestsToSettle: KernelManager#waitForHostRequestsToSettle().
  KernelManager.clearSnapshotTimer: KernelManager#clearSnapshotTimer().
  READY_TIMEOUT_MS: READY_TIMEOUT_MS.
  SNAPSHOT_MAX_OUTPUT_CHARS: SNAPSHOT_MAX_OUTPUT_CHARS.
  KernelBusyAfterInterruptError: KernelBusyAfterInterruptError#
  KernelManagerOptions: KernelManagerOptions#
  KernelSentAgentMessage.message: KernelSentAgentMessage#message.
  ExecuteResult.error.typeLiteral11.evalue: ExecuteResult#error.typeLiteral11:evalue.
  ExecuteResult.durationMs: ExecuteResult#durationMs.
  createKernelStartupAbortError: createKernelStartupAbortError().
  JupyterMessage.header.typeLiteral63.msg_id: JupyterMessage#header.typeLiteral63:msg_id.
  ActiveExecution.requestMsgId: ActiveExecution#requestMsgId.
  ActiveExecution.stdoutTruncated: ActiveExecution#stdoutTruncated.
  ActiveExecution.stderrTruncated: ActiveExecution#stderrTruncated.
  Deferred.promise: Deferred#promise.
  KernelManager.commTargets: KernelManager#commTargets.
  KernelManager.handledHostRequestCommIds: KernelManager#handledHostRequestCommIds.
  KernelManager.inFlightHostRequests: KernelManager#inFlightHostRequests.
  DELIM: DELIM.
  PORTS_RESOLVE_TIMEOUT_MS: PORTS_RESOLVE_TIMEOUT_MS.
  KERNEL_BUSY_REUSE_WAIT_MS: KERNEL_BUSY_REUSE_WAIT_MS.
  HOST_COMM_TARGET: HOST_COMM_TARGET.
  KernelStartOptions: KernelStartOptions#
  KernelStartOptions.signal: KernelStartOptions#signal.
  MAX_ATTACHMENT_DATA_CHARS: MAX_ATTACHMENT_DATA_CHARS.
  ExecuteResult.error.typeLiteral11.traceback: ExecuteResult#error.typeLiteral11:traceback.
  ConnectionInfo.shell_port: ConnectionInfo#shell_port.
  ConnectionInfo.iopub_port: ConnectionInfo#iopub_port.
  ConnectionInfo.control_port: ConnectionInfo#control_port.
  JupyterMessage.metadata: JupyterMessage#metadata.
  ActiveExecution.code: ActiveExecution#code.
  ActiveExecution.started: ActiveExecution#started.
  ActiveExecution.result: ActiveExecution#result.
  ActiveExecution.reject: ActiveExecution#reject.
  Deferred.resolve: Deferred#resolve.
  Deferred.reject: Deferred#reject.
  KernelManager.lastCellCode: KernelManager#lastCellCode.
  PROTOCOL_VERSION: PROTOCOL_VERSION.
  IOPUB_SUBSCRIBE_DELAY_MS: IOPUB_SUBSCRIBE_DELAY_MS.
  DEFAULT_MAX_OUTPUT_CHARS: DEFAULT_MAX_OUTPUT_CHARS.
  HOST_REQUEST_DISPOSE_TIMEOUT_MS: HOST_REQUEST_DISPOSE_TIMEOUT_MS.
  DEFAULT_SNAPSHOT_DEBOUNCE_MS: DEFAULT_SNAPSHOT_DEBOUNCE_MS.
  FORKED_LIVENESS_POLL_MS: FORKED_LIVENESS_POLL_MS.
  SNAPSHOT_DISPOSE_TIMEOUT_MS: SNAPSHOT_DISPOSE_TIMEOUT_MS.
  KERNEL_ABORT_GRACE_MS: KERNEL_ABORT_GRACE_MS.
  KERNEL_BUSY_INTERRUPT_INTERVAL_MS: KERNEL_BUSY_INTERRUPT_INTERVAL_MS.
  MAX_LATE_SENT_AGENT_MESSAGE_HANDLERS: MAX_LATE_SENT_AGENT_MESSAGE_HANDLERS.
  KERNEL_BUSY_AFTER_INTERRUPT_MESSAGE: KERNEL_BUSY_AFTER_INTERRUPT_MESSAGE.
  KernelSnapshotConfig: KernelSnapshotConfig#
  KernelSnapshotConfig.manifestPath: KernelSnapshotConfig#manifestPath.
  KernelSnapshotConfig.maxBytes: KernelSnapshotConfig#maxBytes.
  KernelSnapshotConfig.debounceMs: KernelSnapshotConfig#debounceMs.
  ExecuteOptions.onStream: ExecuteOptions#onStream.
  DIFF_DISPLAY_MIME: DIFF_DISPLAY_MIME.
  ATTACHMENT_DISPLAY_MIME: ATTACHMENT_DISPLAY_MIME.
  KernelDiffDisplay.oldStr: KernelDiffDisplay#oldStr.
  KernelDiffDisplay.newStr: KernelDiffDisplay#newStr.
  KernelDiffDisplay.startLine: KernelDiffDisplay#startLine.
  KernelAttachment.path: KernelAttachment#path.
  ExecuteResult.error.typeLiteral11.ename: ExecuteResult#error.typeLiteral11:ename.
  ConnectionInfo.stdin_port: ConnectionInfo#stdin_port.
  ConnectionInfo.hb_port: ConnectionInfo#hb_port.
  ConnectionInfo.signature_scheme: ConnectionInfo#signature_scheme.
  ConnectionInfo.kernel_name: ConnectionInfo#kernel_name.
  JupyterMessage.header.typeLiteral63.session: JupyterMessage#header.typeLiteral63:session.
  JupyterMessage.header.typeLiteral63.username: JupyterMessage#header.typeLiteral63:username.
  JupyterMessage.header.typeLiteral63.date: JupyterMessage#header.typeLiteral63:date.
  JupyterMessage.header.typeLiteral63.version: JupyterMessage#header.typeLiteral63:version.
  Deferred: Deferred#
  sign: sign().
  CONNECTION_PORT_KEYS: CONNECTION_PORT_KEYS.
  KernelManager.shutdown.opts-typeLiteral530.snapshot: KernelManager#shutdown().(opts)typeLiteral530:snapshot.
  KernelSentAgentMessage.receiverRole: KernelSentAgentMessage#receiverRole.
---
# Module: [`packages/coding-agent/src/core/kernel/index.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts)

## Classes
### `ActiveExecution`
- def: [`packages/coding-agent/src/core/kernel/index.ts:303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L303)
- signature: `interface ActiveExecution`
- members:
  - `attachments` — [`L316`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L316)
  - `code` — [`L306`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L306) — Source of the cell currently executing; surfaced to rlm.run spawns.
  - `diffs` — [`L315`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L315)
  - `error` — [`L318`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L318)
  - `maxChars` — [`L308`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L308)
  - `opts` — [`L309`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L309)
  - `reject` — [`L322`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L322)
  - `requestMsgId` — [`L304`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L304)
  - `resolve` — [`L321`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L321)
  - `result` — [`L314`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L314)
  - `sentAgentMessages` — [`L317`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L317)
  - `settled` — [`L320`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L320)
  - `started` — [`L307`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L307)
  - `status` — [`L319`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L319)
  - `stderr` — [`L311`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L311)
  - `stderrTruncated` — [`L313`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L313)
  - `stdout` — [`L310`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L310)
  - `stdoutTruncated` — [`L312`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L312)
- uses (calls/refs, reference-scoped): [`status`](index.ts.md#ExecuteResult.status), [`KernelSentAgentMessage`](index.ts.md#KernelSentAgentMessage), [`ExecuteResult`](index.ts.md#ExecuteResult), [`error`](index.ts.md#ExecuteResult.error), [`KernelAttachment`](index.ts.md#KernelAttachment), [`KernelDiffDisplay`](index.ts.md#KernelDiffDisplay), [`ExecuteOptions`](index.ts.md#ExecuteOptions)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`resolveExecution`](index.ts.md#KernelManager.resolveExecution), [`handleExecutionMessage`](index.ts.md#KernelManager.handleExecutionMessage), [`activeExecution`](index.ts.md#KernelManager.activeExecution), [`handleHostRequest`](index.ts.md#KernelManager.handleHostRequest), [`finishActiveExecution`](index.ts.md#KernelManager.finishActiveExecution), [`rejectActiveExecution`](index.ts.md#KernelManager.rejectActiveExecution)

### `ConnectionInfo`
- def: [`packages/coding-agent/src/core/kernel/index.ts:276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L276)
- signature: `interface ConnectionInfo`
- members:
  - `control_port` — [`L282`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L282)
  - `hb_port` — [`L283`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L283)
  - `iopub_port` — [`L280`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L280)
  - `ip` — [`L277`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L277)
  - `kernel_name` — [`L286`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L286)
  - `key` — [`L285`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L285)
  - `shell_port` — [`L279`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L279)
  - `signature_scheme` — [`L284`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L284)
  - `stdin_port` — [`L281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L281)
  - `transport` — [`L278`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L278)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`doStart`](index.ts.md#KernelManager.doStart), [`probeReady`](index.ts.md#KernelManager.probeReady), [`shutdown`](index.ts.md#KernelManager.shutdown), [`makeConnection`](index.ts.md#makeConnection), [`sendCommMessage`](index.ts.md#KernelManager.sendCommMessage), [`interrupt`](index.ts.md#KernelManager.interrupt), [`waitForResolvedConnection`](index.ts.md#KernelManager.waitForResolvedConnection), [`connection`](index.ts.md#KernelManager.connection), [`hasResolvedPorts`](index.ts.md#hasResolvedPorts), [`parseConnectionInfo`](index.ts.md#parseConnectionInfo), [`readConnectionInfo`](index.ts.md#readConnectionInfo), [`info`](index.ts.md#makeConnection.typeLiteral123.info)

### `Deferred`
- def: [`packages/coding-agent/src/core/kernel/index.ts:325`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L325)
- signature: `interface Deferred`
- members:
  - `promise` — [`L326`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L326)
  - `reject` — [`L328`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L328)
  - `resolve` — [`L327`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L327)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`createDeferred`](index.ts.md#createDeferred)

### `ExecuteOptions`
- def: [`packages/coding-agent/src/core/kernel/index.ts:98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L98)
- signature: `interface ExecuteOptions`
- members:
  - `internal` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L106) — Synthetic host cell (snapshot/restore/list); excluded from lastCellCode attribution.
  - `maxOutputChars` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L104) — Cap stdout / stderr / result at this many characters. Default 65536.
  - `onLateSentAgentMessage` — [`L102`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L102)
  - `onStream` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L101)
  - `signal` — [`L100`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L100) — Aborting interrupts the kernel via the control channel.
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](index.ts.md#KernelSentAgentMessage)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`resolveExecution`](index.ts.md#KernelManager.resolveExecution), [`execute`](index.ts.md#KernelManager.execute), [`handleExecutionMessage`](index.ts.md#KernelManager.handleExecutionMessage), [`snapshotState`](index.ts.md#KernelManager.snapshotState), [`restoreState`](index.ts.md#KernelManager.restoreState), [`listNamespaceNames`](index.ts.md#KernelManager.listNamespaceNames), [`enqueueExecute`](index.ts.md#KernelManager.enqueueExecute), [`opts`](index.ts.md#ActiveExecution.opts)

### `ExecuteResult`
- def: [`packages/coding-agent/src/core/kernel/index.ts:156`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L156)
- signature: `interface ExecuteResult`
- members:
  - `attachments` — [`L164`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L164) — Media attachments emitted via display_data, in order.
  - `diffs` — [`L162`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L162) — Diffs emitted via display_data, in order.
  - `durationMs` — [`L169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L169)
  - `ename` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L168)
  - `error` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L168)
  - `evalue` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L168)
  - `result` — [`L160`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L160) — Last `execute_result` payload (text/plain), if the cell produced one.
  - `sentAgentMessages` — [`L166`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L166) — Agent messages sent from this cell, in order.
  - `status` — [`L167`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L167) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `stderr` — [`L158`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L158)
  - `stdout` — [`L157`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L157) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `traceback` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L168)
- uses (calls/refs, reference-scoped): [`KernelSentAgentMessage`](index.ts.md#KernelSentAgentMessage), [`KernelAttachment`](index.ts.md#KernelAttachment), [`KernelDiffDisplay`](index.ts.md#KernelDiffDisplay)
- used by: [`createIpythonToolDefinition`](../tools/ipython.ts.md#createIpythonToolDefinition), [`executeInner`](index.ts.md#KernelManager.executeInner), [`startKernel`](../tools/ipython.ts.md#IpythonKernelProvisioner.startKernel), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`resolveExecution`](index.ts.md#KernelManager.resolveExecution), [`execute`](index.ts.md#KernelManager.execute), [`snapshotState`](index.ts.md#KernelManager.snapshotState), [`restoreState`](index.ts.md#KernelManager.restoreState), [`listNamespaceNames`](index.ts.md#KernelManager.listNamespaceNames), [`enqueueExecute`](index.ts.md#KernelManager.enqueueExecute), [`status`](index.ts.md#ActiveExecution.status), [`error`](index.ts.md#ActiveExecution.error), [`resolve`](index.ts.md#ActiveExecution.resolve), [`result`](../tools/ipython.ts.md#executeWithBusyKernelChoice.Promise.typeLiteral149.result)  (11 test-only)

### `HostRequestHandler`
- def: [`packages/coding-agent/src/core/kernel/index.ts:62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L62)
- doc: Handles one typed request from Python code running in the kernel.
- signature: `type HostRequestHandler`
- used by: [`agent-messages.ts`](../agent-messages.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-messages.ts), [`rlm-runtime.ts`](../rlm-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-rlm-runtime.ts), [`createAgentMessageHostHandlers`](../agent-messages.ts.md#createAgentMessageHostHandlers), [`createRlmRunHostHandler`](../rlm-runtime.ts.md#createRlmRunHostHandler), [`createRlmFindModelsHostHandler`](../rlm-runtime.ts.md#createRlmFindModelsHostHandler), [`createRlmDeleteSubagentHostHandler`](../rlm-runtime.ts.md#createRlmDeleteSubagentHostHandler), [`HostRequestHandlers`](index.ts.md#HostRequestHandlers), [`createRlmListSubagentsHostHandler`](../rlm-runtime.ts.md#createRlmListSubagentsHostHandler)

### `HostRequestHandlers`
- def: [`packages/coding-agent/src/core/kernel/index.ts:65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L65)
- doc: Host request handlers keyed by request type (e.g. "rlm.run", "goal.complete").
- signature: `type HostRequestHandlers`
- uses (calls/refs, reference-scoped): [`HostRequestHandler`](index.ts.md#HostRequestHandler)
- used by: [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_createKernelHostHandlers`](../agent-session.ts.md#AgentSession._createKernelHostHandlers), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`hostHandlers`](index.ts.md#KernelManagerOptions.hostHandlers), [`hostHandlers`](../tools/ipython.ts.md#IpythonToolOptions.hostHandlers)  (3 test-only)

### `JupyterMessage`
- def: [`packages/coding-agent/src/core/kernel/index.ts:289`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L289)
- signature: `interface JupyterMessage`
- members:
  - `content` — [`L300`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L300)
  - `date` — [`L294`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L294)
  - `header` — [`L290`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L290)
  - `metadata` — [`L299`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L299)
  - `msg_id` — [`L291`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L291)
  - `msg_type` — [`L295`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L295)
  - `parent_header` — [`L298`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L298)
  - `session` — [`L292`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L292)
  - `username` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L293)
  - `version` — [`L296`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L296)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`handleExecutionMessage`](index.ts.md#KernelManager.handleExecutionMessage), [`probeReady`](index.ts.md#KernelManager.probeReady), [`buildMessage`](index.ts.md#buildMessage), [`runIopubPump`](index.ts.md#KernelManager.runIopubPump), [`encode`](index.ts.md#encode), [`handleCommMessage`](index.ts.md#KernelManager.handleCommMessage), [`decode`](index.ts.md#decode)

### `KernelAttachment`
- def: [`packages/coding-agent/src/core/kernel/index.ts:136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L136)
- doc: One media attachment, captured from an {@link ATTACHMENT_DISPLAY_MIME} display payload.
- signature: `interface KernelAttachment`
- members:
  - `data` — [`L139`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L139) — base64-encoded bytes.
  - `mimeType` — [`L137`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L137)
  - `path` — [`L141`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L141) — Source path, surfaced to the TUI renderer.
- used by: [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`attachments`](index.ts.md#ExecuteResult.attachments), [`imageBlocksFromAttachments`](../tools/ipython.ts.md#imageBlocksFromAttachments), [`parseAttachmentDisplay`](index.ts.md#parseAttachmentDisplay), [`attachments`](index.ts.md#ActiveExecution.attachments), [`attachments`](../tools/ipython.ts.md#IpythonToolDetails.attachments)  (2 test-only)

### `KernelBusyAfterInterruptError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/kernel/index.ts:48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L48)
- signature: `class KernelBusyAfterInterruptError`
- members:
  - `<constructor>()` — [`L49`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L49)
- uses (calls/refs, reference-scoped): [`KERNEL_BUSY_AFTER_INTERRUPT_MESSAGE`](index.ts.md#KERNEL_BUSY_AFTER_INTERRUPT_MESSAGE)
- used by: [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`waitForActiveExecutionToClearForReuse`](index.ts.md#KernelManager.waitForActiveExecutionToClearForReuse), [`kernelRestarted`](../tools/ipython.ts.md#executeWithBusyKernelChoice.Promise.typeLiteral149.kernelRestarted)  (1 test-only)

### `KernelDiffDisplay`
- def: [`packages/coding-agent/src/core/kernel/index.ts:127`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L127)
- doc: One file edit, captured from a {@link DIFF_DISPLAY_MIME} display payload.
- signature: `interface KernelDiffDisplay`
- members:
  - `newStr` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L130)
  - `oldStr` — [`L129`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L129)
  - `path` — [`L128`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L128)
  - `startLine` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L132) — 1-based line where `oldStr` begins in the file, for absolute line numbers.
- used by: [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`isError`](../../modes/interactive/components/edit-summary.ts.md#getToolFileChanges.result-typeLiteral16.isError), [`diffs`](index.ts.md#ExecuteResult.diffs), [`diffs`](index.ts.md#ActiveExecution.diffs), [`parseDiffDisplay`](index.ts.md#parseDiffDisplay), [`diffs`](../tools/ipython.ts.md#IpythonToolDetails.diffs)  (1 test-only)

### `KernelManager`
- def: [`packages/coding-agent/src/core/kernel/index.ts:511`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L511)
- signature: `class KernelManager`
- members:
  - `<constructor>(options: KernelManagerOptions)` — [`L549`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L549)
  - `<get>isRunning` — [`L1526`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1526)
  - `<get>ownerSessionId` — [`L562`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L562)
  - `appendKernelDiagnostic(method)` — [`L566`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L566)
  - `cleanupResources(method)` — [`L1288`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1288) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `clearSnapshotTimer(method)` — [`L1477`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1477)
  - `dispatchLateSentAgentMessage(method)` — [`L1092`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1092)
  - `dispose(method)` — [`L1500`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1500) — Graceful cleanup. Waits briefly for in-flight host request handlers before closing sockets.
  - `disposeSync(method)` — [`L1519`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1519) — Synchronous best-effort cleanup. Safe to call from `process.on('exit')`.
  - `doStart(method)` — [`L583`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L583) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `enqueueExecute(method)` — [`L814`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L814) — Queue and run a cell, serializing against all other executions.
  - `execute(method)` — [`L803`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L803) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `executeInner(method)` — [`L845`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L845) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `finishActiveExecution(method)` — [`L1045`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1045)
  - `flushSnapshotForDispose(method)` — [`L1485`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1485) — Best-effort final snapshot before a graceful dispose, bounded by a timeout.
  - `forkedKernelDied(method)` — [`L733`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L733)
  - `handleCommMessage(method)` — [`L1189`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1189)
  - `handleExecutionMessage(method)` — [`L979`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L979) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `handleHostRequest(method)` — [`L1254`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1254)
  - `interrupt(method)` — [`L1282`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1282)
  - `kill(method)` — [`L1395`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1395)
  - `listNamespaceNames(method)` — [`L1445`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1445) — Live user-defined top-level names, or null if the kernel isn't running. Never throws.
  - `notifyActiveExecutionIdle(method)` — [`L1131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1131)
  - `probeReady(method)` — [`L767`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L767) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `registerLateSentAgentMessageHandler(method)` — [`L1107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1107)
  - `rejectActiveExecution(method)` — [`L1121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1121)
  - `resolveExecution(method)` — [`L1052`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1052) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `restart(method)` — [`L1377`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1377)
  - `restoreState(method)` — [`L1427`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1427) — Revive a previously snapshotted namespace into the kernel. Call right after
  - `runIopubPump(method)` — [`L950`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L950)
  - `scheduleSnapshot(method)` — [`L1464`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1464)
  - `sendCommMessage(method)` — [`L1273`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1273)
  - `shutdown(method)` — [`L1348`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1348) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `snapshotState(method)` — [`L1405`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1405) — Serialize the user namespace to disk (best-effort, per-variable). No-op when — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
  - `start(method)` — [`L570`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L570)
  - `startForkedLivenessMonitor(method)` — [`L718`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L718)
  - `startHostRequestFromComm(method)` — [`L1221`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1221)
  - `startIopubPump(method)` — [`L943`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L943)
  - `waitForActiveExecutionToClear(method)` — [`L1138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1138)
  - `waitForActiveExecutionToClearForReuse(method)` — [`L1168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1168)
  - `waitForHostRequestsToSettle(method)` — [`L1328`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1328)
  - `waitForResolvedConnection(method)` — [`L745`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L745)
  - `activeExecution` — [`L535`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L535)
  - `activeExecutionIdleWaiters` — [`L536`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L536)
  - `clearActive` — [`L1052`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1052)
  - `commTargets` — [`L518`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L518)
  - `connection` — [`L530`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L530)
  - `control` — [`L528`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L528)
  - `executionQueue` — [`L534`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L534) — Serializes execute() calls — Jupyter shell channel is request/reply.
  - `forkedLivenessTimer` — [`L525`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L525) — Polls a forked kernel's pid for death (no "exit" event on a non-child).
  - `handledHostRequestCommIds` — [`L519`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L519)
  - `inFlightHostRequests` — [`L542`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L542)
  - `iopub` — [`L527`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L527)
  - `iopubPumpPromise` — [`L529`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L529)
  - `kernel` — [`L520`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L520)
  - `kernelPid` — [`L523`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L523)
  - `kernelStderr` — [`L532`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L532)
  - `lastCellCode` — [`L541`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L541)
  - `lateSentAgentMessageHandlers` — [`L537`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L537)
  - `options` — [`L512`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L512)
  - `session` — [`L517`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L517)
  - `shell` — [`L526`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L526)
  - `snapshot` — [`L1348`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L1348)
  - `snapshotTimer` — [`L547`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L547) — Pending debounced auto-snapshot, if one has been scheduled.
  - `startPromise` — [`L545`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L545) — Memoized so concurrent callers all await the same in-flight startup.
  - `state` — [`L543`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L543)
  - `tempDir` — [`L531`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L531)
- uses (calls/refs, reference-scoped): [`status`](index.ts.md#ExecuteResult.status), [`ensureKernelPython`](bootstrap.ts.md#ensureKernelPython), [`stdout`](index.ts.md#ExecuteResult.stdout), [`forkKernel`](fork-server.ts.md#forkKernel), [`makeConnection`](index.ts.md#makeConnection), [`buildMessage`](index.ts.md#buildMessage), [`KernelSentAgentMessage`](index.ts.md#KernelSentAgentMessage), [`parseSnapshotResult`](state-snapshot.ts.md#parseSnapshotResult), [`parseRestoreResult`](state-snapshot.ts.md#parseRestoreResult), [`attachments`](index.ts.md#ExecuteResult.attachments), [`cwd`](index.ts.md#KernelManagerOptions.cwd), [`encode`](index.ts.md#encode), [`python`](index.ts.md#KernelManagerOptions.python), [`liveKernels`](index.ts.md#liveKernels), [`snapshot`](index.ts.md#KernelManagerOptions.snapshot), [`parseListNamesResult`](state-snapshot.ts.md#parseListNamesResult), [`parseSentAgentMessage`](index.ts.md#parseSentAgentMessage), [`RestoreResult`](state-snapshot.ts.md#RestoreResult), [`maxChars`](index.ts.md#ActiveExecution.maxChars), [`hostHandlers`](index.ts.md#KernelManagerOptions.hostHandlers), [`ExecuteResult`](index.ts.md#ExecuteResult), [`createDeferred`](index.ts.md#createDeferred), [`installSignalHandlersOnce`](index.ts.md#installSignalHandlersOnce), [`status`](index.ts.md#ActiveExecution.status), [`content`](index.ts.md#JupyterMessage.content), [`error`](index.ts.md#ExecuteResult.error), [`header`](index.ts.md#JupyterMessage.header), [`isForkServerEnabled`](fork-server.ts.md#isForkServerEnabled), [`signal`](index.ts.md#ExecuteOptions.signal), [`stderr`](index.ts.md#ExecuteResult.stderr), [`ForkServerUnavailable`](fork-server.ts.md#ForkServerUnavailable), [`buildRestoreCode`](state-snapshot.ts.md#buildRestoreCode), [`buildSnapshotCode`](state-snapshot.ts.md#buildSnapshotCode), [`errorMessage`](index.ts.md#errorMessage), [`stderr`](index.ts.md#ActiveExecution.stderr), [`diffs`](index.ts.md#ExecuteResult.diffs), [`parseAttachmentDisplay`](index.ts.md#parseAttachmentDisplay), [`sentAgentMessages`](index.ts.md#ExecuteResult.sentAgentMessages), [`ConnectionInfo`](index.ts.md#ConnectionInfo), [`env`](index.ts.md#KernelManagerOptions.env)  (+82 more)
- used by: [`startKernel`](../tools/ipython.ts.md#IpythonKernelProvisioner.startKernel), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`ensure`](../tools/ipython.ts.md#IpythonKernelProvisioner.ensure), [`dispose`](../tools/ipython.ts.md#IpythonKernelProvisioner.dispose), [`liveKernels`](index.ts.md#liveKernels), [`managerPromise`](../tools/ipython.ts.md#IpythonKernelProvisioner.managerPromise), [`kernelRestarted`](../tools/ipython.ts.md#executeWithBusyKernelChoice.Promise.typeLiteral149.kernelRestarted), [`kill`](../tools/ipython.ts.md#IpythonKernelProvisioner.kill), [`signalHandlersInstalled`](index.ts.md#signalHandlersInstalled), [`installSignalHandlersOnce`](index.ts.md#installSignalHandlersOnce), [`listNamespaceNames`](../tools/ipython.ts.md#IpythonKernelProvisioner.listNamespaceNames), [`startedManager`](../tools/ipython.ts.md#IpythonKernelProvisioner.startedManager), [`<get>manager`](../tools/ipython.ts.md#IpythonKernelProvisioner.-get-manager), [`<get>hasRunningKernel`](../tools/ipython.ts.md#IpythonKernelProvisioner.-get-hasRunningKernel), [`current`](../tools/ipython.ts.md#IpythonToolOptions.kernelManagerRef.typeLiteral55.current)  (12 test-only)

### `KernelManagerOptions`
- def: [`packages/coding-agent/src/core/kernel/index.ts:79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L79)
- signature: `interface KernelManagerOptions`
- members:
  - `cwd` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L82)
  - `env` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L83)
  - `hostHandlers` — [`L85`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L85)
  - `python` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L81) — Python interpreter that has `ipykernel` available. Defaults to the auto-bootstrapped kernel.
  - `pythonSkills` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L86)
  - `sessionId` — [`L84`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L84)
  - `snapshot` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L88) — Persist/revive the user namespace across kernel restarts and session resume.
  - `username` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L90) — Default: "prime-agent".
- uses (calls/refs, reference-scoped): [`HostRequestHandlers`](index.ts.md#HostRequestHandlers), [`KernelPythonSkill`](bootstrap.ts.md#KernelPythonSkill), [`KernelSnapshotConfig`](index.ts.md#KernelSnapshotConfig)
- used by: [`executeInner`](index.ts.md#KernelManager.executeInner), [`doStart`](index.ts.md#KernelManager.doStart), [`startKernel`](../tools/ipython.ts.md#IpythonKernelProvisioner.startKernel), [`snapshotState`](index.ts.md#KernelManager.snapshotState), [`<constructor>`](index.ts.md#KernelManager.-constructor), [`restoreState`](index.ts.md#KernelManager.restoreState), [`probeReady`](index.ts.md#KernelManager.probeReady), [`shutdown`](index.ts.md#KernelManager.shutdown), [`sendCommMessage`](index.ts.md#KernelManager.sendCommMessage), [`options`](index.ts.md#KernelManager.options), [`interrupt`](index.ts.md#KernelManager.interrupt), [`handleHostRequest`](index.ts.md#KernelManager.handleHostRequest), [`scheduleSnapshot`](index.ts.md#KernelManager.scheduleSnapshot), [`flushSnapshotForDispose`](index.ts.md#KernelManager.flushSnapshotForDispose), [`<get>ownerSessionId`](index.ts.md#KernelManager.-get-ownerSessionId)  (7 test-only)

### `KernelSentAgentMessage`
- def: [`packages/coding-agent/src/core/kernel/index.ts:144`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L144)
- signature: `interface KernelSentAgentMessage`
- members:
  - `activeSessionId` — [`L150`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L150)
  - `deliveryStatus` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L147)
  - `id` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L145)
  - `message` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L146)
  - `receiverRole` — [`L148`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L148)
  - `sessionId` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L151)
  - `sessionName` — [`L152`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L152)
  - `target` — [`L149`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L149)
- used by: [`interactive-mode.ts`](../../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`handleEvent`](../../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`acpUpdatesForSessionEvent`](../../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`types.ts`](../../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`tool-execution.ts`](../../modes/interactive/components/tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`AgentConnectionSessionEvent`](../../modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`isError`](../../modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent.updateResult.result-typeLiteral20.isError), [`AgentSessionEvent`](../agent-session.ts.md#AgentSessionEvent), [`appendSentAgentMessageToToolResult`](../agent-session.ts.md#appendSentAgentMessageToToolResult), [`parsePersistedIpythonSentAgentMessage`](../agent-session.ts.md#parsePersistedIpythonSentAgentMessage), [`_rememberLateIpythonSentAgentMessage`](../agent-session.ts.md#AgentSession._rememberLateIpythonSentAgentMessage), [`_recordLateIpythonSentAgentMessage`](../agent-session.ts.md#AgentSession._recordLateIpythonSentAgentMessage), [`appendSentAgentMessage`](../../modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent.appendSentAgentMessage), [`parseSentAgentMessage`](index.ts.md#parseSentAgentMessage), [`executeWithBusyKernelChoice`](../tools/ipython.ts.md#executeWithBusyKernelChoice), [`lateSentAgentMessageHandlers`](index.ts.md#KernelManager.lateSentAgentMessageHandlers), [`registerLateSentAgentMessageHandler`](index.ts.md#KernelManager.registerLateSentAgentMessageHandler), [`sentAgentMessages`](index.ts.md#ExecuteResult.sentAgentMessages), [`lateIpythonSentAgentMessages`](../../modes/interactive/interactive-mode.ts.md#InteractiveMode.lateIpythonSentAgentMessages), [`_lateIpythonSentAgentMessages`](../agent-session.ts.md#AgentSession._lateIpythonSentAgentMessages), [`sentAgentMessages`](index.ts.md#ActiveExecution.sentAgentMessages), [`pendingSentAgentMessages`](../../modes/interactive/components/tool-execution.ts.md#ToolExecutionComponent.pendingSentAgentMessages), [`onLateSentAgentMessage`](index.ts.md#ExecuteOptions.onLateSentAgentMessage), [`PersistedIpythonSentAgentMessage`](../agent-session.ts.md#PersistedIpythonSentAgentMessage), [`onLateSentAgentMessage`](../tools/ipython.ts.md#IpythonToolOptions.onLateSentAgentMessage), [`sentAgentMessages`](../tools/ipython.ts.md#IpythonToolDetails.sentAgentMessages)  (8 test-only)

### `KernelSnapshotConfig`
- def: [`packages/coding-agent/src/core/kernel/index.ts:68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L68)
- doc: Where and how to persist the kernel's user namespace so it survives resume.
- signature: `interface KernelSnapshotConfig`
- members:
  - `debounceMs` — [`L76`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L76) — Debounce window for the auto-snapshot after a successful execution. Default 1500 ms.
  - `manifestPath` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L72) — Absolute path for the JSON manifest written alongside the payload.
  - `maxBytes` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L74) — Skip variables (and abort the payload) above this many bytes. Default 256 MiB.
  - `path` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L70) — Absolute path for the dill payload.
- used by: [`snapshotState`](index.ts.md#KernelManager.snapshotState), [`restoreState`](index.ts.md#KernelManager.restoreState), [`scheduleSnapshot`](index.ts.md#KernelManager.scheduleSnapshot), [`snapshot`](index.ts.md#KernelManagerOptions.snapshot)

### `KernelStartOptions`
- def: [`packages/coding-agent/src/core/kernel/index.ts:93`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L93)
- signature: `interface KernelStartOptions`
- members:
  - `onBootstrapProgress` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L94)
  - `signal` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L95)
- uses (calls/refs, reference-scoped): [`KernelBootstrapProgressHandler`](bootstrap.ts.md#KernelBootstrapProgressHandler)
- used by: [`doStart`](index.ts.md#KernelManager.doStart), [`start`](index.ts.md#KernelManager.start)

## Functions
- `buildMessage(msgType: string, content: Record<string, unknown>, session: string, username: string)` — [`L351`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L351) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
- `createDeferred()` — [`L339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L339)
- `createKernelStartupAbortError()` — [`L232`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L232)
- `decode(frames: Buffer<ArrayBufferLike>[])` — [`L388`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L388)
- `encode(msg: JupyterMessage, key: string)` — [`L378`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L378)
- `errorMessage(error: unknown)` — [`L335`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L335)
- `hasResolvedPorts(info: ConnectionInfo)` — [`L408`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L408)
- `installSignalHandlersOnce()` — [`L483`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L483)
- `isRecord(value: unknown)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L331)
- `makeConnection()` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L451) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
- `parseAttachmentDisplay(payload: unknown)` — [`L190`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L190) — Parse an {@link ATTACHMENT_DISPLAY_MIME} payload. Malformed payloads are
- `parseConnectionInfo(value: unknown)` — [`L412`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L412)
- `parseDiffDisplay(payload: unknown)` — [`L173`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L173) — Parse a {@link DIFF_DISPLAY_MIME} payload, tolerating malformed input.
- `parseSentAgentMessage(payload: unknown)` — [`L204`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L204)
- `raceStartupWithAbort(promise: Promise<T>, signal: AbortSignal | undefined)` — [`L236`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L236)
- `readConnectionInfo(path: string)` — [`L443`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L443)
- `sign(parts: Buffer<ArrayBufferLike>[], key: string)` — [`L372`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L372)

## Module values
- `AGENT_MESSAGE_DISPLAY_MIME` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L116) — MIME tag the `agent-message` skill emits after sending a message.
- `ATTACHMENT_DISPLAY_MIME` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L113) — MIME tag the `attach-image` skill emits media payloads under, via `display_data`.
- `CONNECTION_PORT_KEYS` — [`L406`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L406)
- `DEFAULT_MAX_OUTPUT_CHARS` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L31)
- `DEFAULT_SNAPSHOT_DEBOUNCE_MS` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L33)
- `DELIM` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L25)
- `DIFF_DISPLAY_MIME` — [`L110`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L110) — MIME tag the `edit` skill emits diff payloads under, via `display_data`.
- `FORKED_LIVENESS_POLL_MS` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L35)
- `HOST_COMM_TARGET` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L56) — Comm target the kernel-side `rlm.host_request` shim opens for typed host requests.
- `HOST_REQUEST_DISPOSE_TIMEOUT_MS` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L32)
- `IOPUB_SUBSCRIBE_DELAY_MS` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L30)
- `KERNEL_ABORT_GRACE_MS` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L41)
- `KERNEL_BUSY_AFTER_INTERRUPT_MESSAGE` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L45)
- `KERNEL_BUSY_INTERRUPT_INTERVAL_MS` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L43)
- `KERNEL_BUSY_REUSE_WAIT_MS` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L42)
- `MAX_ATTACHMENT_DATA_CHARS` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L124) — Hard ceiling on a single attachment's base64 payload, a defensive guard
- `MAX_LATE_SENT_AGENT_MESSAGE_HANDLERS` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L44)
- `PORTS_RESOLVE_TIMEOUT_MS` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L27)
- `PROTOCOL_VERSION` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L26)
- `READY_TIMEOUT_MS` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L28)
- `SNAPSHOT_DISPOSE_TIMEOUT_MS` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L40)
- `SNAPSHOT_MAX_OUTPUT_CHARS` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L37)
- `info` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L451)
- `liveKernels` — [`L472`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L472)
- `path` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L451)
- `signalHandlersInstalled` — [`L473`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L473)
- `tempDir` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/index.ts#L451)

