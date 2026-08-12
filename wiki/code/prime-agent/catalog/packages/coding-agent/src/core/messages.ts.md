---
title: 'Module: packages/coding-agent/src/core/messages.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/messages.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`messages.ts`/
symbols:
  CustomMessage.role: CustomMessage#role.
  BashExecutionMessage.role: BashExecutionMessage#role.
  BranchSummaryMessage.role: BranchSummaryMessage#role.
  CompactionSummaryMessage.role: CompactionSummaryMessage#role.
  CustomMessage.timestamp: CustomMessage#timestamp.
  BashExecutionMessage.timestamp: BashExecutionMessage#timestamp.
  CustomMessage.customType: CustomMessage#customType.
  CompactionSummaryMessage.timestamp: CompactionSummaryMessage#timestamp.
  BranchSummaryMessage.timestamp: BranchSummaryMessage#timestamp.
  CustomMessage.content: CustomMessage#content.
  convertToLlm: convertToLlm().
  CustomMessage: CustomMessage#
  CustomMessage.display: CustomMessage#display.
  createHeartbeatPromptMessage: createHeartbeatPromptMessage().
  CustomMessage.details: CustomMessage#details.
  createSessionSlashCommandMessage: createSessionSlashCommandMessage().
  createCompactionOutcomeMessage: createCompactionOutcomeMessage().
  createSessionSlashCommandResultMessage: createSessionSlashCommandResultMessage().
  createRlmChildFailureMessage: createRlmChildFailureMessage().
  isSessionSlashCommandMessage: isSessionSlashCommandMessage().
  createCustomMessage: createCustomMessage().
  isSessionSlashCommandResultMessage: isSessionSlashCommandResultMessage().
  createRlmChildTerminalNoticeMessage: createRlmChildTerminalNoticeMessage().
  createCompactionSummaryMessage: createCompactionSummaryMessage().
  isSessionSlashCommand: isSessionSlashCommand().
  isCompactionOutcomeMessage: isCompactionOutcomeMessage().
  createBranchSummaryMessage: createBranchSummaryMessage().
  bashOutputToText: bashOutputToText().
  COMPACTION_OUTCOME_CUSTOM_TYPE: COMPACTION_OUTCOME_CUSTOM_TYPE.
  BashExecutionMessage.output: BashExecutionMessage#output.
  CompactionOutcomeDetails.reason: CompactionOutcomeDetails#reason.
  IPYTHON_STATE_RESTORED_CUSTOM_TYPE: IPYTHON_STATE_RESTORED_CUSTOM_TYPE.
  SESSION_SLASH_COMMAND_CUSTOM_TYPE: SESSION_SLASH_COMMAND_CUSTOM_TYPE.
  CompactionOutcomeDetails.outcome: CompactionOutcomeDetails#outcome.
  CompactionOutcomeMessage: CompactionOutcomeMessage#
  SessionSlashCommandResultDetails.command: SessionSlashCommandResultDetails#command.
  HEARTBEAT_PROMPT_CUSTOM_TYPE: HEARTBEAT_PROMPT_CUSTOM_TYPE.
  SESSION_SLASH_COMMAND_RESULT_CUSTOM_TYPE: SESSION_SLASH_COMMAND_RESULT_CUSTOM_TYPE.
  SessionSlashCommandResultMessage: SessionSlashCommandResultMessage#
  SessionSlashCommandMessage.details: SessionSlashCommandMessage#details.
  SessionSlashCommandResultMessage.details: SessionSlashCommandResultMessage#details.
  SessionSlashCommandDetails.command: SessionSlashCommandDetails#command.
  bashExecutionToText: bashExecutionToText().
  SessionSlashCommandResultDetails.success: SessionSlashCommandResultDetails#success.
  SessionSlashCommandResultDetails.severity: SessionSlashCommandResultDetails#severity.
  BashExecutionMessage: BashExecutionMessage#
  SessionSlashCommandMessage: SessionSlashCommandMessage#
  BashExecutionMessage.exitCode: BashExecutionMessage#exitCode.
  isRecord: isRecord().
  CompactionOutcomeMessage.details: CompactionOutcomeMessage#details.
  BashExecutionMessage.command: BashExecutionMessage#command.
  BranchSummaryMessage.summary: BranchSummaryMessage#summary.
  CompactionSummaryMessage.summary: CompactionSummaryMessage#summary.
  CompactionOutcomeDetails: CompactionOutcomeDetails#
  BashExecutionMessage.cancelled: BashExecutionMessage#cancelled.
  BashExecutionMessage.fullOutputPath: BashExecutionMessage#fullOutputPath.
  HeartbeatPromptDetails.status: HeartbeatPromptDetails#status.
  IpythonStateRestoredDetails: IpythonStateRestoredDetails#
  BranchSummaryMessage: BranchSummaryMessage#
  CompactionSummaryMessage: CompactionSummaryMessage#
  CompactionOutcomeMessage.customType: CompactionOutcomeMessage#customType.
  CustomAgentMessages: '`"@earendil-works/pi-agent-core"`/CustomAgentMessages#'
  HEARTBEAT_PROMPT_PREVIEW_LABEL: HEARTBEAT_PROMPT_PREVIEW_LABEL.
  RLM_CHILD_FAILURE_CUSTOM_TYPE: RLM_CHILD_FAILURE_CUSTOM_TYPE.
  RLM_CHILD_TERMINAL_NOTICE_CUSTOM_TYPE: RLM_CHILD_TERMINAL_NOTICE_CUSTOM_TYPE.
  CompactionOutcomeReason: CompactionOutcomeReason#
  CompactionOutcome: CompactionOutcome#
  CompactionOutcomeMessage.content: CompactionOutcomeMessage#content.
  RlmChildFailureDetails: RlmChildFailureDetails#
  RlmChildTerminalNoticeDetails: RlmChildTerminalNoticeDetails#
  BashExecutionMessage.truncated: BashExecutionMessage#truncated.
  BashExecutionMessage.excludeFromContext: BashExecutionMessage#excludeFromContext.
  HeartbeatPromptDetails: HeartbeatPromptDetails#
  CompactionSummaryMessage.retainedMessageCount: CompactionSummaryMessage#retainedMessageCount.
  SessionSlashCommandMessage.customType: SessionSlashCommandMessage#customType.
  SessionSlashCommandResultMessage.customType: SessionSlashCommandResultMessage#customType.
  SessionSlashCommandDetails: SessionSlashCommandDetails#
  SessionSlashCommandResultDetails: SessionSlashCommandResultDetails#
  SessionSlashCommandResultDetails.error: SessionSlashCommandResultDetails#error.
  SessionSlashCommandMessage.content: SessionSlashCommandMessage#content.
  SessionSlashCommandResultMessage.content: SessionSlashCommandResultMessage#content.
  hasValidCustomMessageEnvelope: hasValidCustomMessageEnvelope().
  CustomAgentMessages.bashExecution: '`"@earendil-works/pi-agent-core"`/CustomAgentMessages#bashExecution.'
  CustomAgentMessages.custom: '`"@earendil-works/pi-agent-core"`/CustomAgentMessages#custom.'
  CustomAgentMessages.branchSummary: '`"@earendil-works/pi-agent-core"`/CustomAgentMessages#branchSummary.'
  RlmChildFailureDetails.childId: RlmChildFailureDetails#childId.
  RlmChildFailureDetails.sessionName: RlmChildFailureDetails#sessionName.
  RlmChildFailureDetails.error: RlmChildFailureDetails#error.
  CompactionSummaryMessage.tokensBefore: CompactionSummaryMessage#tokensBefore.
  CompactionSummaryMessage.customInstructions: CompactionSummaryMessage#customInstructions.
  isValidCommandEntryId: isValidCommandEntryId().
  COMPACTION_SUMMARY_PREFIX: COMPACTION_SUMMARY_PREFIX.
  COMPACTION_SUMMARY_SUFFIX: COMPACTION_SUMMARY_SUFFIX.
  BRANCH_SUMMARY_PREFIX: BRANCH_SUMMARY_PREFIX.
  BRANCH_SUMMARY_SUFFIX: BRANCH_SUMMARY_SUFFIX.
  SessionSlashCommandResultDetails.commandEntryId: SessionSlashCommandResultDetails#commandEntryId.
  HeartbeatPromptDetails.schedule: HeartbeatPromptDetails#schedule.
  IpythonStateRestoredDetails.restored: IpythonStateRestoredDetails#restored.
  BranchSummaryMessage.fromId: BranchSummaryMessage#fromId.
  SessionSlashCommandDetails.commandEntryId: SessionSlashCommandDetails#commandEntryId.
  HeartbeatPromptDetails.jobId: HeartbeatPromptDetails#jobId.
  HeartbeatPromptDetails.runCount: HeartbeatPromptDetails#runCount.
  HeartbeatPromptDetails.nextRunAt: HeartbeatPromptDetails#nextRunAt.
  HeartbeatPromptDetails.lastRunAt: HeartbeatPromptDetails#lastRunAt.
  CustomAgentMessages.compactionSummary: '`"@earendil-works/pi-agent-core"`/CustomAgentMessages#compactionSummary.'
