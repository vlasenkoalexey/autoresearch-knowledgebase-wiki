---
title: 'Module: extensions/pi-autoresearch-vkf/git.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/git.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`git.ts`/
symbols:
  tryGit: tryGit().
  snapshotToBranch.author-typeLiteral8.email: snapshotToBranch().(author)typeLiteral8:email.
  remoteCommitUrl: remoteCommitUrl().
  remoteBranchUrl: remoteBranchUrl().
  branchNameForIdea: branchNameForIdea().
  Snapshot.full: Snapshot#full.
  Snapshot.short: Snapshot#short.
  Snapshot.branch: Snapshot#branch.
  snapshotToBranch: snapshotToBranch().
  httpBaseFromRemote: httpBaseFromRemote().
  git: git().
  Snapshot: Snapshot#
  snapshotToBranch.author-typeLiteral8.name: snapshotToBranch().(author)typeLiteral8:name.
---
# Module: [`extensions/pi-autoresearch-vkf/git.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts)

## Classes
### `Snapshot`
- def: [`extensions/pi-autoresearch-vkf/git.ts:52`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L52)
- signature: `interface Snapshot`
- members:
  - `branch` — [`L58`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L58) — The branch the snapshot was committed onto.
  - `full` — [`L54`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L54) — Full 40-char commit SHA of the snapshot.
  - `short` — [`L56`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L56) — 7-char short SHA, for compact display.
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`email`](git.ts.md#snapshotToBranch.author-typeLiteral8.email)

## Functions
- `branchNameForIdea(idea: string)` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L40) — Branch name for an idea: `autoresearch-vkf-<slug>`. Strips a leading VKF type
- `git(cwd: string, args: string[], env?: any)` — [`L19`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L19)
- `httpBaseFromRemote(remote: string)` — [`L114`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L114) — Parse a git remote URL (scp-like or scheme form) into an https base + host.
- `remoteBranchUrl(cwd: string, branch: string)` — [`L147`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L147) — A web URL for `branch` on the `origin` remote, or `undefined` if none.
- `remoteCommitUrl(cwd: string, fullSha: string)` — [`L138`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L138) — A web URL for `fullSha` built from the repo's `origin` remote (GitHub/GitLab/
- `snapshotToBranch(cwd: string, branch: string, message: string, author?: { name?: string | undefined; email?: string | undefined; } | undefined)` — [`L67`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L67) — Snapshot the current working tree (tracked changes + new files, respecting
- `tryGit(cwd: string, args: string[], env?: any)` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L28)

## Module values
- `email` — [`L71`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L71)
- `name` — [`L71`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/git.ts#L71)

