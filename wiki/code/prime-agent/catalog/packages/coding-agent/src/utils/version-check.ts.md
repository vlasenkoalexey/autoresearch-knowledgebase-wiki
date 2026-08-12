---
title: 'Module: packages/coding-agent/src/utils/version-check.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/version-check.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`version-check.ts`/
symbols:
  getLatestPiRelease: getLatestPiRelease().
  comparePackageVersions: comparePackageVersions().
  checkForNewPiVersion: checkForNewPiVersion().
  getReleaseManifestPath: getReleaseManifestPath().
  getLatestPiVersion: getLatestPiVersion().
  isNewerPackageVersion: isNewerPackageVersion().
  ParsedVersion.prerelease: ParsedVersion#prerelease.
  parsePackageVersion: parsePackageVersion().
  LatestPiRelease.version: LatestPiRelease#version.
  ParsedVersion.major: ParsedVersion#major.
  ParsedVersion.minor: ParsedVersion#minor.
  ParsedVersion.patch: ParsedVersion#patch.
  getPrimeAgentDownloadBaseUrl: getPrimeAgentDownloadBaseUrl().
  LatestPiRelease.installSpec: LatestPiRelease#installSpec.
  LatestPiRelease: LatestPiRelease#
  LatestPiRelease.packageName: LatestPiRelease#packageName.
  DEFAULT_PRIME_AGENT_DOWNLOAD_BASE_URL: DEFAULT_PRIME_AGENT_DOWNLOAD_BASE_URL.
  STABLE_VERSION_MANIFEST_PATH: STABLE_VERSION_MANIFEST_PATH.
  BETA_VERSION_MANIFEST_PATH: BETA_VERSION_MANIFEST_PATH.
  DEFAULT_VERSION_CHECK_TIMEOUT_MS: DEFAULT_VERSION_CHECK_TIMEOUT_MS.
  ParsedVersion: ParsedVersion#
  comparePrereleaseIdentifiers: comparePrereleaseIdentifiers().
  normalizeReleaseVersion: normalizeReleaseVersion().
  resolveReleaseUrl: resolveReleaseUrl().
  getLatestPiRelease.options-typeLiteral51.timeoutMs: getLatestPiRelease().(options)typeLiteral51:timeoutMs.
  getLatestPiVersion.options-typeLiteral79.timeoutMs: getLatestPiVersion().(options)typeLiteral79:timeoutMs.
---
# Module: [`packages/coding-agent/src/utils/version-check.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts)

## Classes
### `LatestPiRelease`
- def: [`packages/coding-agent/src/utils/version-check.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L8)
- signature: `interface LatestPiRelease`
- members:
  - `installSpec` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L11)
  - `packageName` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L10)
  - `version` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L9)
- used by: [`getLatestPiRelease`](version-check.ts.md#getLatestPiRelease), [`getSelfUpdatePlan`](../package-manager-cli.ts.md#getSelfUpdatePlan), [`getLatestPiVersion`](version-check.ts.md#getLatestPiVersion)

### `ParsedVersion`
- def: [`packages/coding-agent/src/utils/version-check.ts:14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L14)
- signature: `interface ParsedVersion`
- members:
  - `major` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L15)
  - `minor` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L16)
  - `patch` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L17)
  - `prerelease` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L18)
- used by: [`comparePackageVersions`](version-check.ts.md#comparePackageVersions), [`getReleaseManifestPath`](version-check.ts.md#getReleaseManifestPath), [`parsePackageVersion`](version-check.ts.md#parsePackageVersion)

## Functions
- `checkForNewPiVersion(currentVersion: string)` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L163)
- `comparePackageVersions(leftVersion: string, rightVersion: string)` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L64)
- `comparePrereleaseIdentifiers(leftPrerelease: string, rightPrerelease: string)` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L21)
- `getLatestPiRelease(currentVersion: string, options?: { timeoutMs?: number | undefined; })` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L114)
- `getLatestPiVersion(currentVersion: string, options?: { timeoutMs?: number | undefined; })` — [`L156`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L156)
- `getPrimeAgentDownloadBaseUrl()` — [`L88`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L88)
- `getReleaseManifestPath(currentVersion: string)` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L99)
- `isNewerPackageVersion(candidateVersion: string, currentVersion: string)` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L80)
- `normalizeReleaseVersion(version: string)` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L95)
- `parsePackageVersion(version: string)` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L51)
- `resolveReleaseUrl(baseUrl: string, pathOrUrl: string)` — [`L104`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L104)

## Module values
- `BETA_VERSION_MANIFEST_PATH` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L5)
- `DEFAULT_PRIME_AGENT_DOWNLOAD_BASE_URL` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L3)
- `DEFAULT_VERSION_CHECK_TIMEOUT_MS` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L6)
- `STABLE_VERSION_MANIFEST_PATH` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L4)
- `timeoutMs` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L116)
- `timeoutMs` — [`L158`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/version-check.ts#L158)