---
# Module: [`packages/coding-agent/src/core/messages.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts)

## Classes
### `BashExecutionMessage`
- def: [`packages/coding-agent/src/core/messages.ts:131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L131)
- doc: Message type for bash executions via the ! command.
- signature: `interface BashExecutionMessage`
- members:
  - `cancelled` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L136)
  - `command` — [`L133`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L133)
  - `excludeFromContext` — [`L141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L141) — If true, this message is excluded from LLM context (!! prefix)
  - `exitCode` — [`L135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L135)
  - `fullOutputPath` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L138)
  - `output` — [`L134`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L134)
  - `role` — [`L132`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L132) — documented in [packages-coding-agent-src-core-messages.ts](../../../../../concepts/packages-coding-agent-src-core-messages.ts.md)
  - `timestamp` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L139)
  - `truncated` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L137)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`handleEvent`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`appendMessage`](session-manager.ts.md#SessionManager.appendMessage), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`buildConversationComponents`](../modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`acpUpdatesForSessionEvent`](../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`session-manager.ts`](session-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-session-manager.ts), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`limitTranscript`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntryDisplayText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`applyFilter`](../modes/interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`getSessionStats`](agent-session.ts.md#AgentSession.getSessionStats), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction), [`flattenTree`](../modes/interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`_runAutoCompaction`](agent-session.ts.md#AgentSession._runAutoCompaction), [`convertToLlm`](messages.ts.md#convertToLlm), [`refreshWorkerSummaries`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`createAgentObserveMessagePreview`](agent-observe.ts.md#createAgentObserveMessagePreview), [`handleEvent`](../modes/interactive/agent-activity.ts.md#AgentActivityTracker.handleEvent), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`_handleRetryableError`](agent-session.ts.md#AgentSession._handleRetryableError), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`recordBashResult`](agent-session.ts.md#AgentSession.recordBashResult)  (+53 more; 89 test-only)

### `BranchSummaryMessage`
- def: [`packages/coding-agent/src/core/messages.ts:170`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L170)
- signature: `interface BranchSummaryMessage`
- members:
  - `fromId` — [`L173`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L173)
  - `role` — [`L171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L171)
  - `summary` — [`L172`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L172)
  - `timestamp` — [`L174`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L174)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`handleEvent`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`buildConversationComponents`](../modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`acpUpdatesForSessionEvent`](../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`limitTranscript`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntryDisplayText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`applyFilter`](../modes/interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`getSessionStats`](agent-session.ts.md#AgentSession.getSessionStats), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction), [`flattenTree`](../modes/interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`_runAutoCompaction`](agent-session.ts.md#AgentSession._runAutoCompaction), [`convertToLlm`](messages.ts.md#convertToLlm), [`refreshWorkerSummaries`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`createAgentObserveMessagePreview`](agent-observe.ts.md#createAgentObserveMessagePreview), [`handleEvent`](../modes/interactive/agent-activity.ts.md#AgentActivityTracker.handleEvent), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`_handleRetryableError`](agent-session.ts.md#AgentSession._handleRetryableError), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`estimateTokens`](compaction/compaction.ts.md#estimateTokens), [`handleRunFailure`](../../../agent/src/agent.ts.md#Agent.handleRunFailure), [`_notifyKernelStateAfterCompaction`](agent-session.ts.md#AgentSession._notifyKernelStateAfterCompaction), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry)  (+50 more; 78 test-only)

### `CompactionOutcome`
- def: [`packages/coding-agent/src/core/messages.ts:63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L63)
- signature: `type CompactionOutcome`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_persistCompactionOutcome`](agent-session.ts.md#AgentSession._persistCompactionOutcome), [`_endCompactionUnsuccessfully`](agent-session.ts.md#AgentSession._endCompactionUnsuccessfully), [`CompactionOutcomeDetails`](messages.ts.md#CompactionOutcomeDetails)

### `CompactionOutcomeDetails`
- def: [`packages/coding-agent/src/core/messages.ts:65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L65)
- signature: `interface CompactionOutcomeDetails`
- members:
  - `outcome` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L67)
  - `reason` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L66)
- uses (calls/refs, reference-scoped): [`CompactionOutcome`](messages.ts.md#CompactionOutcome), [`CompactionOutcomeReason`](messages.ts.md#CompactionOutcomeReason)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`_persistCompactionOutcome`](agent-session.ts.md#AgentSession._persistCompactionOutcome), [`createCompactionOutcomeMessage`](messages.ts.md#createCompactionOutcomeMessage), [`<constructor>`](../modes/interactive/components/compaction-outcome-message.ts.md#CompactionOutcomeMessageComponent.-constructor), [`CompactionOutcomeMessage`](messages.ts.md#CompactionOutcomeMessage), [`details`](messages.ts.md#CompactionOutcomeMessage.details)  (2 test-only)

### `CompactionOutcomeMessage`
- def: [`packages/coding-agent/src/core/messages.ts:70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L70)
- signature: `interface CompactionOutcomeMessage`
- members:
  - `content` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L72)
  - `customType` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L71)
  - `details` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L73)
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`COMPACTION_OUTCOME_CUSTOM_TYPE`](messages.ts.md#COMPACTION_OUTCOME_CUSTOM_TYPE), [`CompactionOutcomeDetails`](messages.ts.md#CompactionOutcomeDetails)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`headless-completion.ts`](../modes/headless-completion.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-headless-completion.ts), [`selectHeadlessTerminalResult`](../modes/headless-completion.ts.md#selectHeadlessTerminalResult), [`_persistCompactionOutcome`](agent-session.ts.md#AgentSession._persistCompactionOutcome), [`createCompactionOutcomeMessage`](messages.ts.md#createCompactionOutcomeMessage), [`<constructor>`](../modes/interactive/components/compaction-outcome-message.ts.md#CompactionOutcomeMessageComponent.-constructor), [`compaction-outcome-message.ts`](../modes/interactive/components/compaction-outcome-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-compaction-outcome-message.ts), [`isCompactionOutcomeMessage`](messages.ts.md#isCompactionOutcomeMessage), [`HeadlessTerminalResult`](../modes/headless-completion.ts.md#HeadlessTerminalResult)

### `CompactionOutcomeReason`
- def: [`packages/coding-agent/src/core/messages.ts:62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L62)
- signature: `type CompactionOutcomeReason`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_persistCompactionOutcome`](agent-session.ts.md#AgentSession._persistCompactionOutcome), [`reason`](messages.ts.md#CompactionOutcomeDetails.reason), [`_endCompactionUnsuccessfully`](agent-session.ts.md#AgentSession._endCompactionUnsuccessfully)

### `CompactionSummaryMessage`
- def: [`packages/coding-agent/src/core/messages.ts:177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L177)
- signature: `interface CompactionSummaryMessage`
- members:
  - `customInstructions` — [`L184`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L184) — User instructions that guided the summary (from `/compact <instructions>`)
  - `retainedMessageCount` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L182) — Number of retained messages that precede this summary in transcript presentation.
  - `role` — [`L178`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L178)
  - `summary` — [`L179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L179)
  - `timestamp` — [`L185`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L185)
  - `tokensBefore` — [`L180`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L180)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`handleEvent`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`buildConversationComponents`](../modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`acpUpdatesForSessionEvent`](../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`limitTranscript`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntryDisplayText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`applyFilter`](../modes/interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`getSessionStats`](agent-session.ts.md#AgentSession.getSessionStats), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction), [`flattenTree`](../modes/interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage), [`_runAutoCompaction`](agent-session.ts.md#AgentSession._runAutoCompaction), [`convertToLlm`](messages.ts.md#convertToLlm), [`refreshWorkerSummaries`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.refreshWorkerSummaries), [`findCutPoint`](compaction/compaction.ts.md#findCutPoint), [`createAgentObserveMessagePreview`](agent-observe.ts.md#createAgentObserveMessagePreview), [`handleEvent`](../modes/interactive/agent-activity.ts.md#AgentActivityTracker.handleEvent), [`applyChildUsageAttributions`](session-manager.ts.md#applyChildUsageAttributions), [`_persist`](session-manager.ts.md#SessionManager._persist), [`_handleRetryableError`](agent-session.ts.md#AgentSession._handleRetryableError), [`getUserMessagesForForking`](agent-session.ts.md#AgentSession.getUserMessagesForForking), [`estimateTokens`](compaction/compaction.ts.md#estimateTokens), [`handleRunFailure`](../../../agent/src/agent.ts.md#Agent.handleRunFailure), [`_notifyKernelStateAfterCompaction`](agent-session.ts.md#AgentSession._notifyKernelStateAfterCompaction), [`isAssistantEntry`](context-tree.ts.md#isAssistantEntry)  (+50 more; 78 test-only)

### `CustomAgentMessages`
- def: [`packages/coding-agent/src/core/messages.ts:190`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L190)
- doc: Extensible interface for custom app messages.
- signature: `interface CustomAgentMessages`
- members:
  - `bashExecution` — [`L191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L191)
  - `branchSummary` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L193)
  - `compactionSummary` — [`L194`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L194)
  - `custom` — [`L192`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L192)
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`BashExecutionMessage`](messages.ts.md#BashExecutionMessage), [`BranchSummaryMessage`](messages.ts.md#BranchSummaryMessage), [`CompactionSummaryMessage`](messages.ts.md#CompactionSummaryMessage)
- used by: [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage)

### `CustomMessage`
- def: [`packages/coding-agent/src/core/messages.ts:148`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L148)
- doc: Message type for extension-injected messages via sendMessage().
- signature: `interface CustomMessage`
- members:
  - `content` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L151)
  - `customType` — [`L150`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L150)
  - `details` — [`L153`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L153)
  - `display` — [`L152`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L152)
  - `role` — [`L149`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L149) — documented in [packages-coding-agent-src-core-messages.ts](../../../../../concepts/packages-coding-agent-src-core-messages.ts.md)
  - `timestamp` — [`L154`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L154)
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`TextContent`](../../../ai/src/types.ts.md#TextContent)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`handleEvent`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`appendMessage`](session-manager.ts.md#SessionManager.appendMessage), [`summaryEntry`](agent-session.ts.md#AgentSession._navigateTreeUnderPause.Promise.typeLiteral4237.summaryEntry), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`type`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.attachClient.command-Extract.typeLiteral2177.type), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`buildConversationComponents`](../modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`acpUpdatesForSessionEvent`](../modes/acp/acp-events.ts.md#acpUpdatesForSessionEvent), [`buildSessionContext`](session-manager.ts.md#buildSessionContext), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`session-manager.ts`](session-manager.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-session-manager.ts), [`createBranchedSession`](session-manager.ts.md#SessionManager.createBranchedSession), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`limitTranscript`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.renderSessionContext.options-typeLiteral2780.limitTranscript), [`fork`](agent-session-runtime.ts.md#AgentSessionRuntime.fork), [`getEntryDisplayText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getEntryDisplayText), [`rlmChildSnapshotForActiveSession`](../modes/daemon/daemon-session-list.ts.md#rlmChildSnapshotForActiveSession), [`sendCustomMessage`](agent-session.ts.md#AgentSession.sendCustomMessage), [`acceptedBeforeCompletion`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion), [`applyFilter`](../modes/interactive/components/tree-selector.ts.md#TreeList.applyFilter), [`getSessionStats`](agent-session.ts.md#AgentSession.getSessionStats), [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`preRenderCustomTools`](export-html/index.ts.md#preRenderCustomTools), [`_promptInjectedMessage`](agent-session.ts.md#AgentSession._promptInjectedMessage), [`_checkCompaction`](agent-session.ts.md#AgentSession._checkCompaction), [`flattenTree`](../modes/interactive/components/tree-selector.ts.md#TreeList.flattenTree), [`getSearchableText`](../modes/interactive/components/tree-selector.ts.md#TreeList.getSearchableText), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`loadContextTreeChildFromDisk`](context-tree.ts.md#loadContextTreeChildFromDisk), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`appendChildUsageAttribution`](session-manager.ts.md#SessionManager.appendChildUsageAttribution), [`getMessageFromEntry`](compaction/branch-summarization.ts.md#getMessageFromEntry), [`getContextUsage`](agent-session.ts.md#AgentSession.getContextUsage)  (+127 more; 100 test-only)

### `HeartbeatPromptDetails`
- def: [`packages/coding-agent/src/core/messages.ts:157`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L157)
- signature: `interface HeartbeatPromptDetails`
- members:
  - `jobId` — [`L158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L158)
  - `lastRunAt` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L163)
  - `nextRunAt` — [`L162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L162)
  - `runCount` — [`L161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L161)
  - `schedule` — [`L159`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L159)
  - `status` — [`L160`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L160)
- uses (calls/refs, reference-scoped): [`AgentCronJob`](cron-jobs.ts.md#AgentCronJob), [`status`](cron-jobs.ts.md#AgentCronJob.status)
- used by: [`injected-prompt-message.ts`](../modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`createHeartbeatPromptMessage`](messages.ts.md#createHeartbeatPromptMessage), [`heartbeatHeaderText`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptMessageComponent.heartbeatHeaderText), [`InjectedPromptDetails`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptDetails)

### `IpythonStateRestoredDetails`
- def: [`packages/coding-agent/src/core/messages.ts:166`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L166)
- signature: `interface IpythonStateRestoredDetails`
- members:
  - `restored` — [`L167`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L167)
- used by: [`injected-prompt-message.ts`](../modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`headerText`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptMessageComponent.headerText), [`InjectedPromptDetails`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptDetails)  (1 test-only)

### `RlmChildFailureDetails`
- def: [`packages/coding-agent/src/core/messages.ts:76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L76)
- signature: `interface RlmChildFailureDetails`
- members:
  - `childId` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L77)
  - `error` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L79)
  - `sessionName` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L78)
