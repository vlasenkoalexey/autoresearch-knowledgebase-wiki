# Wiki index

**Read this first.** A content catalog of everything in this wiki — both **code repos** (ingested by the
`wikify-ingest-repo` skill) and **prose** (articles/docs/notes, the classic Karpathy way). Find the
relevant entry here, then drill into its page. See [`log.md`](log.md) for the chronological history.

## Code repos
One `wiki/code/<slug>/` per ingested repo. Open its `overview.md` as a map, then `grep` to the
concept/catalog page and cite the catalog anchor; drop to the pinned source for line-level certainty.

_None yet._ — run **`ingest <repo-url-or-path>`** to add one (the skill adds a row here and an entry
to [`log.md`](log.md)).

## Cross-repo concepts
Host vocabulary (`wiki/concepts/<key>.md`), wired by the `wikify-connect-repo` skill: each concept page
links **down** to every repo's implementation, and each implementation links back up.

_None yet._ — appears once two or more code repos are ingested and connected.

## Topics
Synthesized prose pages (`wiki/topics/<topic>.md`) — entities, concepts, comparisons that span sources.

_None yet._

## Sources
One summary page (`wiki/sources/<source>.md`) per ingested article/doc/note; the raw source lives in
`raw/sources/`.

_None yet._

## Notes
Cross-cutting answers filed back from queries (`wiki/notes/<note>.md`) — may mix code and prose.

_None yet._
