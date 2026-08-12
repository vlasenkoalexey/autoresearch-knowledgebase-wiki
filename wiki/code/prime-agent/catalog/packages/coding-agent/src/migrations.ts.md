---
title: 'Module: packages/coding-agent/src/migrations.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/migrations.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/`migrations.ts`/
symbols:
  runMigrations: runMigrations().
  migrateLegacySessionDirsToSessionRoot: migrateLegacySessionDirsToSessionRoot().
  migrateKeybindingsConfigFile: migrateKeybindingsConfigFile().
  migrateExtensionSystem: migrateExtensionSystem().
  migrateSessionsFromAgentRoot: migrateSessionsFromAgentRoot().
  showDeprecationWarnings: showDeprecationWarnings().
  migrateToolsToBin: migrateToolsToBin().
  migrateAuthToAuthJson: migrateAuthToAuthJson().
  isSessionJsonlFile: isSessionJsonlFile().
  migrateCommandsToPrompts: migrateCommandsToPrompts().
  checkDeprecatedExtensionDirs: checkDeprecatedExtensionDirs().
  runMigrations.typeLiteral209.migratedAuthProviders: runMigrations().typeLiteral209:migratedAuthProviders.
  runMigrations.typeLiteral209.deprecationWarnings: runMigrations().typeLiteral209:deprecationWarnings.
  MIGRATION_GUIDE_URL: MIGRATION_GUIDE_URL.
  EXTENSIONS_DOC_URL: EXTENSIONS_DOC_URL.
  isLegacySessionDirName: isLegacySessionDirName().
  filesHaveSameContent: filesHaveSameContent().
  uniqueSessionRootPath: uniqueSessionRootPath().
---
# Module: [`packages/coding-agent/src/migrations.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts)

## Functions
- `checkDeprecatedExtensionDirs(baseDir: string, label: string)` — [`L329`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L329) — Check for deprecated hooks/ and tools/ directories.
- `filesHaveSameContent(a: string, b: string)` — [`L219`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L219)
- `isLegacySessionDirName(name: string)` — [`L152`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L152)
- `isSessionJsonlFile(filePath: string)` — [`L139`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L139)
- `migrateAuthToAuthJson()` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L33) — Migrate legacy oauth.json and settings.json apiKeys to auth.json.
- `migrateCommandsToPrompts(baseDir: string, label: string)` — [`L244`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L244) — Migrate commands/ to prompts/ if needed.
- `migrateExtensionSystem(cwd: string)` — [`L364`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L364) — Run extension system migrations (commands→prompts) and collect warnings about deprecated directories.
- `migrateKeybindingsConfigFile()` — [`L264`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L264)
- `migrateLegacySessionDirsToSessionRoot()` — [`L163`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L163) — Migrate legacy per-cwd session directories into the flat session root.
- `migrateSessionsFromAgentRoot()` — [`L96`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L96) — Migrate sessions from ~/.pi/agent/*.jsonl to the session root.
- `migrateToolsToBin()` — [`L284`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L284) — Move fd/rg binaries from tools/ to bin/ if they exist.
- `runMigrations(cwd: string)` — [`L412`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L412) — Run all migrations. Called once on startup.
- `showDeprecationWarnings(warnings: string[])` — [`L384`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L384) — Print deprecation warnings and wait for keypress.
- `uniqueSessionRootPath(sessionsDir: string, file: string)` — [`L230`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L230)

## Module values
- `EXTENSIONS_DOC_URL` — [`L25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L25)
- `MIGRATION_GUIDE_URL` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L23)
- `deprecationWarnings` — [`L414`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L414)
- `migratedAuthProviders` — [`L413`](../../../../../../../raw/code/prime-agent/packages/coding-agent/src/migrations.ts#L413)

