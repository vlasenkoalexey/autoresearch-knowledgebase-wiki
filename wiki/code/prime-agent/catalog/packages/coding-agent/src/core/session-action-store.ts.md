---
title: 'Module: packages/coding-agent/src/core/session-action-store.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-action-store.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-action-store.ts`/
symbols:
  SessionAction.payload: SessionAction#payload.
  SessionAction.lifecycle: SessionAction#lifecycle.
  SessionTurnPayload.kind: SessionTurnPayload#kind.
  SessionCommandPayload.kind: SessionCommandPayload#kind.
  SessionActionSnapshot.steering: SessionActionSnapshot#steering.
  SessionActionSnapshot.queuedCount: SessionActionSnapshot#queuedCount.
  SessionActionSnapshot.followUps: SessionActionSnapshot#followUps.
  SessionAction.id: SessionAction#id.
  canEvictWorker: canEvictWorker().
  canSelectSessionAction: canSelectSessionAction().
  DeliveryRecord.message: DeliveryRecord#message.
  ActionStore.unfinishedActions: ActionStore#unfinishedActions().
  transitionSessionAction: transitionSessionAction().
  SessionAction.delivery: SessionAction#delivery.
  ActionStore.queuedActions: ActionStore#queuedActions().
  canPassivateSession: canPassivateSession().
  ActionTicketController.-constructor: ActionTicketController#`<constructor>`().
  SessionAction.agentMessageId: SessionAction#agentMessageId.
  SessionTurnPayload.records: SessionTurnPayload#records.
  ActionStore.enqueue: ActionStore#enqueue().
  ActionStore.actionsForMessage: ActionStore#actionsForMessage().
  transitionSessionAction.options-typeLiteral36.rollbackProof: transitionSessionAction().(options)typeLiteral36:rollbackProof.
  ActionStore.selectFirst: ActionStore#selectFirst().
  ActionStore.queuePreview: ActionStore#queuePreview().
  ActionStore.enqueueFront: ActionStore#enqueueFront().
  isIdleEvictionThresholdMet: isIdleEvictionThresholdMet().
  ActionStore.releaseTerminal: ActionStore#releaseTerminal().
  primaryRecords: primaryRecords().
  DeliveryRecord.role: DeliveryRecord#role.
  SessionTurnPayload.text: SessionTurnPayload#text.
  SessionCommandPayload.text: SessionCommandPayload#text.
  SessionAction: SessionAction#
  ActionStore.ticketFor: ActionStore#ticketFor().
  DeliveryPolicy: DeliveryPolicy#
  ActionStore.activeActions: ActionStore#activeActions().
  ActionStore.actions: ActionStore#actions().
  ActionTicketController.settleCompleted: ActionTicketController#settleCompleted().
  ActionStore.list: ActionStore#list().
  ActionStore: ActionStore#
  ActionStore.moveQueued: ActionStore#moveQueued().
  QueuedMessageMutation: QueuedMessageMutation#
  SessionActionSnapshot.active: SessionActionSnapshot#active.
  DeliveryRecord.durable: DeliveryRecord#durable.
  ActionLifecycle: ActionLifecycle#
  createDeferred: createDeferred().
  IdleEvictionMinutes: IdleEvictionMinutes#
  ActionTicketController.settleDelivered: ActionTicketController#settleDelivered().
  ActionStore.clearableActions: ActionStore#clearableActions().
  SessionActionSnapshot: SessionActionSnapshot#
  SessionAction.wake: SessionAction#wake.
  ActionTicket.delivered: ActionTicket#delivered.
  ActionStore.rollback: ActionStore#rollback().
  SessionCommandPayload.command: SessionCommandPayload#command.
  ActionTicketController.settleAccepted: ActionTicketController#settleAccepted().
  ActionStore.ownedActions: ActionStore#ownedActions().
  ActionStore.assertNewAction: ActionStore#assertNewAction().
  DeliveryRecord: DeliveryRecord#
  SessionAction.queueKey: SessionAction#queueKey.
  SessionAction.source: SessionAction#source.
  isClearable: isClearable().
  ActionTicketController.ticket: ActionTicketController#ticket.
  ActionStore.swapQueued: ActionStore#swapQueued().
  WorkerEvictionSnapshot.sessions: WorkerEvictionSnapshot#sessions.
  QueuedMessageLane: QueuedMessageLane#
  queuedMessageLaneDeliveryPolicy: queuedMessageLaneDeliveryPolicy().
  ActionTicketController.delivered: ActionTicketController#delivered.
  ActionTicketController.rejectDelivered: ActionTicketController#rejectDelivered().
  ActionStore.tickets: ActionStore#tickets.
  SessionActionPayload: SessionActionPayload#
  SessionAction.suppressAutonomousContinuation: SessionAction#suppressAutonomousContinuation.
  ActionTicketController.accepted: ActionTicketController#accepted.
  SessionEvictionSnapshot.lastActivityAt: SessionEvictionSnapshot#lastActivityAt.
  SessionPassivationSnapshot: SessionPassivationSnapshot#
  DeliveryRecord.started: DeliveryRecord#started.
  SessionTurnPayload.preview: SessionTurnPayload#preview.
  ActionTicket.completed: ActionTicket#completed.
  ActionStore.remove: ActionStore#remove().
  RuntimeActivity: RuntimeActivity#
  SubmissionOutcome: SubmissionOutcome#
  ActionTicketController.completed: ActionTicketController#completed.
  RollbackProof: RollbackProof#
  TERMINAL_STATES: TERMINAL_STATES.
  ActionTicket.accepted: ActionTicket#accepted.
  QueuedMessageMutationStatus: QueuedMessageMutationStatus#
  Deferred.promise: Deferred#promise.
  Deferred.settle: Deferred#settle().
  RuntimeActivity.refinementApply: RuntimeActivity#refinementApply.
  ACTIVE_STATES: ACTIVE_STATES.
  CLEARABLE_STATES: CLEARABLE_STATES.
  LEGAL_TRANSITIONS: LEGAL_TRANSITIONS.
  ActionStore.snapshotActions: ActionStore#snapshotActions().
  WakePolicy: WakePolicy#
  DeliveryRecord.id: DeliveryRecord#id.
  DeliveryRecord.ownerActionId: DeliveryRecord#ownerActionId.
  SessionTurnPayload: SessionTurnPayload#
  SessionCommandPayload: SessionCommandPayload#
  DeliveryOutcome: DeliveryOutcome#
  ActionTicket: ActionTicket#
  Deferred.reject: Deferred#reject().
  ActionStore.nextTurnBoundary: ActionStore#nextTurnBoundary.
  ActionStore.whenRunIdle: ActionStore#whenRunIdle.
  RuntimeActivity.lowerAgentRun: RuntimeActivity#lowerAgentRun.
  RuntimeActivity.compaction: RuntimeActivity#compaction.
  RuntimeActivity.retry: RuntimeActivity#retry.
  RuntimeActivity.bash: RuntimeActivity#bash.
  RuntimeActivity.branchMutation: RuntimeActivity#branchMutation.
  RuntimeActivity.schedulerPauseCount: RuntimeActivity#schedulerPauseCount.
  RuntimeActivity.disposing: RuntimeActivity#disposing.
  SessionEvictionSnapshot: SessionEvictionSnapshot#
  WorkerEvictionSnapshot: WorkerEvictionSnapshot#
  SessionActionSnapshot.active.typeLiteral222.kind: SessionActionSnapshot#active.typeLiteral222:kind.
  SessionActionSnapshot.active.typeLiteral222.phase: SessionActionSnapshot#active.typeLiteral222:phase.
  ActionTicketController: ActionTicketController#
  WorkerEvictionSnapshot.lifecycle: WorkerEvictionSnapshot#lifecycle.
  WorkerEvictionSnapshot.isConnected: WorkerEvictionSnapshot#isConnected.
  WorkerEvictionSnapshot.isStopping: WorkerEvictionSnapshot#isStopping.
  WorkerEvictionSnapshot.hasOwnerClient: WorkerEvictionSnapshot#hasOwnerClient.
  WorkerEvictionSnapshot.isPreparingUpdateRestart: WorkerEvictionSnapshot#isPreparingUpdateRestart.
  SessionActionSnapshot.active.typeLiteral222.label: SessionActionSnapshot#active.typeLiteral222:label.
  RollbackProof.dispatchSettled: RollbackProof#dispatchSettled.
  RollbackProof.transcript: RollbackProof#transcript.
  AdmissionDisposition: AdmissionDisposition#
  ActionTicket.id: ActionTicket#id.
  Deferred: Deferred#
  SessionEvictionSnapshot.isSessionActive: SessionEvictionSnapshot#isSessionActive.
  SessionEvictionSnapshot.attachedClients: SessionEvictionSnapshot#attachedClients.
  SessionEvictionSnapshot.hasRegisteredHeartbeat: SessionEvictionSnapshot#hasRegisteredHeartbeat.
  SessionEvictionSnapshot.hasRegisteredCronJob: SessionEvictionSnapshot#hasRegisteredCronJob.
  SessionPassivationSnapshot.hasParent: SessionPassivationSnapshot#hasParent.
  SessionPassivationSnapshot.hasNonPassiveDescendants: SessionPassivationSnapshot#hasNonPassiveDescendants.
  SessionPassivationSnapshot.isHydrating: SessionPassivationSnapshot#isHydrating.
