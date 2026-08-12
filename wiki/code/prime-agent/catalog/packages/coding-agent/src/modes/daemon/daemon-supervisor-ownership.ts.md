---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-supervisor-ownership.ts`/
symbols:
  acquireDaemonSupervisorOwnership: acquireDaemonSupervisorOwnership().
  persistDaemonStartupFenceFromOwner: persistDaemonStartupFenceFromOwner().
  DaemonShutdownAdmission.assertOrRenew: DaemonShutdownAdmission#assertOrRenew().
  acquireDaemonShutdownAdmission: acquireDaemonShutdownAdmission().
  assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.socketPath: assertDaemonSupervisorOwnerCurrent().(owner)typeLiteral90:socketPath.
  isDaemonSupervisorOwnerRecord: isDaemonSupervisorOwnerRecord().
  writeOwnerScope: writeOwnerScope().
  waitForDaemonStartupFence: waitForDaemonStartupFence().
  DaemonSupervisorOwnership.release: DaemonSupervisorOwnership#release().
  readStartupFence: readStartupFence().
  ProcessIdentity.processStartId: ProcessIdentity#processStartId.
  DaemonSupervisorOwnerRecord.generation: DaemonSupervisorOwnerRecord#generation.
  mutateDaemonSupervisorOwner: mutateDaemonSupervisorOwner().
  readShutdownAdmission: readShutdownAdmission().
  ProcessIdentity.pid: ProcessIdentity#pid.
  DaemonShutdownAdmission.release: DaemonShutdownAdmission#release().
  DaemonSupervisorOwnership.updatePhase: DaemonSupervisorOwnership#updatePhase().
  isDaemonSupervisorOwnerScope: isDaemonSupervisorOwnerScope().
  AcquireDaemonSupervisorOwnershipOptions.generation: AcquireDaemonSupervisorOwnershipOptions#generation.
  withDaemonSupervisorRegistryGuard: withDaemonSupervisorRegistryGuard().
  AcquireDaemonSupervisorOwnershipOptions.socketPath: AcquireDaemonSupervisorOwnershipOptions#socketPath.
  AcquireDaemonSupervisorOwnershipOptions.descriptorDir: AcquireDaemonSupervisorOwnershipOptions#descriptorDir.
  AcquireDaemonSupervisorOwnershipOptions.agentDir: AcquireDaemonSupervisorOwnershipOptions#agentDir.
  AcquireDaemonSupervisorOwnershipOptions.appVersion: AcquireDaemonSupervisorOwnershipOptions#appVersion.
  DaemonSupervisorOwnerRecord: DaemonSupervisorOwnerRecord#
  AcquireDaemonSupervisorOwnershipOptions.registryDir: AcquireDaemonSupervisorOwnershipOptions#registryDir.
  isProcessIdentityAlive: isProcessIdentityAlive().
  sameOwnerRecord: sameOwnerRecord().
  readActiveShutdownAdmission: readActiveShutdownAdmission().
  DaemonSupervisorOwnerRecord.socketPath: DaemonSupervisorOwnerRecord#socketPath.
  DaemonSupervisorOwnerRecord.token: DaemonSupervisorOwnerRecord#token.
  DaemonSupervisorOwnership.assertCurrent: DaemonSupervisorOwnership#assertCurrent().
  DaemonShutdownAdmission.-constructor: DaemonShutdownAdmission#`<constructor>`().
  matchesExactProcessIdentity: matchesExactProcessIdentity().
  isDaemonShutdownAdmissionActive: isDaemonShutdownAdmissionActive().
  defaultDaemonSupervisorRegistryDir: defaultDaemonSupervisorRegistryDir().
  readOwnerRecordForScope: readOwnerRecordForScope().
  readOwnerScope: readOwnerScope().
  readOwnerRecord: readOwnerRecord().
  ownerConflicts: ownerConflicts().
  DaemonSupervisorOwnerRecord.phase: DaemonSupervisorOwnerRecord#phase.
  DaemonShutdownAdmissionRecord: DaemonShutdownAdmissionRecord#
  DaemonSupervisorAlreadyRunningError.-constructor: DaemonSupervisorAlreadyRunningError#`<constructor>`().
  OWNER_VERSION: OWNER_VERSION.
  DaemonSupervisorOwnerScope: DaemonSupervisorOwnerScope#
  writeOwnerRecord: writeOwnerRecord().
  DaemonStartupFenceRecord: DaemonStartupFenceRecord#
  shutdownAdmissionPath: shutdownAdmissionPath().
  DaemonSupervisorHelloIdentity.supervisorPid: DaemonSupervisorHelloIdentity#supervisorPid.
  normalizeSocketPath: normalizeSocketPath().
  requireOwnerRecord: requireOwnerRecord().
  ProcessIdentity: ProcessIdentity#
  DaemonSupervisorOwnerRecord.updatedAt: DaemonSupervisorOwnerRecord#updatedAt.
  DaemonShutdownAdmissionRecord.token: DaemonShutdownAdmissionRecord#token.
  DaemonShutdownAdmissionRecord.expiresAt: DaemonShutdownAdmissionRecord#expiresAt.
  DaemonSupervisorOwnerScope.socketPath: DaemonSupervisorOwnerScope#socketPath.
  DaemonSupervisorHelloIdentity.supervisorGeneration: DaemonSupervisorHelloIdentity#supervisorGeneration.
  DaemonSupervisorHelloIdentity.supervisorOwnerToken: DaemonSupervisorHelloIdentity#supervisorOwnerToken.
  DaemonSupervisorHelloIdentity.supervisorProcessStartId: DaemonSupervisorHelloIdentity#supervisorProcessStartId.
  DaemonSupervisorHelloIdentity.supervisorSocketPath: DaemonSupervisorHelloIdentity#supervisorSocketPath.
  writeJsonAtomically: writeJsonAtomically().
  startupFencePath: startupFencePath().
  DaemonSupervisorOwnerScope.descriptorDir: DaemonSupervisorOwnerScope#descriptorDir.
  DaemonStartupFenceRecord.token: DaemonStartupFenceRecord#token.
  DaemonSupervisorOwnershipLostError.-constructor: DaemonSupervisorOwnershipLostError#`<constructor>`().
  DaemonSupervisorOwnership.released: DaemonSupervisorOwnership#released.
  DaemonShutdownAdmission.refreshTimer: DaemonShutdownAdmission#refreshTimer.
  assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.generation: assertDaemonSupervisorOwnerCurrent().(owner)typeLiteral90:generation.
  ownerDirectoryPath: ownerDirectoryPath().
  DaemonSupervisorOwnership.-constructor: DaemonSupervisorOwnership#`<constructor>`().
  ownerRecordFingerprint: ownerRecordFingerprint().
  DaemonSupervisorOwnerRecord.version: DaemonSupervisorOwnerRecord#version.
  DaemonSupervisorOwnerRecord.role: DaemonSupervisorOwnerRecord#role.
  DaemonSupervisorOwnerRecord.descriptorDir: DaemonSupervisorOwnerRecord#descriptorDir.
  DaemonSupervisorOwnerScope.generation: DaemonSupervisorOwnerScope#generation.
  DaemonStartupFenceRecord.socketPath: DaemonStartupFenceRecord#socketPath.
  DaemonShutdownAdmissionError.-constructor: DaemonShutdownAdmissionError#`<constructor>`().
  DaemonShutdownAdmission.released: DaemonShutdownAdmission#released.
  DaemonShutdownAdmission.refreshPromise: DaemonShutdownAdmission#refreshPromise.
  isProcessAlive: isProcessAlive().
  REGISTRY_LOCK_RETRY_MS: REGISTRY_LOCK_RETRY_MS.
  SHUTDOWN_ADMISSION_LEASE_MS: SHUTDOWN_ADMISSION_LEASE_MS.
  DaemonSupervisorOwnerPhase: DaemonSupervisorOwnerPhase#
  DaemonSupervisorOwnerRecord.agentDir: DaemonSupervisorOwnerRecord#agentDir.
  DaemonSupervisorOwnerRecord.appVersion: DaemonSupervisorOwnerRecord#appVersion.
  DaemonSupervisorOwnerRecord.createdAt: DaemonSupervisorOwnerRecord#createdAt.
  DaemonShutdownAdmissionRecord.updatedAt: DaemonShutdownAdmissionRecord#updatedAt.
  DaemonSupervisorOwnerScope.version: DaemonSupervisorOwnerScope#version.
  DaemonSupervisorOwnerScope.role: DaemonSupervisorOwnerScope#role.
  DaemonSupervisorOwnerScope.token: DaemonSupervisorOwnerScope#token.
  DaemonStartupFenceRecord.version: DaemonStartupFenceRecord#version.
  DaemonStartupFenceRecord.ownerToken: DaemonStartupFenceRecord#ownerToken.
  DaemonStartupFenceRecord.supervisorGeneration: DaemonStartupFenceRecord#supervisorGeneration.
  DaemonStartupFenceRecord.createdAt: DaemonStartupFenceRecord#createdAt.
  DaemonShutdownAdmission.lost: DaemonShutdownAdmission#lost.
  assertDaemonSupervisorOwnerCurrent: assertDaemonSupervisorOwnerCurrent().
  assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.pid: assertDaemonSupervisorOwnerCurrent().(owner)typeLiteral90:pid.
  assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.processStartId: assertDaemonSupervisorOwnerCurrent().(owner)typeLiteral90:processStartId.
  canonicalizeFilesystemPath: canonicalizeFilesystemPath().
  listOwnerDirectories: listOwnerDirectories().
  delay: delay().
  DAEMON_SUPERVISOR_REGISTRY_DIR_ENV: DAEMON_SUPERVISOR_REGISTRY_DIR_ENV.
  REGISTRY_LOCK_STALE_MS: REGISTRY_LOCK_STALE_MS.
  REGISTRY_LOCK_UPDATE_MS: REGISTRY_LOCK_UPDATE_MS.
  REGISTRY_LOCK_RETRIES: REGISTRY_LOCK_RETRIES.
  STARTUP_FENCE_POLL_MS: STARTUP_FENCE_POLL_MS.
  SHUTDOWN_ADMISSION_FILE_NAME: SHUTDOWN_ADMISSION_FILE_NAME.
  SHUTDOWN_ADMISSION_REFRESH_MS: SHUTDOWN_ADMISSION_REFRESH_MS.
  SHUTDOWN_ADMISSION_WAIT_MS: SHUTDOWN_ADMISSION_WAIT_MS.
  DaemonShutdownAdmissionRecord.version: DaemonShutdownAdmissionRecord#version.
  DaemonShutdownAdmissionRecord.createdAt: DaemonShutdownAdmissionRecord#createdAt.
  DaemonSupervisorHelloIdentity: DaemonSupervisorHelloIdentity#
  AcquireDaemonSupervisorOwnershipOptions: AcquireDaemonSupervisorOwnershipOptions#
  DaemonSupervisorOwnership: DaemonSupervisorOwnership#
  DaemonShutdownAdmission: DaemonShutdownAdmission#
  DaemonSupervisorAlreadyRunningError: DaemonSupervisorAlreadyRunningError#
  DaemonSupervisorAlreadyRunningError.code: DaemonSupervisorAlreadyRunningError#code.
  DaemonSupervisorOwnershipLostError: DaemonSupervisorOwnershipLostError#
  DaemonSupervisorOwnershipLostError.code: DaemonSupervisorOwnershipLostError#code.
  DaemonShutdownAdmissionError: DaemonShutdownAdmissionError#
  DaemonShutdownAdmissionError.code: DaemonShutdownAdmissionError#code.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts)

## Classes
### `AcquireDaemonSupervisorOwnershipOptions`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:85`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L85)
- signature: `interface AcquireDaemonSupervisorOwnershipOptions`
- members:
  - `agentDir` — [`L88`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L88)
  - `appVersion` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L90)
  - `descriptorDir` — [`L87`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L87)
  - `generation` — [`L89`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L89)
  - `registryDir` — [`L91`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L91)
  - `socketPath` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L86)
