---
title: 'Module: domains/article_opt/cli.py'
type: catalog
provenance: extracted
module: domains/article_opt/cli.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.cli`/
symbols:
  cmd_mechresearch: cmd_mechresearch().
  cmd_run: cmd_run().
  cmd_inner: cmd_inner().
  cmd_once: cmd_once().
  v: v.
  make_runner: make_runner().
  main: main().
  load_articles: load_articles().
  logger: logger.
  BASE_DIR: BASE_DIR.
  line: line.
  ARTICLE_FILES: ARTICLE_FILES.
  _env_path: _env_path.
  ARTICLES_DIR: ARTICLES_DIR.
  REFERENCE_DOC: REFERENCE_DOC.
  k: k.
---
# Module: [`domains/article_opt/cli.py`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py)

## Functions
- `cmd_inner(args)` — [`L150`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L150) — Inner loop only — useful for debugging a single article. — documented in [core-inner_loop](../../../concepts/core-inner_loop.md)
- `cmd_mechresearch(args)` — [`L179`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L179) — Level 2 mechanism research — outer LLM generates a new pipeline stage. — documented in [core-inner_loop](../../../concepts/core-inner_loop.md)
- `cmd_once(args)` — [`L282`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L282) — Single pipeline pass — smoke test. — documented in [domains-article_opt-cli](../../../concepts/domains-article_opt-cli.md)
- `cmd_run(args)` — [`L85`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L85) — Full dual-layer experiment. — documented in [core-inner_loop](../../../concepts/core-inner_loop.md)
- `load_articles(ids: list[str])` — [`L56`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L56) — documented in [domains-article_opt-cli](../../../concepts/domains-article_opt-cli.md)
- `main()` — [`L310`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L310) — documented in [domains-article_opt-cli](../../../concepts/domains-article_opt-cli.md)
- `make_runner(provider: str = "minimax", model: str = "")` — [`L70`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L70) — documented in [domains-article_opt-cli](../../../concepts/domains-article_opt-cli.md)

## Module values
- `ARTICLES_DIR` — [`L46`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L46)
- `ARTICLE_FILES` — [`L49`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L49)
- `BASE_DIR` — [`L45`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L45)
- `REFERENCE_DOC` — [`L47`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L47)
- `_env_path` — [`L22`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L22)
- `k` — [`L27`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L27)
- `line` — [`L24`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L24)
- `logger` — [`L43`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L43)
- `v` — [`L27`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/cli.py#L27)

