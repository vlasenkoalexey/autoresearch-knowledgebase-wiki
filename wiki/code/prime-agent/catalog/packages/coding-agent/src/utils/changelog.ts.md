---
title: 'Module: packages/coding-agent/src/utils/changelog.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/changelog.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`changelog.ts`/
symbols:
  getNewEntries: getNewEntries().
  compareVersions: compareVersions().
  ChangelogEntry: ChangelogEntry#
  parseChangelog: parseChangelog().
  ChangelogEntry.major: ChangelogEntry#major.
  ChangelogEntry.minor: ChangelogEntry#minor.
  ChangelogEntry.content: ChangelogEntry#content.
  ChangelogEntry.patch: ChangelogEntry#patch.
---
# Module: [`packages/coding-agent/src/utils/changelog.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts)

## Classes
### `ChangelogEntry`
- def: [`packages/coding-agent/src/utils/changelog.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L3)
- signature: `interface ChangelogEntry`
- members:
  - `content` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L7)
  - `major` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L4)
  - `minor` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L5)
  - `patch` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L6)
- used by: [`handleChangelogCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleChangelogCommand), [`getNewEntries`](changelog.ts.md#getNewEntries), [`compareVersions`](changelog.ts.md#compareVersions), [`parseChangelog`](changelog.ts.md#parseChangelog)

## Functions
- `compareVersions(v1: ChangelogEntry, v2: ChangelogEntry)` — [`L76`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L76) — Compare versions. Returns: -1 if v1 < v2, 0 if v1 === v2, 1 if v1 > v2
- `getNewEntries(entries: ChangelogEntry[], lastVersion: string)` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L85) — Get entries newer than lastVersion
- `parseChangelog(changelogPath: string)` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/changelog.ts#L14) — Parse changelog entries from CHANGELOG.md