- used by: [`_startRlmChildRun`](agent-session.ts.md#AgentSession._startRlmChildRun), [`injected-prompt-message.ts`](../modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`createRlmChildFailureMessage`](messages.ts.md#createRlmChildFailureMessage), [`InjectedPromptDetails`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptDetails)

### `RlmChildTerminalNoticeDetails`
- def: [`packages/coding-agent/src/core/messages.ts:82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L82)
- signature: `type RlmChildTerminalNoticeDetails`
- used by: [`injected-prompt-message.ts`](../modes/interactive/components/injected-prompt-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-injected-prompt-message.ts), [`createRlmChildTerminalNoticeMessage`](messages.ts.md#createRlmChildTerminalNoticeMessage), [`InjectedPromptDetails`](../modes/interactive/components/injected-prompt-message.ts.md#InjectedPromptDetails)

### `SessionSlashCommandDetails`
- def: [`packages/coding-agent/src/core/messages.ts:37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L37)
- signature: `interface SessionSlashCommandDetails`
- members:
  - `command` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L38)
  - `commandEntryId` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L39)
- uses (calls/refs, reference-scoped): [`SessionSlashCommand`](slash-commands.ts.md#SessionSlashCommand)
- used by: [`createSessionSlashCommandMessage`](messages.ts.md#createSessionSlashCommandMessage), [`_restoreSessionCommand`](agent-session.ts.md#AgentSession._restoreSessionCommand), [`details`](messages.ts.md#SessionSlashCommandMessage.details), [`SessionSlashCommandMessage`](messages.ts.md#SessionSlashCommandMessage)  (1 test-only)

### `SessionSlashCommandMessage`
- def: [`packages/coding-agent/src/core/messages.ts:50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L50)
- signature: `interface SessionSlashCommandMessage`
- members:
  - `content` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L52)
  - `customType` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L51)
  - `details` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L53)
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`SESSION_SLASH_COMMAND_CUSTOM_TYPE`](messages.ts.md#SESSION_SLASH_COMMAND_CUSTOM_TYPE), [`SessionSlashCommandDetails`](messages.ts.md#SessionSlashCommandDetails)
- used by: [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`buildConversationComponents`](../modes/interactive/components/conversation-components.ts.md#buildConversationComponents), [`createSessionSlashCommandMessage`](messages.ts.md#createSessionSlashCommandMessage), [`isSessionSlashCommandMessage`](messages.ts.md#isSessionSlashCommandMessage), [`_restoreSessionCommand`](agent-session.ts.md#AgentSession._restoreSessionCommand)  (1 test-only)

### `SessionSlashCommandResultDetails`
- def: [`packages/coding-agent/src/core/messages.ts:42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L42)
- signature: `interface SessionSlashCommandResultDetails`
- members:
  - `command` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L43)
  - `commandEntryId` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L47)
  - `error` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L46)
  - `severity` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L45)
  - `success` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L44)
