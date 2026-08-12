---
title: 'Module: packages/coding-agent/src/core/kernel/bootstrap.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/kernel/bootstrap.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/kernel/`bootstrap.ts`/
symbols:
  ensureKernelPythonUncached: ensureKernelPythonUncached().
  syncPythonSkills: syncPythonSkills().
  ensureKernelPython: ensureKernelPython().
  writeBootstrapVersion: writeBootstrapVersion().
  BootstrapPythonSkill: BootstrapPythonSkill#
  normalizePythonSkills: normalizePythonSkills().
  bootstrapVenv: bootstrapVenv().
  bootstrapBaseVersionCurrent: bootstrapBaseVersionCurrent().
  ensureUv: ensureUv().
  resolveSiblingPythonSkillDependency: resolveSiblingPythonSkillDependency().
  acquireBootstrapLock: acquireBootstrapLock().
  readPythonSkillDependencyNames: readPythonSkillDependencyNames().
  BootstrapPythonSkill.packagePath: BootstrapPythonSkill#packagePath.
  kernelReady: kernelReady().
  sortPythonSkillsForInstall: sortPythonSkillsForInstall().
  pythonSkillsMatch: pythonSkillsMatch().
  bootstrapVersionCurrent: bootstrapVersionCurrent().
  BootstrapPythonSkill.importName: BootstrapPythonSkill#importName.
  readPythonSkillProjectName: readPythonSkillProjectName().
  readBootstrapVersion: readBootstrapVersion().
  KernelPythonSkill: KernelPythonSkill#
  BootstrapPythonSkill.pyprojectPath: BootstrapPythonSkill#pyprojectPath.
  DEFAULT_RLM_EXTRA_UV_ARGS: DEFAULT_RLM_EXTRA_UV_ARGS.
  DEFAULT_RLM_EXTRA_IMPORT_NAMES: DEFAULT_RLM_EXTRA_IMPORT_NAMES.
  resolveRuntimeIdentity: resolveRuntimeIdentity().
  missingPythonSkillImportLabels: missingPythonSkillImportLabels().
  reportProgress: reportProgress().
  kernelBaseReady: kernelBaseReady().
  KernelBootstrapProgressHandler: KernelBootstrapProgressHandler#
  BootstrapPythonSkill.pyprojectHash: BootstrapPythonSkill#pyprojectHash.
  run: run().
  EnsureKernelPythonOptions: EnsureKernelPythonOptions#
  resolveWritableKernelVenvDir: resolveWritableKernelVenvDir().
  hasPrimeAgentRuntime: hasPrimeAgentRuntime().
  formatPythonSkillInstallArgs: formatPythonSkillInstallArgs().
  resolveRuntimeSourceDir: resolveRuntimeSourceDir().
  DEFAULT_RLM_EXTRA_IMPORT_LABELS: DEFAULT_RLM_EXTRA_IMPORT_LABELS.
  missingRlmExtraImportLabels: missingRlmExtraImportLabels().
  BootstrapVersion.pythonSkills: BootstrapVersion#pythonSkills.
  getKernelVenvDir: getKernelVenvDir().
  pythonImports: pythonImports().
  hasIpykernel: hasIpykernel().
  inFlightEnsureKernelPython: inFlightEnsureKernelPython.
  errorMessage: errorMessage().
  EnsureKernelPythonOptions.pythonSkills: EnsureKernelPythonOptions#pythonSkills.
  findExecutable: findExecutable().
  DEFAULT_RLM_EXTRA_PACKAGES: DEFAULT_RLM_EXTRA_PACKAGES.
  EnsureKernelPythonOptions.onProgress: EnsureKernelPythonOptions#onProgress.
  BootstrapVersion: BootstrapVersion#
  RUNTIME_READY_CHECK: RUNTIME_READY_CHECK.
  ensureKernelPythonKey: ensureKernelPythonKey().
  getXdgKernelVenvDir: getXdgKernelVenvDir().
  bootstrapLockDir: bootstrapLockDir().
  processIsRunning: processIsRunning().
  lockMissingPidIsStale: lockMissingPidIsStale().
  runtimeCandidateDirs: runtimeCandidateDirs().
  formatBootstrapFailure: formatBootstrapFailure().
  IPYKERNEL_REQUIREMENT: IPYKERNEL_REQUIREMENT.
  STATE_SNAPSHOT_REQUIREMENT: STATE_SNAPSHOT_REQUIREMENT.
  UV_INSTALL_COMMAND: UV_INSTALL_COMMAND.
  isExecutable: isExecutable().
  expandHome: expandHome().
  BOOTSTRAP_SCHEMA: BOOTSTRAP_SCHEMA.
  PYTHON_VERSION: PYTHON_VERSION.
  RUNTIME_REQUIREMENT: RUNTIME_REQUIREMENT.
  BOOTSTRAP_VERSION_FILE: BOOTSTRAP_VERSION_FILE.
  BootstrapVersion.schema: BootstrapVersion#schema.
  BootstrapVersion.ipykernel: BootstrapVersion#ipykernel.
  BootstrapVersion.runtime: BootstrapVersion#runtime.
  BootstrapVersion.snapshot: BootstrapVersion#snapshot.
  BootstrapVersion.extraUvArgs: BootstrapVersion#extraUvArgs.
  isNodeError: isNodeError().
  isRecord: isRecord().
  fileContentHash: fileContentHash().
  readTomlProjectSection: readTomlProjectSection().
  REQUIRED_HARNESS_METHODS: REQUIRED_HARNESS_METHODS.
  BOOTSTRAP_LOCK_NAME: BOOTSTRAP_LOCK_NAME.
  BOOTSTRAP_LOCK_RETRY_MS: BOOTSTRAP_LOCK_RETRY_MS.
  BOOTSTRAP_LOCK_STALE_WITHOUT_PID_MS: BOOTSTRAP_LOCK_STALE_WITHOUT_PID_MS.
  exists: exists().
  parseDependencyPackageName: parseDependencyPackageName().
  findTomlArrayEnd: findTomlArrayEnd().
  run.options-typeLiteral217.stdio: run().(options)typeLiteral217:stdio.
  readLockPid: readLockPid().
  confirmUvInstall: confirmUvInstall().
  extraUvArgsMatch: extraUvArgsMatch().
  hashRuntimeSource: hashRuntimeSource().
