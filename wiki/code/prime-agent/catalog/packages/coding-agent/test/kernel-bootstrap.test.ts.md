---
title: 'Module: packages/coding-agent/test/kernel-bootstrap.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/kernel-bootstrap.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`kernel-bootstrap.test.ts`/
symbols:
  tempDir: tempDir.
  createPythonSkill: createPythonSkill().
  writeBootstrapVersion: writeBootstrapVersion().
  installFakeUv: installFakeUv().
  writeFakePython: writeFakePython().
  createPythonSkillWithDependency: createPythonSkillWithDependency().
  pyprojectHash: pyprojectHash().
  runtimeIdentity: runtimeIdentity.
  writeExecutable: writeExecutable().
  originalEnv: originalEnv.
---
# Module: [`packages/coding-agent/test/kernel-bootstrap.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts)

## Functions
- `createPythonSkill(name?: string)` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L47)
- `createPythonSkillWithDependency(name: string, dependencyName: string)` — [`L68`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L68)
- `installFakeUv()` — [`L101`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L101)
- `pyprojectHash(pyprojectPath: string)` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L19)
- `writeBootstrapVersion(venv: string, pythonSkills?: readonly PythonSkillRuntimeInfo[])` — [`L28`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L28)
- `writeExecutable(filePath: string, content: string)` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L23)
- `writeFakePython(filePath: string, importableModules: readonly string[])` — [`L81`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L81)

## Module values
- `originalEnv` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L16)
- `runtimeIdentity` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L17)
- `tempDir` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/kernel-bootstrap.test.ts#L15)