- used by: [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership)  (3 test-only)

### `DaemonShutdownAdmission`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:182`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L182)
- signature: `class DaemonShutdownAdmission`
- members:
  - `<constructor>(record: DaemonShutdownAdmissionRecord, registryDir: string)` — [`L188`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L188)
  - `assertOrRenew(method)` — [`L202`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L202)
  - `release(method)` — [`L232`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L232)
  - `lost` — [`L184`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L184)
  - `refreshPromise` — [`L185`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L185)
  - `refreshTimer` — [`L186`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L186)
  - `released` — [`L183`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L183)
- uses (calls/refs, reference-scoped): [`processStartId`](daemon-supervisor-ownership.ts.md#ProcessIdentity.processStartId), [`readShutdownAdmission`](daemon-supervisor-ownership.ts.md#readShutdownAdmission), [`pid`](daemon-supervisor-ownership.ts.md#ProcessIdentity.pid), [`withDaemonSupervisorRegistryGuard`](daemon-supervisor-ownership.ts.md#withDaemonSupervisorRegistryGuard), [`matchesExactProcessIdentity`](daemon-supervisor-ownership.ts.md#matchesExactProcessIdentity), [`DaemonShutdownAdmissionRecord`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionRecord), [`shutdownAdmissionPath`](daemon-supervisor-ownership.ts.md#shutdownAdmissionPath), [`expiresAt`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionRecord.expiresAt), [`token`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionRecord.token), [`writeJsonAtomically`](daemon-supervisor-ownership.ts.md#writeJsonAtomically), [`<constructor>`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionError.-constructor), [`SHUTDOWN_ADMISSION_LEASE_MS`](daemon-supervisor-ownership.ts.md#SHUTDOWN_ADMISSION_LEASE_MS), [`updatedAt`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionRecord.updatedAt), [`SHUTDOWN_ADMISSION_REFRESH_MS`](daemon-supervisor-ownership.ts.md#SHUTDOWN_ADMISSION_REFRESH_MS)
- used by: [`originActiveSessionId`](../../package-manager-cli.ts.md#runDaemonUpdateRestartCoordinator.options-typeLiteral607.originActiveSessionId), [`acquireDaemonShutdownAdmission`](daemon-supervisor-ownership.ts.md#acquireDaemonShutdownAdmission), [`runShutdownAll`](../../cli/daemon-ps.ts.md#runShutdownAll)  (1 test-only)

### `DaemonShutdownAdmissionError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:112`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L112)
- signature: `class DaemonShutdownAdmissionError`
- members:
  - `<constructor>(message?: string)` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L115)
  - `code` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L113)
