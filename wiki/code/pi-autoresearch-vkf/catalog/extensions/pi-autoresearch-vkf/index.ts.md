---
title: 'Module: extensions/pi-autoresearch-vkf/index.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/index.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`index.ts`/
symbols:
  autoresearchExtension: autoresearchExtension().
  buildDashboardPayload: buildDashboardPayload().
  toCardLike: toCardLike.
  validationNote: validationNote().
  continuationNote: continuationNote().
  promptStub: promptStub().
  staleIdSet: staleIdSet().
  requireSession: requireSession().
  parseDdgResults: parseDdgResults().
  writeProgressDashboard: writeProgressDashboard().
  fetchText: fetchText().
  truncateRun: truncateRun().
  MAX_OUTPUT_CHARS: MAX_OUTPUT_CHARS.
  RUN_OUTPUT_CHARS: RUN_OUTPUT_CHARS.
  truncate: truncate.
  FetchedText: FetchedText#
  FetchedText.status: FetchedText#status.
  FetchedText.contentType: FetchedText#contentType.
  FetchedText.body: FetchedText#body.
  WebSearchHit: WebSearchHit#
  htmlToText: htmlToText().
  WEB_FETCH_DEFAULT_CHARS: WEB_FETCH_DEFAULT_CHARS.
  FetchedText.finalUrl: FetchedText#finalUrl.
  WebSearchHit.title: WebSearchHit#title.
  WebSearchHit.url: WebSearchHit#url.
  WebSearchHit.snippet: WebSearchHit#snippet.
  writeFileIfAbsent: writeFileIfAbsent().
  VERSION: VERSION.
  capStr: capStr.
  OUR_TOOL_NAMES: OUR_TOOL_NAMES.
  WEB_USER_AGENT: WEB_USER_AGENT.
  decodeDdgHref: decodeDdgHref().
  shortCommit: shortCommit().
  browserOpenCommand: browserOpenCommand().
  measureStub: measureStub().
---
# Module: [`extensions/pi-autoresearch-vkf/index.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts)

## Classes
### `FetchedText`
- def: [`extensions/pi-autoresearch-vkf/index.ts:1809`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1809)
- signature: `interface FetchedText`
- members:
  - `body` — [`L1812`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1812)
  - `contentType` — [`L1811`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1811)
  - `finalUrl` — [`L1813`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1813)
  - `status` — [`L1810`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1810)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`fetchText`](index.ts.md#fetchText)

### `WebSearchHit`
- def: [`extensions/pi-autoresearch-vkf/index.ts:1816`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1816)
- signature: `interface WebSearchHit`
- members:
  - `snippet` — [`L1819`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1819)
  - `title` — [`L1817`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1817)
  - `url` — [`L1818`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1818)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`parseDdgResults`](index.ts.md#parseDdgResults)

## Functions
- `autoresearchExtension(pi: ExtensionAPI)` — [`L205`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L205) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- `browserOpenCommand(target: string)` — [`L2004`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L2004) — The platform command that opens a file/URL in the user's default browser.
- `buildDashboardPayload(root: string, refreshSeconds?: number | undefined, includeGraph?: boolean)` — [`L1895`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1895) — Build the dashboard payload from the current session + memory state. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `continuationNote(root: string, config: ResearchConfig, rt: Runtime)` — [`L148`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L148) — The autonomy directive appended to loop-tool outputs. Skill text fades out of — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `decodeDdgHref(href: string)` — [`L1858`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1858) — DuckDuckGo HTML wraps result links as //duckduckgo.com/l/?uddg=<encoded>. Unwrap them.
- `fetchText(url: string, signal: any, timeoutMs: number)` — [`L1823`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1823) — Fetch a URL as text, following redirects, aborting on the tool signal or timeout.
- `htmlToText(html: string)` — [`L1836`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1836) — Reduce an HTML document to readable plain text (best-effort, no DOM).
- `measureStub(command: string)` — [`L2020`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L2020)
- `parseDdgResults(html: string, limit: number)` — [`L1871`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1871) — Parse titles/urls/snippets out of a DuckDuckGo HTML results page.
- `promptStub(config: ResearchConfig)` — [`L2037`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L2037) — The structured handoff document. A fresh agent (after a restart or context — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `requireSession(root: string)` — [`L121`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L121) — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `shortCommit(explicit: string | undefined, cwd: string)` — [`L1990`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1990) — Normalize a commit reference to a 7-char short hash. Uses the explicit value
- `staleIdSet(root: string)` — [`L180`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L180) — Ids of memory cards that should be treated as stale: those whose `valid_until` — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `truncateRun(s: string, cap?: number)` — [`L86`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L86) — Truncate run output keeping head AND tail — errors and METRIC lines print last.
- `validationNote(root: string, profile: number)` — [`L128`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L128) — Summarize a post-write validation, for inclusion in tool output. — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `writeFileIfAbsent(path: string, contents: string)` — [`L2016`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L2016)
- `writeProgressDashboard(root: string, refreshSeconds?: number | undefined, includeGraph?: boolean)` — [`L1976`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1976) — (Re)generate the interactive progress dashboard. Writes the HTML shell — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)

## Module values
- `MAX_OUTPUT_CHARS` — [`L73`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L73)
- `OUR_TOOL_NAMES` — [`L1782`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1782) — Tool names this extension registers, used by the watchdog to detect an engaged loop.
- `RUN_OUTPUT_CHARS` — [`L83`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L83)
- `VERSION` — [`L94`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L94) — Package version, surfaced in the dashboard footer. Keep in sync with package.json.
- `WEB_FETCH_DEFAULT_CHARS` — [`L82`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L82) — Context-hygiene caps. Tool results live in the conversation forever, so the
- `WEB_USER_AGENT` — [`L1807`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L1807)
- `capStr` — [`L114`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L114) — Cap a free-text field (mechanism, context, …) that recurs in tool output every call.
- `toCardLike` — [`L97`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L97) — Adapt a listed card to the shape the synthesis heuristics consume. Pure. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `truncate` — [`L116`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/index.ts#L116)