---
# Module: [`packages/coding-agent/src/core/kernel/bootstrap.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts)

## Classes
### `BootstrapPythonSkill`
- def: [`packages/coding-agent/src/core/kernel/bootstrap.ts:70`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L70)
- signature: `interface BootstrapPythonSkill`
- members:
  - `importName` — [`L71`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L71)
  - `packagePath` — [`L72`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L72)
  - `pyprojectHash` — [`L74`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L74)
  - `pyprojectPath` — [`L73`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L73)
- used by: [`ensureKernelPythonUncached`](bootstrap.ts.md#ensureKernelPythonUncached), [`syncPythonSkills`](bootstrap.ts.md#syncPythonSkills), [`writeBootstrapVersion`](bootstrap.ts.md#writeBootstrapVersion), [`bootstrapVenv`](bootstrap.ts.md#bootstrapVenv), [`normalizePythonSkills`](bootstrap.ts.md#normalizePythonSkills), [`resolveSiblingPythonSkillDependency`](bootstrap.ts.md#resolveSiblingPythonSkillDependency), [`readPythonSkillDependencyNames`](bootstrap.ts.md#readPythonSkillDependencyNames), [`kernelReady`](bootstrap.ts.md#kernelReady), [`bootstrapVersionCurrent`](bootstrap.ts.md#bootstrapVersionCurrent), [`pythonSkillsMatch`](bootstrap.ts.md#pythonSkillsMatch), [`sortPythonSkillsForInstall`](bootstrap.ts.md#sortPythonSkillsForInstall), [`readBootstrapVersion`](bootstrap.ts.md#readBootstrapVersion), [`readPythonSkillProjectName`](bootstrap.ts.md#readPythonSkillProjectName), [`formatPythonSkillInstallArgs`](bootstrap.ts.md#formatPythonSkillInstallArgs), [`pythonSkills`](bootstrap.ts.md#BootstrapVersion.pythonSkills), [`ensureKernelPythonKey`](bootstrap.ts.md#ensureKernelPythonKey)

### `BootstrapVersion`
- def: [`packages/coding-agent/src/core/kernel/bootstrap.ts:77`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L77)
- signature: `interface BootstrapVersion`
- members:
  - `extraUvArgs` — [`L82`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L82)
  - `ipykernel` — [`L79`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L79)
  - `pythonSkills` — [`L83`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L83)
  - `runtime` — [`L80`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L80)
  - `schema` — [`L78`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L78)
  - `snapshot` — [`L81`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L81)
- uses (calls/refs, reference-scoped): [`BootstrapPythonSkill`](bootstrap.ts.md#BootstrapPythonSkill)
- used by: [`syncPythonSkills`](bootstrap.ts.md#syncPythonSkills), [`writeBootstrapVersion`](bootstrap.ts.md#writeBootstrapVersion), [`bootstrapBaseVersionCurrent`](bootstrap.ts.md#bootstrapBaseVersionCurrent), [`bootstrapVersionCurrent`](bootstrap.ts.md#bootstrapVersionCurrent), [`readBootstrapVersion`](bootstrap.ts.md#readBootstrapVersion)

### `EnsureKernelPythonOptions`
- def: [`packages/coding-agent/src/core/kernel/bootstrap.ts:65`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L65)
- signature: `interface EnsureKernelPythonOptions`
- members:
  - `onProgress` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L67)
  - `pythonSkills` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L66)
- uses (calls/refs, reference-scoped): [`KernelPythonSkill`](bootstrap.ts.md#KernelPythonSkill), [`KernelBootstrapProgressHandler`](bootstrap.ts.md#KernelBootstrapProgressHandler)
- used by: [`ensureKernelPythonUncached`](bootstrap.ts.md#ensureKernelPythonUncached), [`syncPythonSkills`](bootstrap.ts.md#syncPythonSkills), [`ensureKernelPython`](bootstrap.ts.md#ensureKernelPython), [`bootstrapVenv`](bootstrap.ts.md#bootstrapVenv), [`ensureUv`](bootstrap.ts.md#ensureUv), [`reportProgress`](bootstrap.ts.md#reportProgress)

### `KernelBootstrapProgressHandler`
- def: [`packages/coding-agent/src/core/kernel/bootstrap.ts:63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L63)
- signature: `type KernelBootstrapProgressHandler`
- used by: [`createIpythonToolDefinition`](../tools/ipython.ts.md#createIpythonToolDefinition), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-index.ts), [`ensure`](../tools/ipython.ts.md#IpythonKernelProvisioner.ensure), [`executeWithBusyKernelChoice`](../tools/ipython.ts.md#executeWithBusyKernelChoice), [`EnsureKernelPythonOptions`](bootstrap.ts.md#EnsureKernelPythonOptions), [`startupListeners`](../tools/ipython.ts.md#IpythonKernelProvisioner.startupListeners), [`onBootstrapProgress`](index.ts.md#KernelStartOptions.onBootstrapProgress)  (1 test-only)

### `KernelPythonSkill`
- def: [`packages/coding-agent/src/core/kernel/bootstrap.ts:62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L62)
- signature: `type KernelPythonSkill`
- uses (calls/refs, reference-scoped): [`PythonSkillRuntimeInfo`](../skills.ts.md#PythonSkillRuntimeInfo)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-index.ts), [`normalizePythonSkills`](bootstrap.ts.md#normalizePythonSkills), [`missingPythonSkillImportLabels`](bootstrap.ts.md#missingPythonSkillImportLabels), [`pythonSkills`](index.ts.md#KernelManagerOptions.pythonSkills), [`pythonSkills`](bootstrap.ts.md#EnsureKernelPythonOptions.pythonSkills)  (4 test-only)

## Functions
- `acquireBootstrapLock(venv: string)` — [`L477`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L477)
- `bootstrapBaseVersionCurrent(version: BootstrapVersion | null, runtimeIdentity: string)` — [`L633`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L633)
- `bootstrapLockDir(venv: string)` — [`L445`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L445)
- `bootstrapVenv(venv: string, pythonSkills: readonly BootstrapPythonSkill[], options: EnsureKernelPythonOptions)` — [`L721`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L721)
- `bootstrapVersionCurrent(version: BootstrapVersion | null, runtimeIdentity: string, pythonSkills: readonly BootstrapPythonSkill[])` — [`L621`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L621)
- `confirmUvInstall()` — [`L545`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L545)
- `ensureKernelPython(options?: EnsureKernelPythonOptions)` — [`L919`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L919) — documented in [packages-coding-agent-src-core-kernel-index.ts](../../../../../../concepts/packages-coding-agent-src-core-kernel-index.ts.md)
- `ensureKernelPythonKey(pythonSkills: readonly BootstrapPythonSkill[])` — [`L329`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L329)
- `ensureKernelPythonUncached(options: EnsureKernelPythonOptions, pythonSkills: readonly BootstrapPythonSkill[])` — [`L855`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L855)
- `ensureUv(options: EnsureKernelPythonOptions)` — [`L514`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L514)
- `errorMessage(error: unknown)` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L86)
- `exists(filePath: string)` — [`L98`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L98)
- `expandHome(filePath: string)` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L116)
- `extraUvArgsMatch(a: string[] | undefined, b: string[] | undefined)` — [`L600`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L600)
- `fileContentHash(filePath: string)` — [`L122`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L122)
- `findExecutable(name: string)` — [`L500`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L500)
- `findTomlArrayEnd(text: string, startIndex: number)` — [`L194`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L194)
- `formatBootstrapFailure(error: unknown)` — [`L847`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L847)
- `formatPythonSkillInstallArgs(skill: BootstrapPythonSkill)` — [`L325`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L325)
- `getKernelVenvDir()` — [`L339`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L339)
- `getXdgKernelVenvDir()` — [`L345`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L345)
- `hasIpykernel(python: string)` — [`L401`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L401)
- `hasPrimeAgentRuntime(python: string)` — [`L405`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L405)
- `hashRuntimeSource(sourceDir: string)` — [`L695`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L695)
- `isExecutable(filePath: string)` — [`L107`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L107)
- `isNodeError(error: unknown, code: string)` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L90)
- `isRecord(value: unknown)` — [`L94`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L94)
- `kernelBaseReady(python: string, venv: string, runtimeIdentity: string)` — [`L826`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L826)
- `kernelReady(python: string, venv: string, runtimeIdentity: string, pythonSkills: readonly BootstrapPythonSkill[])` — [`L834`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L834)
- `lockMissingPidIsStale(lockDir: string)` — [`L468`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L468)
- `missingPythonSkillImportLabels(python: string, pythonSkills: readonly PythonSkillRuntimeInfo[])` — [`L424`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L424)
- `missingRlmExtraImportLabels(python: string)` — [`L414`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L414)
- `normalizePythonSkills(pythonSkills: readonly PythonSkillRuntimeInfo[] | undefined)` — [`L130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L130)
- `parseDependencyPackageName(dependency: string)` — [`L185`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L185)
- `processIsRunning(pid: number)` — [`L449`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L449)
- `pythonImports(python: string, moduleName: string)` — [`L392`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L392)
- `pythonSkillsMatch(a: BootstrapPythonSkill[] | undefined, b: readonly BootstrapPythonSkill[])` — [`L607`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L607)
- `readBootstrapVersion(venv: string)` — [`L560`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L560)
- `readLockPid(lockDir: string)` — [`L458`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L458)
- `readPythonSkillDependencyNames(skill: BootstrapPythonSkill)` — [`L224`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L224)
- `readPythonSkillProjectName(skill: BootstrapPythonSkill)` — [`L179`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L179)
- `readTomlProjectSection(pyprojectPath: string)` — [`L163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L163)
- `reportProgress(options: EnsureKernelPythonOptions, message: string)` — [`L437`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L437)
- `resolveRuntimeIdentity()` — [`L686`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L686)
- `resolveRuntimeSourceDir()` — [`L673`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L673)
- `resolveSiblingPythonSkillDependency(skill: BootstrapPythonSkill, dependencyName: string)` — [`L254`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L254)
- `resolveWritableKernelVenvDir()` — [`L352`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L352)
- `run(command: string, args: string[], options?: { stdio?: "ignore" | "inherit" | undefined; })` — [`L374`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L374)
- `runtimeCandidateDirs()` — [`L659`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L659)
- `sortPythonSkillsForInstall(pythonSkills: readonly BootstrapPythonSkill[])` — [`L281`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L281)
- `syncPythonSkills(uv: string, venv: string, python: string, runtimeIdentity: string, pythonSkills: readonly BootstrapPythonSkill[], options: EnsureKernelPythonOptions)` — [`L748`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L748)
- `writeBootstrapVersion(venv: string, runtimeIdentity: string, pythonSkills: readonly BootstrapPythonSkill[])` — [`L643`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L643)

## Module values
- `BOOTSTRAP_LOCK_NAME` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L56)
- `BOOTSTRAP_LOCK_RETRY_MS` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L57)
- `BOOTSTRAP_LOCK_STALE_WITHOUT_PID_MS` — [`L58`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L58)
- `BOOTSTRAP_SCHEMA` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L14)
- `BOOTSTRAP_VERSION_FILE` — [`L55`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L55)
- `DEFAULT_RLM_EXTRA_IMPORT_LABELS` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L37)
- `DEFAULT_RLM_EXTRA_IMPORT_NAMES` — [`L36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L36)
- `DEFAULT_RLM_EXTRA_PACKAGES` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L21)
- `DEFAULT_RLM_EXTRA_UV_ARGS` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L35)
- `IPYKERNEL_REQUIREMENT` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L16)
- `PYTHON_VERSION` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L15)
- `REQUIRED_HARNESS_METHODS` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L39)
- `RUNTIME_READY_CHECK` — [`L54`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L54)
- `RUNTIME_REQUIREMENT` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L17)
- `STATE_SNAPSHOT_REQUIREMENT` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L20)
- `UV_INSTALL_COMMAND` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L38)
- `inFlightEnsureKernelPython` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L60)
- `stdio` — [`L374`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/bootstrap.ts#L374)

