---
title: 'Module: packages/coding-agent/src/cli/daemon-command.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-command.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-command.ts`/
symbols:
  parseSessionOption: parseSessionOption().
  runOpen: runOpen().
  runDaemonClientCommand: runDaemonClientCommand().
  parseSessionArgs: parseSessionArgs().
  DaemonAttachTerminal.handleMessage: DaemonAttachTerminal#handleMessage().
  isSessionSummary: isSessionSummary().
  DaemonAttachTerminal.writeLine: DaemonAttachTerminal#writeLine().
  runCreate: runCreate().
  handleDaemonCommand: handleDaemonCommand().
  DaemonAttachTerminal.handleSessionEvent: DaemonAttachTerminal#handleSessionEvent().
  ParsedDaemonClientCommand.positionals: ParsedDaemonClientCommand#positionals.
  printResponseData: printResponseData().
  runJsonAttach: runJsonAttach().
  runPrompt: runPrompt().
  runSend: runSend().
  runStart: runStart().
  runList: runList().
  runRename: runRename().
  runCron: runCron().
  DaemonAttachTerminal.run: DaemonAttachTerminal#run().
  DaemonAttachTerminal.handleInput: DaemonAttachTerminal#handleInput().
  getMessageRole: getMessageRole().
  createDaemonMessageWaiter: createDaemonMessageWaiter().
  parseDaemonClientCommand: parseDaemonClientCommand().
  resolveLiveSessionSelector: resolveLiveSessionSelector().
  requireSuccess: requireSuccess().
  ParsedDaemonClientCommand.json: ParsedDaemonClientCommand#json.
  DaemonAttachTerminal.rl: DaemonAttachTerminal#rl.
  DaemonAttachTerminal.printMessage: DaemonAttachTerminal#printMessage().
  getLiveSessions: getLiveSessions().
  parseExtensionFlagOption: parseExtensionFlagOption().
  runPsCommand: runPsCommand().
  printJson: printJson().
  parseSendArgs: parseSendArgs().
  canConnectToDaemon: canConnectToDaemon().
  isLiveSessionSummary: isLiveSessionSummary().
  ParsedDaemonClientCommand.socketPath: ParsedDaemonClientCommand#socketPath.
  resolvePathOption: resolvePathOption().
  requireActiveSessionId: requireActiveSessionId().
  runAttach: runAttach().
  runMessageCommand: runMessageCommand().
  requireSuccessAsync: requireSuccessAsync().
  DaemonAttachTerminal.printTranscript: DaemonAttachTerminal#printTranscript().
  runAgentMessages: runAgentMessages().
  waitForSessionEnd: waitForSessionEnd().
  waitForSessionClose: waitForSessionClose().
  waitUntilInterrupted: waitUntilInterrupted().
  nextDefaultSessionName: nextDefaultSessionName().
  getSessionSummaries: getSessionSummaries().
  ParsedSessionArgs.config: ParsedSessionArgs#config.
  ParsedDaemonClientCommand.command: ParsedDaemonClientCommand#command.
  runShutdown: runShutdown().
  ParsedSessionOption: ParsedSessionOption#
  ParsedSessionOption.consumed: ParsedSessionOption#consumed.
  ParsedSessionOption.daemonArg: ParsedSessionOption#daemonArg.
  findSessionCwdArg: findSessionCwdArg().
  DaemonAttachTerminal.isStreaming: DaemonAttachTerminal#isStreaming.
  getMessageText: getMessageText().
  formatContentBlock: formatContentBlock().
  ParsedDaemonClientCommand: ParsedDaemonClientCommand#
  SessionEndWaiter.promise: SessionEndWaiter#promise.
  SessionEndWaiter.cancel: SessionEndWaiter#cancel.
  DaemonAttachTerminal.printHelp: DaemonAttachTerminal#printHelp().
  ParsedSessionArgs.name: ParsedSessionArgs#name.
  SessionEndWaiter: SessionEndWaiter#
  getStringProperty: getStringProperty().
  parseListArgs: parseListArgs().
  DaemonWaiterMessagePredicate: DaemonWaiterMessagePredicate#
  DaemonAttachTerminal.-constructor: DaemonAttachTerminal#`<constructor>`().
  isMessagesData: isMessagesData().
  formatContent: formatContent().
  getCronJobs: getCronJobs().
  ParsedSessionArgs.daemonArgs: ParsedSessionArgs#daemonArgs.
  ParsedSessionArgs.sessionPath: ParsedSessionArgs#sessionPath.
  ParsedSessionArgs.continueRecent: ParsedSessionArgs#continueRecent.
  ParsedSessionOption.value: ParsedSessionOption#value.
  ParsedSessionOption.sessionPath: ParsedSessionOption#sessionPath.
  requireOptionValue: requireOptionValue().
  requireNoExtraArgs: requireNoExtraArgs().
  ParsedSessionOption.continueRecent: ParsedSessionOption#continueRecent.
  parseCsvValue: parseCsvValue().
  parseListArgs.typeLiteral517.all: parseListArgs().typeLiteral517:all.
  ParsedSendArgs.targetActiveSessionId: ParsedSendArgs#targetActiveSessionId.
  ParsedSendArgs.fromActiveSessionId: ParsedSendArgs#fromActiveSessionId.
  ParsedSendArgs.message: ParsedSendArgs#message.
  printJsonLine: printJsonLine.
  getCronJob: getCronJob().
  DAEMON_CLIENT_COMMANDS: DAEMON_CLIENT_COMMANDS.
  ParsedSessionArgs: ParsedSessionArgs#
  SESSION_BOOLEAN_FLAGS: SESSION_BOOLEAN_FLAGS.
  looksLikeSessionPath: looksLikeSessionPath().
  ParsedSendArgs: ParsedSendArgs#
  DaemonAttachTerminal.prompt: DaemonAttachTerminal#prompt.
  getUnknownProperty: getUnknownProperty().
  formatRole: formatRole().
  indent: indent().
  isAgentMessageReceipt: isAgentMessageReceipt().
  DaemonAttachTerminal: DaemonAttachTerminal#