- used by: [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership), [`assertOrRenew`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmission.assertOrRenew)

### `DaemonShutdownAdmissionRecord`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L51)
- signature: `interface DaemonShutdownAdmissionRecord`
- members:
  - `createdAt` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L54)
  - `expiresAt` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L56)
  - `token` — [`L53`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L53)
  - `updatedAt` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L55)
  - `version` — [`L52`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L52)
- uses (calls/refs, reference-scoped): [`ProcessIdentity`](daemon-supervisor-ownership.ts.md#ProcessIdentity)
- used by: [`assertOrRenew`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmission.assertOrRenew), [`acquireDaemonShutdownAdmission`](daemon-supervisor-ownership.ts.md#acquireDaemonShutdownAdmission), [`readShutdownAdmission`](daemon-supervisor-ownership.ts.md#readShutdownAdmission), [`release`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmission.release), [`readActiveShutdownAdmission`](daemon-supervisor-ownership.ts.md#readActiveShutdownAdmission), [`<constructor>`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmission.-constructor)

### `DaemonStartupFenceRecord`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:68`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L68)
- signature: `interface DaemonStartupFenceRecord`
- members:
  - `createdAt` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L74)
  - `ownerToken` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L71)
  - `socketPath` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L72)
  - `supervisorGeneration` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L73)
  - `token` — [`L70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L70)
  - `version` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L69)
- uses (calls/refs, reference-scoped): [`ProcessIdentity`](daemon-supervisor-ownership.ts.md#ProcessIdentity)
- used by: [`persistDaemonStartupFenceFromOwner`](daemon-supervisor-ownership.ts.md#persistDaemonStartupFenceFromOwner), [`waitForDaemonStartupFence`](daemon-supervisor-ownership.ts.md#waitForDaemonStartupFence), [`readStartupFence`](daemon-supervisor-ownership.ts.md#readStartupFence)

### `DaemonSupervisorAlreadyRunningError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L94)
- signature: `class DaemonSupervisorAlreadyRunningError`
- members:
  - `<constructor>(owner: DaemonSupervisorOwnerRecord)` — [`L97`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L97)
  - `code` — [`L95`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L95)