---
# Module: [`packages/coding-agent/src/core/session-action-store.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts)

## Classes
### `ActionLifecycle`
- def: [`packages/coding-agent/src/core/session-action-store.ts:57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L57)
- signature: `type ActionLifecycle`
- used by: [`lifecycle`](session-action-store.ts.md#SessionAction.lifecycle), [`transitionSessionAction`](session-action-store.ts.md#transitionSessionAction), [`TERMINAL_STATES`](session-action-store.ts.md#TERMINAL_STATES), [`ACTIVE_STATES`](session-action-store.ts.md#ACTIVE_STATES), [`CLEARABLE_STATES`](session-action-store.ts.md#CLEARABLE_STATES), [`LEGAL_TRANSITIONS`](session-action-store.ts.md#LEGAL_TRANSITIONS)  (1 test-only)

### `ActionStore`
- def: [`packages/coding-agent/src/core/session-action-store.ts:208`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L208)
- signature: `class ActionStore`
- members:
  - `actions(method)` — [`L322`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L322)
  - `actionsForMessage(method)` — [`L305`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L305)
  - `activeActions(method)` — [`L285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L285)
  - `assertNewAction(method)` — [`L331`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L331)
  - `clearableActions(method)` — [`L273`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L273)
  - `enqueue(method)` — [`L213`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L213)
  - `enqueueFront(method)` — [`L219`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L219)
  - `list(method)` — [`L327`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L327)
  - `moveQueued(method)` — [`L256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L256)
  - `ownedActions(method)` — [`L301`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L301)
  - `queuePreview(method)` — [`L289`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L289)
  - `queuedActions(method)` — [`L269`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L269)
  - `releaseTerminal(method)` — [`L312`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L312)
  - `remove(method)` — [`L235`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L235)
  - `rollback(method)` — [`L241`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L241)
  - `selectFirst(method)` — [`L227`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L227)
  - `snapshotActions(method)` — [`L277`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L277)
  - `swapQueued(method)` — [`L245`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L245)
  - `ticketFor(method)` — [`L295`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L295)
  - `unfinishedActions(method)` — [`L281`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L281)
  - `nextTurnBoundary` — [`L209`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L209)
  - `tickets` — [`L211`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L211)
  - `whenRunIdle` — [`L210`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L210)
- uses (calls/refs, reference-scoped): [`payload`](session-action-store.ts.md#SessionAction.payload), [`CustomMessage`](messages.ts.md#CustomMessage), [`lifecycle`](session-action-store.ts.md#SessionAction.lifecycle), [`kind`](session-action-store.ts.md#SessionTurnPayload.kind), [`kind`](session-action-store.ts.md#SessionCommandPayload.kind), [`id`](session-action-store.ts.md#SessionAction.id), [`message`](session-action-store.ts.md#DeliveryRecord.message), [`UserMessage`](../../../ai/src/types.ts.md#UserMessage), [`transitionSessionAction`](session-action-store.ts.md#transitionSessionAction), [`delivery`](session-action-store.ts.md#SessionAction.delivery), [`<constructor>`](session-action-store.ts.md#ActionTicketController.-constructor), [`records`](session-action-store.ts.md#SessionTurnPayload.records), [`text`](session-action-store.ts.md#SessionCommandPayload.text), [`text`](session-action-store.ts.md#SessionTurnPayload.text), [`SessionAction`](session-action-store.ts.md#SessionAction), [`DeliveryPolicy`](session-action-store.ts.md#DeliveryPolicy), [`isClearable`](session-action-store.ts.md#isClearable), [`preview`](session-action-store.ts.md#SessionTurnPayload.preview), [`RollbackProof`](session-action-store.ts.md#RollbackProof), [`TERMINAL_STATES`](session-action-store.ts.md#TERMINAL_STATES), [`ACTIVE_STATES`](session-action-store.ts.md#ACTIVE_STATES), [`ActionTicketController`](session-action-store.ts.md#ActionTicketController)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`waitForIdle`](agent-session.ts.md#AgentSession.waitForIdle), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`_actionStore`](agent-session.ts.md#AgentSession._actionStore), [`clearQueue`](agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`getFollowUpMessages`](agent-session.ts.md#AgentSession.getFollowUpMessages), [`waitForSessionInputCheckpoint`](agent-session.ts.md#AgentSession.waitForSessionInputCheckpoint), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`getSessionActionSnapshot`](agent-session.ts.md#AgentSession.getSessionActionSnapshot), [`<get>queuedActionCount`](agent-session.ts.md#AgentSession.-get-queuedActionCount), [`removeQueuedFollowUp`](agent-session.ts.md#AgentSession.removeQueuedFollowUp), [`_isBusyForSessionInput`](agent-session.ts.md#AgentSession._isBusyForSessionInput), [`getSteeringMessages`](agent-session.ts.md#AgentSession.getSteeringMessages), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`<get>hasPendingSessionWork`](agent-session.ts.md#AgentSession.-get-hasPendingSessionWork), [`_coalescedFollowUpOwner`](agent-session.ts.md#AgentSession._coalescedFollowUpOwner), [`<get>hasAcceptedPromptInFlight`](agent-session.ts.md#AgentSession.-get-hasAcceptedPromptInFlight), [`<get>unfinishedActionCount`](agent-session.ts.md#AgentSession.-get-unfinishedActionCount), [`<get>_steeringStopPending`](agent-session.ts.md#AgentSession.-get-_steeringStopPending), [`_hasCancelledDispatchCapture`](agent-session.ts.md#AgentSession._hasCancelledDispatchCapture), [`getFollowUpMessagePreviews`](agent-session.ts.md#AgentSession.getFollowUpMessagePreviews), [`_invalidateQueuedPromptPreparation`](agent-session.ts.md#AgentSession._invalidateQueuedPromptPreparation), [`_hasSelectableSessionInput`](agent-session.ts.md#AgentSession._hasSelectableSessionInput), [`getSteeringMessagePreviews`](agent-session.ts.md#AgentSession.getSteeringMessagePreviews), [`_rejectQueuedAgentMessageDeliveries`](agent-session.ts.md#AgentSession._rejectQueuedAgentMessageDeliveries)  (4 test-only)

### `ActionTicket`
- def: [`packages/coding-agent/src/core/session-action-store.ts:137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L137)
- signature: `interface ActionTicket`
- members:
  - `accepted` — [`L139`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L139)
  - `completed` — [`L141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L141)
  - `delivered` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L140)
  - `id` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L138)
- uses (calls/refs, reference-scoped): [`SubmissionOutcome`](session-action-store.ts.md#SubmissionOutcome), [`DeliveryOutcome`](session-action-store.ts.md#DeliveryOutcome)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`sendCustomMessage`](agent-session.ts.md#AgentSession.sendCustomMessage), [`_promptInjectedMessage`](agent-session.ts.md#AgentSession._promptInjectedMessage), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`<constructor>`](session-action-store.ts.md#ActionTicketController.-constructor), [`ticket`](session-action-store.ts.md#ActionTicketController.ticket)  (2 test-only)

### `ActionTicketController`
- def: [`packages/coding-agent/src/core/session-action-store.ts:176`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L176)
- signature: `class ActionTicketController`
- members:
  - `<constructor>(id: string)` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L182)
  - `rejectDelivered(method)` — [`L199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L199)
  - `settleAccepted(method)` — [`L191`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L191)
  - `settleCompleted(method)` — [`L203`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L203)
  - `settleDelivered(method)` — [`L195`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L195)
  - `accepted` — [`L178`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L178)
  - `completed` — [`L180`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L180)
  - `delivered` — [`L179`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L179)
  - `ticket` — [`L177`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L177)