- uses (calls/refs, reference-scoped): [`SessionSlashCommand`](slash-commands.ts.md#SessionSlashCommand)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`_appendDurableSessionCommandMessage`](agent-session.ts.md#AgentSession._appendDurableSessionCommandMessage), [`createSessionSlashCommandResultMessage`](messages.ts.md#createSessionSlashCommandResultMessage), [`SessionSlashCommandResultMessage`](messages.ts.md#SessionSlashCommandResultMessage), [`details`](messages.ts.md#SessionSlashCommandResultMessage.details)  (2 test-only)

### `SessionSlashCommandResultMessage`
- def: [`packages/coding-agent/src/core/messages.ts:56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L56)
- signature: `interface SessionSlashCommandResultMessage`
- members:
  - `content` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L58)
  - `customType` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L57)
  - `details` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L59)
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`SESSION_SLASH_COMMAND_RESULT_CUSTOM_TYPE`](messages.ts.md#SESSION_SLASH_COMMAND_RESULT_CUSTOM_TYPE), [`SessionSlashCommandResultDetails`](messages.ts.md#SessionSlashCommandResultDetails)
- used by: [`runPrintModeWithConnectionInternal`](../modes/print-mode.ts.md#runPrintModeWithConnectionInternal), [`headless-completion.ts`](../modes/headless-completion.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-headless-completion.ts), [`createSessionSlashCommandResultMessage`](messages.ts.md#createSessionSlashCommandResultMessage), [`isSessionSlashCommandResultMessage`](messages.ts.md#isSessionSlashCommandResultMessage), [`slash-command-result-message.ts`](../modes/interactive/components/slash-command-result-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-slash-command-result-message.ts), [`<constructor>`](../modes/interactive/components/slash-command-result-message.ts.md#SlashCommandResultMessageComponent.-constructor), [`HeadlessTerminalResultMessage`](../modes/headless-completion.ts.md#HeadlessTerminalResultMessage)  (1 test-only)

## Functions
- `bashExecutionToText(msg: BashExecutionMessage)` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L232) — Convert a BashExecutionMessage to user message text for LLM context.
- `bashOutputToText(msg: Pick<BashExecutionMessage, "output" | "cancelled" | "exitCode" | "truncated" | "fullOutputPath">)` — [`L202`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L202) — Format bash output for LLM context. The fence must be longer than any
- `convertToLlm(messages: AgentMessage[])` — [`L430`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L430) — Transform AgentMessages (including custom types) to LLM-compatible Messages.
- `createBranchSummaryMessage(summary: string, fromId: string, timestamp: string)` — [`L236`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L236)
- `createCompactionOutcomeMessage(content: string, details: CompactionOutcomeDetails, display?: boolean, timestamp?: number)` — [`L312`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L312)
- `createCompactionSummaryMessage(summary: string, tokensBefore: number, timestamp: string, customInstructions?: string | undefined, retainedMessageCount?: number | undefined)` — [`L245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L245)
- `createCustomMessage(customType: string, content: string | (TextContent | ImageContent)[], display: boolean, details: unknown, timestamp: string)` — [`L263`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L263) — Convert CustomMessageEntry to AgentMessage format
- `createHeartbeatPromptMessage(job: AgentCronJob, timestamp?: number)` — [`L401`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L401)
- `createRlmChildFailureMessage(details: RlmChildFailureDetails, timestamp?: number)` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L96)
- `createRlmChildTerminalNoticeMessage(details: RlmChildTerminalNoticeDetails, timestamp?: number)` — [`L110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L110)
- `createSessionSlashCommandMessage(command: SessionSlashCommand, details?: Omit<SessionSlashCommandDetails, "command">, display?: boolean, timestamp?: number)` — [`L280`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L280)
- `createSessionSlashCommandResultMessage(content: string, details: SessionSlashCommandResultDetails, display?: boolean, timestamp?: number)` — [`L296`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L296)
- `hasValidCustomMessageEnvelope(message: Record<string, unknown>, customType: string)` — [`L332`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L332)
- `isCompactionOutcomeMessage(message: unknown)` — [`L388`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L388)
- `isRecord(value: unknown)` — [`L328`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L328)
- `isSessionSlashCommand(value: unknown)` — [`L343`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L343)
- `isSessionSlashCommandMessage(message: unknown)` — [`L362`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L362)
- `isSessionSlashCommandResultMessage(message: unknown)` — [`L374`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L374)
- `isValidCommandEntryId(value: unknown)` — [`L358`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L358)

## Module values
- `BRANCH_SUMMARY_PREFIX` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L21)
- `BRANCH_SUMMARY_SUFFIX` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L26)
- `COMPACTION_OUTCOME_CUSTOM_TYPE` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L33)
- `COMPACTION_SUMMARY_PREFIX` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L13)
- `COMPACTION_SUMMARY_SUFFIX` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L18)
- `HEARTBEAT_PROMPT_CUSTOM_TYPE` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L28)
- `HEARTBEAT_PROMPT_PREVIEW_LABEL` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L29)
- `IPYTHON_STATE_RESTORED_CUSTOM_TYPE` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L30)
- `RLM_CHILD_FAILURE_CUSTOM_TYPE` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L34)
- `RLM_CHILD_TERMINAL_NOTICE_CUSTOM_TYPE` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L35)
- `SESSION_SLASH_COMMAND_CUSTOM_TYPE` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L31)
- `SESSION_SLASH_COMMAND_RESULT_CUSTOM_TYPE` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/messages.ts#L32)