- uses (calls/refs, reference-scoped): [`generation`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.generation), [`DaemonSupervisorOwnerRecord`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord), [`socketPath`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.socketPath)
- used by: [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership)

### `DaemonSupervisorHelloIdentity`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L77)
- signature: `interface DaemonSupervisorHelloIdentity`
- members:
  - `supervisorGeneration` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L78)
  - `supervisorOwnerToken` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L79)
  - `supervisorPid` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L80)
  - `supervisorProcessStartId` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L81)
  - `supervisorSocketPath` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L82)
- used by: [`persistDaemonStartupFenceFromOwner`](daemon-supervisor-ownership.ts.md#persistDaemonStartupFenceFromOwner)  (1 test-only)

### `DaemonSupervisorOwnerPhase`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L30)
- signature: `type DaemonSupervisorOwnerPhase`
- used by: [`updatePhase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.updatePhase), [`phase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.phase)

### `DaemonSupervisorOwnerRecord`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L37)
- signature: `interface DaemonSupervisorOwnerRecord`
- members:
  - `agentDir` — [`L44`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L44)
  - `appVersion` — [`L45`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L45)
  - `createdAt` — [`L47`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L47)
  - `descriptorDir` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L43)
  - `generation` — [`L41`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L41)
  - `phase` — [`L46`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L46)
  - `role` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L39)
  - `socketPath` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L42)
  - `token` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L40)
  - `updatedAt` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L48)
  - `version` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L38)
