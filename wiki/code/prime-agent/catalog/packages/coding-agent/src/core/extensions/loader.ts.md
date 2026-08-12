---
title: 'Module: packages/coding-agent/src/core/extensions/loader.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/extensions/loader.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/extensions/`loader.ts`/
symbols:
  createExtensionAPI: createExtensionAPI().
  createExtensionRuntime: createExtensionRuntime().
  discoverAndLoadExtensions: discoverAndLoadExtensions().
  createExtension: createExtension().
  loadExtensions: loadExtensions().
  loadExtensionFromFactory: loadExtensionFromFactory().
  loadExtensionModule: loadExtensionModule().
  loadExtension.Promise.typeLiteral169.error: loadExtension().Promise:typeLiteral169:error.
  discoverExtensionsInDir: discoverExtensionsInDir().
  resolveExtensionEntries: resolveExtensionEntries().
  getAliases: getAliases().
  loadExtension: loadExtension().
  resolvePath: resolvePath().
  _aliases: _aliases.
  normalizeUnicodeSpaces: normalizeUnicodeSpaces().
  expandPath: expandPath().
  isBundledCli: isBundledCli.
  loadExtension.Promise.typeLiteral169.extension: loadExtension().Promise:typeLiteral169:extension.
  readPiManifest: readPiManifest().
  require: require.
  __PI_BUNDLED__: __PI_BUNDLED__.
  PiManifest: PiManifest#
  PiManifest.extensions: PiManifest#extensions.
  UNICODE_SPACES: UNICODE_SPACES.
  HandlerFn: HandlerFn#
  isExtensionFile: isExtensionFile().
  PiManifest.themes: PiManifest#themes.
  PiManifest.skills: PiManifest#skills.
  PiManifest.prompts: PiManifest#prompts.
---
# Module: [`packages/coding-agent/src/core/extensions/loader.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts)

## Classes
### `HandlerFn`
- def: [`packages/coding-agent/src/core/extensions/loader.ts:109`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L109)
- signature: `type HandlerFn`
- used by: [`createExtensionAPI`](loader.ts.md#createExtensionAPI)

### `PiManifest`
- def: [`packages/coding-agent/src/core/extensions/loader.ts:447`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L447)
- signature: `interface PiManifest`
- members:
  - `extensions` — [`L448`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L448)
  - `prompts` — [`L451`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L451)
  - `skills` — [`L450`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L450)
  - `themes` — [`L449`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L449)
- used by: [`resolveExtensionEntries`](loader.ts.md#resolveExtensionEntries), [`readPiManifest`](loader.ts.md#readPiManifest)

## Functions
- `createExtension(extensionPath: string, resolvedPath: string)` — [`L357`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L357) — Create an Extension object with empty collections.
- `createExtensionAPI(extension: Extension, runtime: ExtensionRuntime, cwd: string, eventBus: EventBus)` — [`L168`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L168) — Create the ExtensionAPI for an extension.
- `createExtensionRuntime()` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L115) — Create a runtime with throwing stubs for action methods.
- `discoverAndLoadExtensions(configuredPaths: string[], cwd: string, agentDir?: string, eventBus?: EventBus | undefined)` — [`L559`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L559) — Discover and load extensions from standard locations.
- `discoverExtensionsInDir(dir: string)` — [`L522`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L522) — Discover extensions in a directory.
- `expandPath(p: string)` — [`L90`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L90)
- `getAliases()` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L37)
- `isExtensionFile(name: string)` — [`L467`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L467)
- `loadExtension(extensionPath: string, cwd: string, eventBus: EventBus, runtime: ExtensionRuntime)` — [`L377`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L377)
- `loadExtensionFromFactory(factory: ExtensionFactory, cwd: string, eventBus: EventBus, runtime: ExtensionRuntime, extensionPath?: string)` — [`L405`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L405) — Create an Extension from an inline factory function.
- `loadExtensionModule(extensionPath: string)` — [`L331`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L331)
- `loadExtensions(paths: string[], cwd: string, eventBus?: EventBus | undefined)` — [`L421`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L421) — Load extensions from paths.
- `normalizeUnicodeSpaces(str: string)` — [`L86`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L86)
- `readPiManifest(packageJsonPath: string)` — [`L454`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L454)
- `resolveExtensionEntries(dir: string)` — [`L480`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L480) — Resolve extension entry points from a directory.
- `resolvePath(extPath: string, cwd: string)` — [`L101`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L101)

## Module values
- `UNICODE_SPACES` — [`L84`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L84)
- `__PI_BUNDLED__` — [`L328`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L328)
- `_aliases` — [`L35`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L35) — Get aliases for jiti (used in Node.js/development mode).
- `error` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L382)
- `extension` — [`L382`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L382)
- `isBundledCli` — [`L329`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L329)
- `require` — [`L29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/loader.ts#L29)

