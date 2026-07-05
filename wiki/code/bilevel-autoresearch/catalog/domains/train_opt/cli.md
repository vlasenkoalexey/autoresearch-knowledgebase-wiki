---
title: 'Module: domains/train_opt/cli.py'
type: catalog
provenance: extracted
module: domains/train_opt/cli.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.cli`/
symbols:
  cmd_inner: cmd_inner().
  cmd_bilevel: cmd_bilevel().
  _v: _v.
  _line: _line.
  get_llm_client: get_llm_client().
  _env_path: _env_path.
  PROJECT_ROOT: PROJECT_ROOT.
  main: main().
  AUTORESEARCH_DIR: AUTORESEARCH_DIR.
  logger: logger.
  _k: _k.
---
# Module: [`domains/train_opt/cli.py`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py)

## Functions
- `cmd_bilevel(args)` — [`L109`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L109) — Full bilevel experiment (Level 1 + Level 1.5). — documented in [domains-train_opt-config](../../../concepts/domains-train_opt-config.md)
- `cmd_inner(args)` — [`L65`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L65) — Inner loop only — equivalent to Karpathy's autoresearch (Level 1). — documented in [domains-train_opt-config](../../../concepts/domains-train_opt-config.md)
- `get_llm_client(provider: str = "deepseek", model: str = "")` — [`L53`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L53) — Create LLM client from environment.
- `main()` — [`L161`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L161)

## Module values
- `AUTORESEARCH_DIR` — [`L47`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L47)
- `PROJECT_ROOT` — [`L20`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L20)
- `_env_path` — [`L24`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L24)
- `_k` — [`L29`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L29)
- `_line` — [`L26`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L26)
- `_v` — [`L29`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L29)
- `logger` — [`L44`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/cli.py#L44)