- uses (calls/refs, reference-scoped): [`ProcessIdentity`](daemon-supervisor-ownership.ts.md#ProcessIdentity), [`DaemonSupervisorOwnerPhase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerPhase)
- used by: [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership), [`handleConnection`](daemon-supervisor.ts.md#DaemonSupervisor.handleConnection), [`persistDaemonStartupFenceFromOwner`](daemon-supervisor-ownership.ts.md#persistDaemonStartupFenceFromOwner), [`isDaemonSupervisorOwnerRecord`](daemon-supervisor-ownership.ts.md#isDaemonSupervisorOwnerRecord), [`socketPath`](daemon-supervisor-ownership.ts.md#assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.socketPath), [`writeOwnerScope`](daemon-supervisor-ownership.ts.md#writeOwnerScope), [`release`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.release), [`mutateDaemonSupervisorOwner`](daemon-supervisor-ownership.ts.md#mutateDaemonSupervisorOwner), [`supervisorSocketPath`](daemon-supervisor.ts.md#DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorSocketPath), [`updatePhase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.updatePhase), [`sameOwnerRecord`](daemon-supervisor-ownership.ts.md#sameOwnerRecord), [`assertCurrent`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.assertCurrent), [`readOwnerRecordForScope`](daemon-supervisor-ownership.ts.md#readOwnerRecordForScope), [`readOwnerRecord`](daemon-supervisor-ownership.ts.md#readOwnerRecord), [`<constructor>`](daemon-supervisor-ownership.ts.md#DaemonSupervisorAlreadyRunningError.-constructor), [`writeOwnerRecord`](daemon-supervisor-ownership.ts.md#writeOwnerRecord), [`requireOwnerRecord`](daemon-supervisor-ownership.ts.md#requireOwnerRecord), [`<constructor>`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.-constructor), [`ownerRecordFingerprint`](daemon-supervisor-ownership.ts.md#ownerRecordFingerprint)  (2 test-only)

### `DaemonSupervisorOwnerScope`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:59`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L59)
- signature: `interface DaemonSupervisorOwnerScope`
- members:
  - `descriptorDir` — [`L65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L65)
  - `generation` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L63)
  - `role` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L61)
  - `socketPath` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L64)
  - `token` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L62)
  - `version` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L60)
- used by: [`persistDaemonStartupFenceFromOwner`](daemon-supervisor-ownership.ts.md#persistDaemonStartupFenceFromOwner), [`writeOwnerScope`](daemon-supervisor-ownership.ts.md#writeOwnerScope), [`isDaemonSupervisorOwnerScope`](daemon-supervisor-ownership.ts.md#isDaemonSupervisorOwnerScope), [`readOwnerRecordForScope`](daemon-supervisor-ownership.ts.md#readOwnerRecordForScope), [`readOwnerScope`](daemon-supervisor-ownership.ts.md#readOwnerScope), [`ownerConflicts`](daemon-supervisor-ownership.ts.md#ownerConflicts)

### `DaemonSupervisorOwnership`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:121`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L121)
- signature: `class DaemonSupervisorOwnership`
- members:
  - `<constructor>(record: DaemonSupervisorOwnerRecord, registryDir: string, ownerDirectory: string)` — [`L124`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L124)
  - `assertCurrent(method)` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L130)
  - `release(method)` — [`L159`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L159)
  - `updatePhase(method)` — [`L140`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L140)
  - `released` — [`L122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L122)
- uses (calls/refs, reference-scoped): [`generation`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.generation), [`mutateDaemonSupervisorOwner`](daemon-supervisor-ownership.ts.md#mutateDaemonSupervisorOwner), [`withDaemonSupervisorRegistryGuard`](daemon-supervisor-ownership.ts.md#withDaemonSupervisorRegistryGuard), [`DaemonSupervisorOwnerRecord`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord), [`sameOwnerRecord`](daemon-supervisor-ownership.ts.md#sameOwnerRecord), [`socketPath`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.socketPath), [`token`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.token), [`readOwnerRecord`](daemon-supervisor-ownership.ts.md#readOwnerRecord), [`phase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.phase), [`updatedAt`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord.updatedAt), [`<constructor>`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnershipLostError.-constructor), [`DaemonSupervisorOwnerPhase`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerPhase)
- used by: [`start`](daemon-supervisor.ts.md#DaemonSupervisor.start), [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership), [`shutdown`](daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`cleanupSupervisorResourcesOnce`](daemon-supervisor.ts.md#DaemonSupervisor.cleanupSupervisorResourcesOnce), [`assertCurrentOwnership`](daemon-supervisor.ts.md#DaemonSupervisor.assertCurrentOwnership)  (3 test-only)

### `DaemonSupervisorOwnershipLostError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:103`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L103)
- signature: `class DaemonSupervisorOwnershipLostError`
- members:
  - `<constructor>(generation: string)` — [`L106`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L106)
  - `code` — [`L104`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L104)
- used by: [`socketPath`](daemon-supervisor-ownership.ts.md#assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.socketPath), [`assertCurrent`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnership.assertCurrent)

### `ProcessIdentity`
- def: [`packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts:32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L32)
- signature: `interface ProcessIdentity`
- members:
  - `pid` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L33)
  - `processStartId` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L34)
- used by: [`acquireDaemonSupervisorOwnership`](daemon-supervisor-ownership.ts.md#acquireDaemonSupervisorOwnership), [`handleConnection`](daemon-supervisor.ts.md#DaemonSupervisor.handleConnection), [`persistDaemonStartupFenceFromOwner`](daemon-supervisor-ownership.ts.md#persistDaemonStartupFenceFromOwner), [`assertOrRenew`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmission.assertOrRenew), [`isDaemonSupervisorOwnerRecord`](daemon-supervisor-ownership.ts.md#isDaemonSupervisorOwnerRecord), [`socketPath`](daemon-supervisor-ownership.ts.md#assertDaemonSupervisorOwnerCurrent.owner-typeLiteral90.socketPath), [`waitForDaemonStartupFence`](daemon-supervisor-ownership.ts.md#waitForDaemonStartupFence), [`readStartupFence`](daemon-supervisor-ownership.ts.md#readStartupFence), [`supervisorSocketPath`](daemon-supervisor.ts.md#DaemonSupervisor.supervisorAuthenticationClaim.typeLiteral584.supervisorSocketPath), [`readShutdownAdmission`](daemon-supervisor-ownership.ts.md#readShutdownAdmission), [`DaemonSupervisorOwnerRecord`](daemon-supervisor-ownership.ts.md#DaemonSupervisorOwnerRecord), [`isProcessIdentityAlive`](daemon-supervisor-ownership.ts.md#isProcessIdentityAlive), [`sameOwnerRecord`](daemon-supervisor-ownership.ts.md#sameOwnerRecord), [`matchesExactProcessIdentity`](daemon-supervisor-ownership.ts.md#matchesExactProcessIdentity), [`DaemonShutdownAdmissionRecord`](daemon-supervisor-ownership.ts.md#DaemonShutdownAdmissionRecord), [`DaemonStartupFenceRecord`](daemon-supervisor-ownership.ts.md#DaemonStartupFenceRecord)  (2 test-only)

## Functions
- `acquireDaemonShutdownAdmission()` — [`L392`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L392)
- `acquireDaemonSupervisorOwnership(options: AcquireDaemonSupervisorOwnershipOptions)` — [`L303`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L303)
- `assertDaemonSupervisorOwnerCurrent(owner: { generation: string; pid: number; processStartId?: string | undefined; socketPath: string; }, validatedFingerprint?: string | undefined)` — [`L365`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L365)
- `canonicalizeFilesystemPath(path: string)` — [`L555`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L555)
- `defaultDaemonSupervisorRegistryDir(environment?: ProcessEnv)` — [`L249`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L249)
- `delay(ms: number)` — [`L805`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L805)
- `isDaemonShutdownAdmissionActive()` — [`L420`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L420)
- `isDaemonSupervisorOwnerRecord(value: unknown)` — [`L648`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L648)
- `isDaemonSupervisorOwnerScope(value: unknown)` — [`L683`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L683)
- `isProcessAlive(pid: number)` — [`L539`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L539)
- `isProcessIdentityAlive(identity: ProcessIdentity)` — [`L521`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L521)
- `listOwnerDirectories(registryDir: string)` — [`L596`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L596)
- `matchesExactProcessIdentity(identity: ProcessIdentity)` — [`L532`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L532)
- `mutateDaemonSupervisorOwner(generation: string, expectedToken: string, mutation: (owner: DaemonSupervisorOwnerRecord) => void, registryDir?: string)` — [`L274`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L274)
- `normalizeSocketPath(socketPath: string)` — [`L548`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L548)
- `ownerConflicts(left: DaemonSupervisorOwnerScope, right: DaemonSupervisorOwnerScope)` — [`L578`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L578)
- `ownerDirectoryPath(registryDir: string, generation: string)` — [`L602`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L602)
- `ownerRecordFingerprint(record: DaemonSupervisorOwnerRecord)` — [`L592`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L592)
- `persistDaemonStartupFenceFromOwner(socketPath: string, hello: DaemonSupervisorHelloIdentity, registryDir?: string)` — [`L425`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L425)
- `readActiveShutdownAdmission(registryDir: string)` — [`L743`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L743)
- `readOwnerRecord(directory: string)` — [`L639`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L639)
- `readOwnerRecordForScope(directory: string, isRelevant: (scope: DaemonSupervisorOwnerScope) => boolean)` — [`L617`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L617)
- `readOwnerScope(directory: string)` — [`L671`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L671)
- `readShutdownAdmission(path: string)` — [`L756`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L756)
- `readStartupFence(path: string)` — [`L714`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L714)
- `requireOwnerRecord(directory: string)` — [`L609`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L609)
- `sameOwnerRecord(left: DaemonSupervisorOwnerRecord, right: DaemonSupervisorOwnerRecord)` — [`L582`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L582)
- `shutdownAdmissionPath(registryDir: string)` — [`L801`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L801)
- `startupFencePath(directory: string, socketPath: string)` — [`L796`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L796)
- `waitForDaemonStartupFence(socketPath: string, timeoutMs?: number, registryDir?: string)` — [`L482`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L482)
- `withDaemonSupervisorRegistryGuard(registryDir: string, action: () => T | Promise<T>)` — [`L253`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L253)
- `writeJsonAtomically(path: string, value: unknown)` — [`L785`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L785)
- `writeOwnerRecord(directory: string, record: DaemonSupervisorOwnerRecord)` — [`L710`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L710)
- `writeOwnerScope(directory: string, owner: DaemonSupervisorOwnerRecord)` — [`L698`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L698)

## Module values
- `DAEMON_SUPERVISOR_REGISTRY_DIR_ENV` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L17)
- `OWNER_VERSION` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L19)
- `REGISTRY_LOCK_RETRIES` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L22)
- `REGISTRY_LOCK_RETRY_MS` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L23)
- `REGISTRY_LOCK_STALE_MS` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L20)
- `REGISTRY_LOCK_UPDATE_MS` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L21)
- `SHUTDOWN_ADMISSION_FILE_NAME` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L25)
- `SHUTDOWN_ADMISSION_LEASE_MS` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L26)
- `SHUTDOWN_ADMISSION_REFRESH_MS` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L27)
- `SHUTDOWN_ADMISSION_WAIT_MS` — [`L28`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L28)
- `STARTUP_FENCE_POLL_MS` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L24)
- `generation` — [`L367`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L367)
- `pid` — [`L368`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L368)
- `processStartId` — [`L369`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L369)
- `socketPath` — [`L370`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-supervisor-ownership.ts#L370)

