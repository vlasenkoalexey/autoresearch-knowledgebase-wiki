# Wiki index

**Read this first.** A content catalog of everything in this wiki — a collection of papers on
**autoresearch and auto-optimization** (summarized the classic Karpathy way) plus any optional **code
repos** (ingested by the `wikify-ingest-repo` skill). Find the relevant entry here, then drill into its
page. See [`log.md`](log.md) for the chronological history.

## Papers / Sources
One summary page (`wiki/sources/<paper>.md`) per ingested paper; the raw source lives in `raw/papers/`.

_None yet._ — drop a paper in `raw/papers/` and say **`ingest raw/papers/<paper>`** to add one.

## Topics
Synthesized prose pages (`wiki/topics/<topic>.md`) — methods, concepts, entities, comparisons that span
papers (e.g. AI-scientist systems, NAS, learned optimizers, kernel auto-tuning).

_None yet._

## Notes
Cross-cutting answers filed back from queries (`wiki/notes/<note>.md`) — may span papers and code.

_None yet._

## Code repos (optional)
One `wiki/code/<slug>/` per ingested implementation. Open its `overview.md` as a map, then `grep` to the
concept/catalog page and cite the catalog anchor; drop to the pinned source for line-level certainty.

- [**autoresearch**](code/autoresearch/overview.md) — Karpathy's minimal harness for autonomous overnight
  LLM research: an AI agent edits one training file, trains for a fixed 5-minute budget, keeps/discards on
  `val_bpb`, and repeats. Pinned @ `228791f`. Answers: what the agent can change and how a run works
  ([train](code/autoresearch/concepts/train.md)), what's frozen and why the metric can't be gamed
  ([prepare](code/autoresearch/concepts/prepare.md)), and the autonomous
  [experiment loop](code/autoresearch/doc-concepts/autonomous-experiment-loop.md) itself.

## Cross-paper concepts (optional)
Host vocabulary (`wiki/concepts/<key>.md`), wired by the `wikify-connect-repo` skill: each concept page
links **down** to every repo's implementation, and each implementation links back up.

_None yet._ — appears once two or more code repos are ingested and connected.