---
# Module: [`packages/coding-agent/src/cli/daemon-command.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts)

## Classes
### `DaemonAttachTerminal`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:1253`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1253)
- signature: `class DaemonAttachTerminal`
- members:
  - `<constructor>(client: DaemonClient, activeSessionId: string)` — [`L1258`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1258)
  - `handleInput(method)` — [`L1298`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1298)
  - `handleMessage(method)` — [`L1353`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1353)
  - `handleSessionEvent(method)` — [`L1418`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1418)
  - `printHelp(method)` — [`L1502`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1502)
  - `printMessage(method)` — [`L1495`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1495)
  - `printTranscript(method)` — [`L1489`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1489)
  - `run(method)` — [`L1263`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1263)
  - `writeLine(method)` — [`L1506`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1506)
  - `isStreaming` — [`L1255`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1255)
  - `prompt` — [`L1256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1256)
  - `rl` — [`L1254`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1254)
- uses (calls/refs, reference-scoped): [`id`](../../../ai/src/types.ts.md#Model.id), [`provider`](../../../ai/src/types.ts.md#Model.provider), [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage), [`request`](../modes/daemon/daemon-client.ts.md#DaemonClient.request), [`DaemonOutbound`](../modes/daemon/daemon-protocol.ts.md#DaemonOutbound), [`sessionFile`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.sessionFile), [`DaemonClient`](../modes/daemon/daemon-client.ts.md#DaemonClient), [`sessionName`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.sessionName), [`status`](../core/goals.ts.md#GoalState.status), [`name`](../../../ai/src/types.ts.md#ToolCall.name), [`AgentSessionEvent`](../core/agent-session.ts.md#AgentSessionEvent), [`isStreaming`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.isStreaming), [`messages`](../modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.messages), [`steering`](../core/session-action-store.ts.md#SessionActionSnapshot.steering), [`followUps`](../core/session-action-store.ts.md#SessionActionSnapshot.followUps), [`queuedCount`](../core/session-action-store.ts.md#SessionActionSnapshot.queuedCount), [`state`](../modes/daemon/daemon-protocol.ts.md#DaemonSessionSnapshot.state), [`getMessageRole`](daemon-command.ts.md#getMessageRole), [`model`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.model), [`requireSuccess`](daemon-command.ts.md#requireSuccess), [`onMessage`](../modes/daemon/daemon-client.ts.md#DaemonClient.onMessage), [`isStreaming`](../modes/agent-connection/types.ts.md#AgentConnectionState.isStreaming), [`requireSuccessAsync`](daemon-command.ts.md#requireSuccessAsync), [`sessionName`](../modes/agent-connection/types.ts.md#AgentConnectionState.sessionName), [`status`](../core/agent-session.ts.md#RlmChildAgentSnapshot.status), [`getMessageText`](daemon-command.ts.md#getMessageText), [`isMessagesData`](daemon-command.ts.md#isMessagesData), [`label`](../core/agent-session.ts.md#RlmChildAgentSnapshot.label), [`formatRole`](daemon-command.ts.md#formatRole), [`indent`](daemon-command.ts.md#indent)
- used by: [`runAttach`](daemon-command.ts.md#runAttach)

### `DaemonWaiterMessagePredicate`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:1132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1132)
- signature: `type DaemonWaiterMessagePredicate`
- uses (calls/refs, reference-scoped): [`DaemonOutbound`](../modes/daemon/daemon-protocol.ts.md#DaemonOutbound)
- used by: [`createDaemonMessageWaiter`](daemon-command.ts.md#createDaemonMessageWaiter)

### `ParsedDaemonClientCommand`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L21)
- signature: `interface ParsedDaemonClientCommand`
- members:
  - `command` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L22)
  - `json` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L24)
  - `positionals` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L25)
  - `socketPath` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L23)
- used by: [`runOpen`](daemon-command.ts.md#runOpen), [`runDaemonClientCommand`](daemon-command.ts.md#runDaemonClientCommand), [`runStart`](daemon-command.ts.md#runStart), [`parseDaemonClientCommand`](daemon-command.ts.md#parseDaemonClientCommand), [`runPsCommand`](daemon-command.ts.md#runPsCommand)

### `ParsedSendArgs`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:917`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L917)
- signature: `interface ParsedSendArgs`
- members:
  - `fromActiveSessionId` — [`L919`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L919)
  - `message` — [`L920`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L920)
  - `targetActiveSessionId` — [`L918`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L918)