- uses (calls/refs, reference-scoped): [`createDeferred`](session-action-store.ts.md#createDeferred), [`delivered`](session-action-store.ts.md#ActionTicket.delivered), [`completed`](session-action-store.ts.md#ActionTicket.completed), [`SubmissionOutcome`](session-action-store.ts.md#SubmissionOutcome), [`accepted`](session-action-store.ts.md#ActionTicket.accepted), [`promise`](session-action-store.ts.md#Deferred.promise), [`settle`](session-action-store.ts.md#Deferred.settle), [`ActionTicket`](session-action-store.ts.md#ActionTicket), [`DeliveryOutcome`](session-action-store.ts.md#DeliveryOutcome), [`reject`](session-action-store.ts.md#Deferred.reject), [`id`](session-action-store.ts.md#ActionTicket.id)
- used by: [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`enqueue`](session-action-store.ts.md#ActionStore.enqueue), [`enqueueFront`](session-action-store.ts.md#ActionStore.enqueueFront), [`ticketFor`](session-action-store.ts.md#ActionStore.ticketFor), [`tickets`](session-action-store.ts.md#ActionStore.tickets)  (2 test-only)

### `AdmissionDisposition`
- def: [`packages/coding-agent/src/core/session-action-store.ts:129`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L129)
- signature: `type AdmissionDisposition`
- used by: [`SubmissionOutcome`](session-action-store.ts.md#SubmissionOutcome)

### `Deferred`
- def: [`packages/coding-agent/src/core/session-action-store.ts:144`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L144)
- signature: `interface Deferred`
- members:
  - `reject(method)` — [`L147`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L147)
  - `settle(method)` — [`L146`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L146)
  - `promise` — [`L145`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L145)
- used by: [`<constructor>`](session-action-store.ts.md#ActionTicketController.-constructor), [`settleCompleted`](session-action-store.ts.md#ActionTicketController.settleCompleted), [`createDeferred`](session-action-store.ts.md#createDeferred), [`settleDelivered`](session-action-store.ts.md#ActionTicketController.settleDelivered), [`settleAccepted`](session-action-store.ts.md#ActionTicketController.settleAccepted), [`rejectDelivered`](session-action-store.ts.md#ActionTicketController.rejectDelivered)

### `DeliveryOutcome`
- def: [`packages/coding-agent/src/core/session-action-store.ts:135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L135)
- signature: `type DeliveryOutcome`
- used by: [`settleDelivered`](session-action-store.ts.md#ActionTicketController.settleDelivered), [`delivered`](session-action-store.ts.md#ActionTicket.delivered), [`delivered`](session-action-store.ts.md#ActionTicketController.delivered)

### `DeliveryPolicy`
- def: [`packages/coding-agent/src/core/session-action-store.ts:7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L7)
- signature: `type DeliveryPolicy`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`unfinishedActions`](session-action-store.ts.md#ActionStore.unfinishedActions), [`delivery`](session-action-store.ts.md#SessionAction.delivery), [`queuedActions`](session-action-store.ts.md#ActionStore.queuedActions), [`queuePreview`](session-action-store.ts.md#ActionStore.queuePreview), [`activeActions`](session-action-store.ts.md#ActionStore.activeActions), [`actions`](session-action-store.ts.md#ActionStore.actions), [`list`](session-action-store.ts.md#ActionStore.list), [`moveQueued`](session-action-store.ts.md#ActionStore.moveQueued), [`clearableActions`](session-action-store.ts.md#ActionStore.clearableActions), [`queuedMessageLaneDeliveryPolicy`](session-action-store.ts.md#queuedMessageLaneDeliveryPolicy), [`_deliveryPolicy`](agent-session.ts.md#AgentSession._deliveryPolicy), [`delivery`](agent-session.ts.md#SessionActionRecoveryAction.delivery)  (3 test-only)

### `DeliveryRecord`
- def: [`packages/coding-agent/src/core/session-action-store.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L33)
- signature: `interface DeliveryRecord`
- members:
  - `durable` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L38)
  - `id` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L34)
  - `message` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L36)
  - `ownerActionId` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L39)
  - `role` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L35)
  - `started` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L37)
- uses (calls/refs, reference-scoped): [`CustomMessage`](messages.ts.md#CustomMessage), [`UserMessage`](../../../ai/src/types.ts.md#UserMessage)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`waitForSessionInputCheckpoint`](agent-session.ts.md#AgentSession.waitForSessionInputCheckpoint), [`_clearQueuedAutonomousContinuations`](agent-session.ts.md#AgentSession._clearQueuedAutonomousContinuations), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`primaryDeliveryRecord`](agent-session.ts.md#primaryDeliveryRecord), [`<get>hasPendingSessionWork`](agent-session.ts.md#AgentSession.-get-hasPendingSessionWork), [`records`](session-action-store.ts.md#SessionTurnPayload.records), [`_createDeliveryRecord`](agent-session.ts.md#AgentSession._createDeliveryRecord), [`actionsForMessage`](session-action-store.ts.md#ActionStore.actionsForMessage), [`rollbackProof`](session-action-store.ts.md#transitionSessionAction.options-typeLiteral36.rollbackProof), [`source`](agent-session.ts.md#AgentSession._queuePreparedPrompt.options-typeLiteral1804.source), [`primaryRecords`](session-action-store.ts.md#primaryRecords), [`role`](agent-session.ts.md#SessionActionRecoveryRecord.role)  (2 test-only)

### `IdleEvictionMinutes`
- def: [`packages/coding-agent/src/core/session-action-store.ts:348`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L348)
- signature: `type IdleEvictionMinutes`
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`settings-selector.ts`](../modes/interactive/components/settings-selector.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-settings-selector.ts), [`passivateSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passivateSession), [`daemon-worker-protocol.ts`](../modes/daemon/daemon-worker-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-worker-protocol.ts), [`canEvictWorker`](session-action-store.ts.md#canEvictWorker), [`canPassivateSession`](session-action-store.ts.md#canPassivateSession), [`DaemonWorkerCommand`](../modes/daemon/daemon-worker-protocol.ts.md#DaemonWorkerCommand), [`passivateIdleChildren`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passivateIdleChildren), [`isIdleEvictionThresholdMet`](session-action-store.ts.md#isIdleEvictionThresholdMet), [`idleEvictionSweepIntervalMs`](../modes/daemon/daemon-supervisor.ts.md#idleEvictionSweepIntervalMs), [`idleEvictionMinutes`](../modes/interactive/components/settings-selector.ts.md#SettingsConfig.idleEvictionMinutes), [`onIdleEvictionMinutesChange`](../modes/interactive/components/settings-selector.ts.md#SettingsCallbacks.onIdleEvictionMinutesChange)

### `QueuedMessageLane`
- def: [`packages/coding-agent/src/core/session-action-store.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L10)
- signature: `type QueuedMessageLane`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`QueuedMessageMutation`](session-action-store.ts.md#QueuedMessageMutation), [`queuedMessageLaneDeliveryPolicy`](session-action-store.ts.md#queuedMessageLaneDeliveryPolicy), [`AgentConnectionQueuedMessageLane`](../modes/agent-connection/types.ts.md#AgentConnectionQueuedMessageLane)

### `QueuedMessageMutation`
- def: [`packages/coding-agent/src/core/session-action-store.ts:16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L16)
- signature: `type QueuedMessageMutation`
- uses (calls/refs, reference-scoped): [`ImageContent`](../../../ai/src/types.ts.md#ImageContent), [`QueuedMessageLane`](session-action-store.ts.md#QueuedMessageLane)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`DaemonCommand`](../modes/daemon/daemon-protocol.ts.md#DaemonCommand), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`AgentConnectionQueuedMessageMutation`](../modes/agent-connection/types.ts.md#AgentConnectionQueuedMessageMutation)  (1 test-only)

### `QueuedMessageMutationStatus`
- def: [`packages/coding-agent/src/core/session-action-store.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L20)
- signature: `type QueuedMessageMutationStatus`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`AgentConnectionQueuedMessageMutationStatus`](../modes/agent-connection/types.ts.md#AgentConnectionQueuedMessageMutationStatus)

### `RollbackProof`
- def: [`packages/coding-agent/src/core/session-action-store.ts:79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L79)
- signature: `interface RollbackProof`
- members:
  - `dispatchSettled` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L80)
  - `transcript` — [`L81`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L81)
- uses (calls/refs, reference-scoped): [`AgentMessage`](../../../agent/src/types.ts.md#AgentMessage)
- used by: [`rollbackProof`](session-action-store.ts.md#transitionSessionAction.options-typeLiteral36.rollbackProof), [`rollback`](session-action-store.ts.md#ActionStore.rollback)

### `RuntimeActivity`
- def: [`packages/coding-agent/src/core/session-action-store.ts:337`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L337)
- signature: `interface RuntimeActivity`
- members:
  - `bash` — [`L341`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L341)
  - `branchMutation` — [`L343`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L343)
  - `compaction` — [`L339`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L339)
  - `disposing` — [`L345`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L345)
  - `lowerAgentRun` — [`L338`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L338)
  - `refinementApply` — [`L342`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L342)
  - `retry` — [`L340`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L340)
  - `schedulerPauseCount` — [`L344`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L344)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`_runtimeActivity`](agent-session.ts.md#AgentSession._runtimeActivity), [`canSelectSessionAction`](session-action-store.ts.md#canSelectSessionAction)  (2 test-only)

### `SessionAction`
- def: [`packages/coding-agent/src/core/session-action-store.ts:67`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L67)
- signature: `interface SessionAction`
- members:
  - `agentMessageId` — [`L75`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L75)
  - `delivery` — [`L70`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L70)
  - `id` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L68)
  - `lifecycle` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L73) — documented in [packages-coding-agent-src-core-session-action-store.ts](../../../../../concepts/packages-coding-agent-src-core-session-action-store.ts.md)
  - `payload` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L72) — documented in [packages-coding-agent-src-core-session-action-store.ts](../../../../../concepts/packages-coding-agent-src-core-session-action-store.ts.md)
  - `queueKey` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L74)
  - `source` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L69)
  - `suppressAutonomousContinuation` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L76)
  - `wake` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L71)
