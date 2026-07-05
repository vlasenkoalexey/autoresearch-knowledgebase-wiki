---
title: Configuration env vars
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Configuration env vars

## Definition
The README's "Configuration" table lists five environment variables that customize the extension without
touching a session's `config.json`: `PI_AUTORESEARCH_VKF` (path to the `vkf` executable, overriding
auto-detection), `PI_AUTORESEARCH_VKF_CONDA_ENV` (which conda env to find `vkf` in, default `VKF`),
`PI_AUTORESEARCH_GLOBAL_ROOT` (root for the cross-project global memory, default `~`),
`PI_AUTORESEARCH_SHORTCUT` (key for the fullscreen dashboard, default `alt+g`, or `none` to disable), and
`PI_AUTORESEARCH_OPEN_SHORTCUT` (key to open the progress page in the browser, default `alt+o`, or `none`).

## In pi-autoresearch-vkf (grounded)
The first two are read by [`resolveVkf`](../catalog/extensions/pi-autoresearch-vkf/vkf.ts.md#resolveVkf) in
[the `vkf` CLI bridge](../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md): `$PI_AUTORESEARCH_VKF` wins
outright as an explicit path, and [`condaEnv`](../catalog/extensions/pi-autoresearch-vkf/vkf.ts.md#condaEnv)
resolves `$PI_AUTORESEARCH_VKF_CONDA_ENV` (default `"VKF"`) as the named environment probed for a `vkf`
binary before falling back to `conda run`. `$PI_AUTORESEARCH_GLOBAL_ROOT` is read by
[`globalRoot`](../catalog/extensions/pi-autoresearch-vkf/paths.ts.md#globalRoot) in
[the workspace-layout module](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md) — it is the one override
point for where the cross-project memory bundle lives, resolved through the exact same
[`memoryPaths`](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md) contract used for a project-local
bundle. The two shortcut variables are read by [`resolve`](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md#resolve)
and [`loadShortcuts`](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md#loadShortcuts) in
`shortcuts.ts`, which fall back to [`DEFAULT_FULLSCREEN`](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md#DEFAULT_FULLSCREEN)
(`alt+g`) / [`DEFAULT_OPEN_BROWSER`](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md#DEFAULT_OPEN_BROWSER)
(`alt+o`) and produce a [`ShortcutConfig`](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md#ShortcutConfig)
consumed by [`autoresearchExtension`](../concepts/extensions-pi-autoresearch-vkf-index.ts.md) to bind the
fullscreen overlay and browser-open commands (`undefined`/`"none"` disables either independently).

## Why it matters / when it applies
All five variables exist to make an otherwise-hardcoded assumption overridable: which conda env has `vkf`
installed, where the global memory bundle should live (useful for a shared machine or CI), and which key
bindings are free in a given terminal setup. None of them are required — every one degrades to a documented
default (or, for `vkf`, to "memory works, validation skipped" per
[the CLI bridge's graceful-degradation design](../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)) rather
than failing the extension.

## Connections
- Code concepts: [The vkf CLI bridge](../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md),
  [Workspace layout](../concepts/extensions-pi-autoresearch-vkf-paths.ts.md),
  [The tool spine](../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- Module catalogs: [shortcuts.ts](../catalog/extensions/pi-autoresearch-vkf/shortcuts.ts.md),
  [vkf.ts](../catalog/extensions/pi-autoresearch-vkf/vkf.ts.md), [paths.ts](../catalog/extensions/pi-autoresearch-vkf/paths.ts.md)
- Related doc-concepts: [Browser dashboard export](browser-dashboard-export.md)

## Source
Extracted from `README.md` ("Configuration" section), kept in place.