- used by: [`runSend`](daemon-command.ts.md#runSend), [`parseSendArgs`](daemon-command.ts.md#parseSendArgs)

### `ParsedSessionArgs`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:303`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L303)
- signature: `interface ParsedSessionArgs`
- members:
  - `config` — [`L306`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L306)
  - `continueRecent` — [`L308`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L308)
  - `daemonArgs` — [`L304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L304)
  - `name` — [`L305`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L305)
  - `sessionPath` — [`L307`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L307)
- uses (calls/refs, reference-scoped): [`AgentSessionRuntimeConfig`](../core/agent-session-config.ts.md#AgentSessionRuntimeConfig)
- used by: [`runOpen`](daemon-command.ts.md#runOpen), [`parseSessionArgs`](daemon-command.ts.md#parseSessionArgs), [`runCreate`](daemon-command.ts.md#runCreate), [`runStart`](daemon-command.ts.md#runStart)

### `ParsedSessionOption`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:406`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L406)
- signature: `interface ParsedSessionOption`
- members:
  - `consumed` — [`L407`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L407)
  - `continueRecent` — [`L411`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L411)
  - `daemonArg` — [`L408`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L408)
  - `sessionPath` — [`L410`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L410)
  - `value` — [`L409`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L409)
- used by: [`parseSessionOption`](daemon-command.ts.md#parseSessionOption), [`parseSessionArgs`](daemon-command.ts.md#parseSessionArgs), [`parseExtensionFlagOption`](daemon-command.ts.md#parseExtensionFlagOption)

### `SessionEndWaiter`
- def: [`packages/coding-agent/src/cli/daemon-command.ts:1127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1127)
- signature: `interface SessionEndWaiter`
- members:
  - `cancel` — [`L1129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1129)
  - `promise` — [`L1128`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1128)
- used by: [`runJsonAttach`](daemon-command.ts.md#runJsonAttach), [`runPrompt`](daemon-command.ts.md#runPrompt), [`createDaemonMessageWaiter`](daemon-command.ts.md#createDaemonMessageWaiter), [`waitForSessionClose`](daemon-command.ts.md#waitForSessionClose), [`waitForSessionEnd`](daemon-command.ts.md#waitForSessionEnd), [`waitUntilInterrupted`](daemon-command.ts.md#waitUntilInterrupted)

## Functions
- `canConnectToDaemon(socketPath: string, timeoutMs: number)` — [`L733`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L733)
- `createDaemonMessageWaiter(client: DaemonClient, shouldResolveOnMessage: DaemonWaiterMessagePredicate)` — [`L1134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1134)
- `findSessionCwdArg(args: string[])` — [`L594`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L594)
- `formatContent(content: unknown)` — [`L1537`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1537)
- `formatContentBlock(block: unknown)` — [`L1553`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1553)
- `formatRole(role: string)` — [`L1590`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1590)
- `getCronJob(value: unknown)` — [`L1667`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1667)
- `getCronJobs(value: unknown)` — [`L1659`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1659)
- `getLiveSessions(client: DaemonClient, all?: boolean)` — [`L641`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L641)
- `getMessageRole(message: AgentMessage)` — [`L1523`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1523)
- `getMessageText(message: AgentMessage)` — [`L1530`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1530)
- `getSessionSummaries(value: unknown)` — [`L1610`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1610)
- `getStringProperty(value: object, key: string)` — [`L1580`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1580)
- `getUnknownProperty(value: object, key: string)` — [`L1586`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1586)
- `handleDaemonCommand(args: string[])` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L52)
- `indent(text: string)` — [`L1603`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1603)
- `isAgentMessageReceipt(value: unknown)` — [`L1679`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1679)
- `isLiveSessionSummary(value: unknown)` — [`L1655`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1655)
- `isMessagesData(value: unknown)` — [`L1516`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1516)
- `isSessionSummary(value: unknown)` — [`L1630`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1630)
- `looksLikeSessionPath(value: string)` — [`L624`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L624)
- `nextDefaultSessionName(sessions: SessionSummary[])` — [`L651`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L651)
- `parseCsvValue(value: string)` — [`L587`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L587)
- `parseDaemonClientCommand(args: string[])` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L69)
- `parseExtensionFlagOption(args: string[], index: number, config: AgentSessionRuntimeConfig)` — [`L606`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L606)
- `parseListArgs(args: string[])` — [`L768`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L768)
- `parseSendArgs(args: string[])` — [`L923`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L923)
- `parseSessionArgs(args: string[])` — [`L336`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L336)
- `parseSessionOption(args: string[], index: number, config: AgentSessionRuntimeConfig, pathBaseCwd: string)` — [`L414`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L414)
- `printJson(value: unknown)` — [`L1245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1245)
- `printResponseData(client: DaemonClient, command: DaemonCommandBody, json: boolean)` — [`L1094`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1094)
- `requireActiveSessionId(args: string[])` — [`L1108`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1108)
- `requireNoExtraArgs(args: string[], usage: string)` — [`L890`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L890)
- `requireOptionValue(args: string[], index: number, option: string)` — [`L628`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L628)
- `requireSuccess(response: DaemonResponse)` — [`L1116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1116)
- `requireSuccessAsync(responsePromise: Promise<DaemonResponse>)` — [`L1123`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1123)
- `resolveLiveSessionSelector(client: DaemonClient, selector: string)` — [`L1071`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1071)
- `resolvePathOption(value: string, cwd: string)` — [`L636`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L636)
- `runAgentMessages(client: DaemonClient, args: string[], json: boolean)` — [`L862`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L862)
- `runAttach(client: DaemonClient, activeSessionId: string)` — [`L802`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L802)
- `runCreate(client: DaemonClient, args: string[], json: boolean)` — [`L780`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L780)
- `runCron(client: DaemonClient, args: string[], json: boolean)` — [`L997`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L997)
- `runDaemonClientCommand(parsed: ParsedDaemonClientCommand)` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L132)
- `runJsonAttach(client: DaemonClient, activeSessionId: string)` — [`L807`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L807)
- `runList(client: DaemonClient, args: string[], json: boolean)` — [`L745`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L745)
- `runMessageCommand(client: DaemonClient, type: "steer" | "follow_up", args: string[], json: boolean)` — [`L982`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L982)
- `runOpen(parsed: ParsedDaemonClientCommand)` — [`L266`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L266)
- `runPrompt(client: DaemonClient, args: string[])` — [`L841`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L841)
- `runPsCommand(parsed: ParsedDaemonClientCommand)` — [`L714`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L714)
- `runRename(client: DaemonClient, args: string[], json: boolean)` — [`L821`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L821)
- `runSend(client: DaemonClient, args: string[], json: boolean)` — [`L896`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L896)
- `runShutdown(client: DaemonClient, args: string[], json: boolean)` — [`L254`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L254)
- `runStart(parsed: ParsedDaemonClientCommand)` — [`L673`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L673)
- `waitForSessionClose(client: DaemonClient, activeSessionId: string)` — [`L1206`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1206)
- `waitForSessionEnd(client: DaemonClient, activeSessionId: string, isPromptAcknowledged?: (() => boolean) | undefined)` — [`L1181`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1181)
- `waitUntilInterrupted()` — [`L1213`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1213)

## Module values
- `DAEMON_CLIENT_COMMANDS` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L28)
- `SESSION_BOOLEAN_FLAGS` — [`L311`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L311)
- `all` — [`L768`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L768)
- `printJsonLine` — [`L1249`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-command.ts#L1249)