- uses (calls/refs, reference-scoped): [`InputSource`](extensions/types.ts.md#InputSource), [`DeliveryPolicy`](session-action-store.ts.md#DeliveryPolicy), [`ActionLifecycle`](session-action-store.ts.md#ActionLifecycle), [`SessionActionPayload`](session-action-store.ts.md#SessionActionPayload), [`WakePolicy`](session-action-store.ts.md#WakePolicy)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_prompt`](agent-session.ts.md#AgentSession._prompt), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`acceptedBeforeCompletion`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`clearQueue`](agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`requestAbort`](agent-session.ts.md#AgentSession.requestAbort), [`getFollowUpMessages`](agent-session.ts.md#AgentSession.getFollowUpMessages), [`waitForSessionInputCheckpoint`](agent-session.ts.md#AgentSession.waitForSessionInputCheckpoint), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`_clearQueuedAutonomousContinuations`](agent-session.ts.md#AgentSession._clearQueuedAutonomousContinuations), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`getSessionActionSnapshot`](agent-session.ts.md#AgentSession.getSessionActionSnapshot), [`_clearQueuedGoalContexts`](agent-session.ts.md#AgentSession._clearQueuedGoalContexts), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`removeQueuedFollowUp`](agent-session.ts.md#AgentSession.removeQueuedFollowUp), [`primaryDeliveryRecord`](agent-session.ts.md#primaryDeliveryRecord), [`queuedAgentMessagePreview`](agent-session.ts.md#queuedAgentMessagePreview), [`unfinishedActions`](session-action-store.ts.md#ActionStore.unfinishedActions), [`QueuedSessionAction`](agent-session.ts.md#QueuedSessionAction), [`transitionSessionAction`](session-action-store.ts.md#transitionSessionAction), [`queuedActions`](session-action-store.ts.md#ActionStore.queuedActions), [`getSteeringMessages`](agent-session.ts.md#AgentSession.getSteeringMessages), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`<get>hasPendingSessionWork`](agent-session.ts.md#AgentSession.-get-hasPendingSessionWork), [`visibleSessionActionProjection`](agent-session.ts.md#visibleSessionActionProjection), [`_coalescedFollowUpOwner`](agent-session.ts.md#AgentSession._coalescedFollowUpOwner), [`<get>hasAcceptedPromptInFlight`](agent-session.ts.md#AgentSession.-get-hasAcceptedPromptInFlight), [`actionsForMessage`](session-action-store.ts.md#ActionStore.actionsForMessage), [`enqueue`](session-action-store.ts.md#ActionStore.enqueue), [`rollbackProof`](session-action-store.ts.md#transitionSessionAction.options-typeLiteral36.rollbackProof)  (+19 more; 6 test-only)

### `SessionActionPayload`
- def: [`packages/coding-agent/src/core/session-action-store.ts:55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L55)
- signature: `type SessionActionPayload`
- uses (calls/refs, reference-scoped): [`SessionCommandPayload`](session-action-store.ts.md#SessionCommandPayload), [`SessionTurnPayload`](session-action-store.ts.md#SessionTurnPayload)
- used by: [`SessionAction`](session-action-store.ts.md#SessionAction)

### `SessionActionSnapshot`
- def: [`packages/coding-agent/src/core/session-action-store.ts:22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L22)
- signature: `interface SessionActionSnapshot`
- members:
  - `active` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L26)
  - `followUps` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L25)
  - `kind` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L27)
  - `label` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L29)
  - `phase` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L28)
  - `queuedCount` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L23)
  - `steering` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L24)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`handleEvent`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleEvent), [`installAgentTelemetry`](telemetry.ts.md#installAgentTelemetry), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`createAgentObserveSummary`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.createAgentObserveSummary), [`summaryForInactiveSession`](../modes/daemon/daemon-session-list.ts.md#summaryForInactiveSession), [`summaryForUnifiedRecord`](../modes/agents-view/agents-view-state.ts.md#summaryForUnifiedRecord), [`daemon-session-list.ts`](../modes/daemon/daemon-session-list.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-session-list.ts), [`agentPeerSummary`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.agentPeerSummary), [`rpc-types.ts`](../modes/rpc/rpc-types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-rpc-rpc-types.ts), [`AgentConnectionSessionEvent`](../modes/agent-connection/types.ts.md#AgentConnectionSessionEvent), [`AgentSessionEvent`](agent-session.ts.md#AgentSessionEvent), [`getSessionActionSnapshot`](agent-session.ts.md#AgentSession.getSessionActionSnapshot), [`getSessionStatusLabel`](../modes/agents-view/agents-view-state.ts.md#getSessionStatusLabel), [`isSessionSummary`](../cli/daemon-command.ts.md#isSessionSummary), [`sessionActions`](../modes/daemon/daemon-session-list.ts.md#SessionSummary.sessionActions), [`handleSessionEvent`](../cli/daemon-command.ts.md#DaemonAttachTerminal.handleSessionEvent), [`hasInterruptibleWork`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.hasInterruptibleWork), [`_lastSessionActionSnapshot`](agent-session.ts.md#AgentSession._lastSessionActionSnapshot), [`sessionActions`](../modes/agent-connection/types.ts.md#AgentConnectionState.sessionActions), [`getQueuedActionCount`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.getQueuedActionCount), [`sessionActions`](../modes/rpc/rpc-types.ts.md#RpcSessionState.sessionActions)  (28 test-only)

### `SessionCommandPayload`
- def: [`packages/coding-agent/src/core/session-action-store.ts:49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L49)
- signature: `interface SessionCommandPayload`
- members:
  - `command` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L51)
  - `kind` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L50) — documented in [packages-coding-agent-src-core-session-action-store.ts](../../../../../concepts/packages-coding-agent-src-core-session-action-store.ts.md)
  - `text` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L52)
- uses (calls/refs, reference-scoped): [`SessionSlashCommand`](slash-commands.ts.md#SessionSlashCommand)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`clearQueue`](agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`requestAbort`](agent-session.ts.md#AgentSession.requestAbort), [`getFollowUpMessages`](agent-session.ts.md#AgentSession.getFollowUpMessages), [`waitForSessionInputCheckpoint`](agent-session.ts.md#AgentSession.waitForSessionInputCheckpoint), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`_clearQueuedAutonomousContinuations`](agent-session.ts.md#AgentSession._clearQueuedAutonomousContinuations), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`getSessionActionSnapshot`](agent-session.ts.md#AgentSession.getSessionActionSnapshot), [`_clearQueuedGoalContexts`](agent-session.ts.md#AgentSession._clearQueuedGoalContexts), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`removeQueuedFollowUp`](agent-session.ts.md#AgentSession.removeQueuedFollowUp), [`primaryDeliveryRecord`](agent-session.ts.md#primaryDeliveryRecord), [`queuedAgentMessagePreview`](agent-session.ts.md#queuedAgentMessagePreview), [`getSteeringMessages`](agent-session.ts.md#AgentSession.getSteeringMessages), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`<get>hasPendingSessionWork`](agent-session.ts.md#AgentSession.-get-hasPendingSessionWork), [`visibleSessionActionProjection`](agent-session.ts.md#visibleSessionActionProjection), [`_coalescedFollowUpOwner`](agent-session.ts.md#AgentSession._coalescedFollowUpOwner), [`<get>hasAcceptedPromptInFlight`](agent-session.ts.md#AgentSession.-get-hasAcceptedPromptInFlight), [`actionsForMessage`](session-action-store.ts.md#ActionStore.actionsForMessage), [`queuePreview`](session-action-store.ts.md#ActionStore.queuePreview), [`<get>_steeringStopPending`](agent-session.ts.md#AgentSession.-get-_steeringStopPending), [`_hasCancelledDispatchCapture`](agent-session.ts.md#AgentSession._hasCancelledDispatchCapture), [`primaryRecords`](session-action-store.ts.md#primaryRecords), [`_invalidateQueuedPromptPreparation`](agent-session.ts.md#AgentSession._invalidateQueuedPromptPreparation), [`PreparedCommandPayload`](agent-session.ts.md#PreparedCommandPayload), [`SessionActionPayload`](session-action-store.ts.md#SessionActionPayload)  (4 test-only)

### `SessionEvictionSnapshot`
- def: [`packages/coding-agent/src/core/session-action-store.ts:350`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L350)
- signature: `interface SessionEvictionSnapshot`
- members:
  - `attachedClients` — [`L352`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L352)
  - `hasRegisteredCronJob` — [`L354`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L354)
  - `hasRegisteredHeartbeat` — [`L353`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L353)
  - `isSessionActive` — [`L351`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L351)
  - `lastActivityAt` — [`L355`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L355)
- used by: [`runIdleEvictionSweep`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`passivateSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passivateSession), [`passivateIdleChildren`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passivateIdleChildren), [`isIdleEvictionThresholdMet`](session-action-store.ts.md#isIdleEvictionThresholdMet), [`sessions`](session-action-store.ts.md#WorkerEvictionSnapshot.sessions), [`SessionPassivationSnapshot`](session-action-store.ts.md#SessionPassivationSnapshot)  (1 test-only)

### `SessionPassivationSnapshot`
- def: [`packages/coding-agent/src/core/session-action-store.ts:358`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L358)
- signature: `interface SessionPassivationSnapshot`
- members:
  - `hasNonPassiveDescendants` — [`L360`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L360)
  - `hasParent` — [`L359`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L359)
  - `isHydrating` — [`L361`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L361)
- uses (calls/refs, reference-scoped): [`SessionEvictionSnapshot`](session-action-store.ts.md#SessionEvictionSnapshot)
- used by: [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`sessionPassivationSnapshot`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.sessionPassivationSnapshot), [`passivateSession`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.passivateSession), [`canPassivateSession`](session-action-store.ts.md#canPassivateSession)

### `SessionTurnPayload`
- def: [`packages/coding-agent/src/core/session-action-store.ts:42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L42)
- signature: `interface SessionTurnPayload`
- members:
  - `kind` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L43) — documented in [packages-coding-agent-src-core-session-action-store.ts](../../../../../concepts/packages-coding-agent-src-core-session-action-store.ts.md)
  - `preview` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L46)
  - `records` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L44)
  - `text` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L45)
- uses (calls/refs, reference-scoped): [`DeliveryRecord`](session-action-store.ts.md#DeliveryRecord)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_processAgentEvent`](agent-session.ts.md#AgentSession._processAgentEvent), [`_startPreparedTurnActions`](agent-session.ts.md#AgentSession._startPreparedTurnActions), [`_pumpSessionInputs`](agent-session.ts.md#AgentSession._pumpSessionInputs), [`getSessionActionRecoverySnapshot`](agent-session.ts.md#AgentSession.getSessionActionRecoverySnapshot), [`acceptedBeforeCompletion`](agent-session.ts.md#AgentSession._createPreparedTurnAction.options-typeLiteral696.acceptedBeforeCompletion), [`restoreSessionActions`](agent-session.ts.md#AgentSession.restoreSessionActions), [`_cancelSessionActions`](agent-session.ts.md#AgentSession._cancelSessionActions), [`mutateQueuedMessage`](agent-session.ts.md#AgentSession.mutateQueuedMessage), [`_handleAgentEvent`](agent-session.ts.md#AgentSession._handleAgentEvent), [`ticket`](agent-session.ts.md#AgentSession._admitSessionInput.typeLiteral1523.ticket), [`_executeSelectedSessionCommand`](agent-session.ts.md#AgentSession._executeSelectedSessionCommand), [`clearQueue`](agent-session.ts.md#AgentSession.clearQueue), [`clearQueuedUserMessagesMatching`](agent-session.ts.md#AgentSession.clearQueuedUserMessagesMatching), [`requestAbort`](agent-session.ts.md#AgentSession.requestAbort), [`getFollowUpMessages`](agent-session.ts.md#AgentSession.getFollowUpMessages), [`waitForSessionInputCheckpoint`](agent-session.ts.md#AgentSession.waitForSessionInputCheckpoint), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`_clearQueuedAutonomousContinuations`](agent-session.ts.md#AgentSession._clearQueuedAutonomousContinuations), [`getPendingNextTurnMessageSnapshots`](agent-session.ts.md#AgentSession.getPendingNextTurnMessageSnapshots), [`getSessionActionSnapshot`](agent-session.ts.md#AgentSession.getSessionActionSnapshot), [`_clearQueuedGoalContexts`](agent-session.ts.md#AgentSession._clearQueuedGoalContexts), [`source`](agent-session.ts.md#AgentSession._createSessionCommandAction.options-typeLiteral1777.source), [`removeQueuedFollowUp`](agent-session.ts.md#AgentSession.removeQueuedFollowUp), [`primaryDeliveryRecord`](agent-session.ts.md#primaryDeliveryRecord), [`queuedAgentMessagePreview`](agent-session.ts.md#queuedAgentMessagePreview), [`getSteeringMessages`](agent-session.ts.md#AgentSession.getSteeringMessages), [`_capturingCancelledAction`](agent-session.ts.md#AgentSession._capturingCancelledAction), [`<get>hasPendingSessionWork`](agent-session.ts.md#AgentSession.-get-hasPendingSessionWork), [`visibleSessionActionProjection`](agent-session.ts.md#visibleSessionActionProjection), [`_coalescedFollowUpOwner`](agent-session.ts.md#AgentSession._coalescedFollowUpOwner), [`<get>hasAcceptedPromptInFlight`](agent-session.ts.md#AgentSession.-get-hasAcceptedPromptInFlight), [`actionsForMessage`](session-action-store.ts.md#ActionStore.actionsForMessage), [`queuePreview`](session-action-store.ts.md#ActionStore.queuePreview), [`<get>_steeringStopPending`](agent-session.ts.md#AgentSession.-get-_steeringStopPending), [`_hasCancelledDispatchCapture`](agent-session.ts.md#AgentSession._hasCancelledDispatchCapture), [`primaryRecords`](session-action-store.ts.md#primaryRecords), [`_invalidateQueuedPromptPreparation`](agent-session.ts.md#AgentSession._invalidateQueuedPromptPreparation), [`PreparedTurnPayload`](agent-session.ts.md#PreparedTurnPayload), [`SessionActionPayload`](session-action-store.ts.md#SessionActionPayload)  (4 test-only)

### `SubmissionOutcome`
- def: [`packages/coding-agent/src/core/session-action-store.ts:130`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L130)
- signature: `type SubmissionOutcome`
- uses (calls/refs, reference-scoped): [`AdmissionDisposition`](session-action-store.ts.md#AdmissionDisposition)
- used by: [`settleAccepted`](session-action-store.ts.md#ActionTicketController.settleAccepted), [`accepted`](session-action-store.ts.md#ActionTicketController.accepted), [`accepted`](session-action-store.ts.md#ActionTicket.accepted)

### `WakePolicy`
- def: [`packages/coding-agent/src/core/session-action-store.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L8)
- signature: `type WakePolicy`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`wake`](session-action-store.ts.md#SessionAction.wake), [`wake`](agent-session.ts.md#SessionActionRecoveryAction.wake)

### `WorkerEvictionSnapshot`
- def: [`packages/coding-agent/src/core/session-action-store.ts:364`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L364)
- signature: `interface WorkerEvictionSnapshot`
- members:
  - `hasOwnerClient` — [`L368`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L368)
  - `isConnected` — [`L366`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L366)
  - `isPreparingUpdateRestart` — [`L369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L369)
  - `isStopping` — [`L367`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L367)
  - `lifecycle` — [`L365`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L365)
  - `sessions` — [`L370`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L370)
- uses (calls/refs, reference-scoped): [`SessionEvictionSnapshot`](session-action-store.ts.md#SessionEvictionSnapshot)
- used by: [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`runIdleEvictionSweep`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.runIdleEvictionSweep), [`workerEvictionSnapshot`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.workerEvictionSnapshot), [`canEvictWorker`](session-action-store.ts.md#canEvictWorker)  (1 test-only)

## Functions
- `canEvictWorker(worker: WorkerEvictionSnapshot, idleEvictionMinutes: IdleEvictionMinutes, now?: number)` — [`L406`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L406) — Pure whole-tree residency policy. Callers must supply supervisor-owned attachment state.
- `canPassivateSession(session: SessionPassivationSnapshot, idleEvictionMinutes: IdleEvictionMinutes, now?: number)` — [`L392`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L392) — Pure per-node residency policy. Roots remain owned by whole-worker eviction.
- `canSelectSessionAction(activity: RuntimeActivity)` — [`L424`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L424)
- `createDeferred()` — [`L150`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L150)
- `isClearable(action: SessionAction<SessionActionPayload>)` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L88)
- `isIdleEvictionThresholdMet(session: SessionEvictionSnapshot, idleEvictionMinutes: IdleEvictionMinutes, now: number)` — [`L373`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L373)
- `primaryRecords(action: SessionAction<SessionActionPayload>)` — [`L103`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L103)
- `queuedMessageLaneDeliveryPolicy(lane: QueuedMessageLane)` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L12)
- `transitionSessionAction(action: SessionAction<SessionActionPayload>, next: ActionLifecycle, options?: { rollbackProof?: RollbackProof | undefined; })` — [`L107`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L107)

## Module values
- `ACTIVE_STATES` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L85)
- `CLEARABLE_STATES` — [`L86`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L86)
- `LEGAL_TRANSITIONS` — [`L92`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L92)
- `TERMINAL_STATES` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L84)
- `rollbackProof` — [`L110`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-action-store.ts#L110)

