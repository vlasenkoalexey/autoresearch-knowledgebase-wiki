---
title: PackageManager — resolving extensions, skills, prompts, and themes
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-package-manager.ts
updated: 2026-08-12
status: fresh
---
# PackageManager — resolving extensions, skills, prompts, and themes

## Overview

`DefaultPackageManager.`[`resolve`](../catalog/packages/coding-agent/src/core/package-manager.ts.md#DefaultPackageManager.resolve)
merges global and project [`SettingsManager`](packages-coding-agent-src-core-settings-manager.ts.md)
package sources (git URLs, npm packages, local paths) into a `ResolvedPaths` — its
[`extensions`](../catalog/packages/coding-agent/src/core/package-manager.ts.md#ResolvedPaths.extensions)
field alongside sibling `prompts`/`skills`/`themes`. `addAutoDiscoveredResources` layers in
convention-discovered resources (e.g. an `.agent/skills/` directory) without an explicit package-source
entry, and `checkForAvailableUpdates` diffs installed git/npm package versions against upstream. This is
the extensibility substrate underneath the coding-agent's skills/extensions system — analogous to, but a
distinct mechanism from, [`continual-harness`](../../continual-harness/overview.md)'s runtime CRUD
self-editing of skills, since package resolution happens at session-start, not mid-episode.

## See also
- [`packages-coding-agent-src-core-settings-manager.ts`](packages-coding-agent-src-core-settings-manager.ts.md) —
  the settings layer this resolver reads sources from.
