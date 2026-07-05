---
title: 'Module: paper/bilevel-autoresearch/openalex_to_bibtex.py'
type: catalog
provenance: extracted
module: paper/bilevel-autoresearch/openalex_to_bibtex.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `paper.bilevel-autoresearch.openalex_to_bibtex`/
symbols:
  work_to_bibtex: work_to_bibtex().
  main: main().
  normalize_ascii: normalize_ascii().
  make_cite_key: make_cite_key().
  format_authors: format_authors().
  get_journal_or_venue: get_journal_or_venue().
  get_pages: get_pages().
  get_volume_issue: get_volume_issue().
  reconstruct_abstract: reconstruct_abstract().
---
# Module: [`paper/bilevel-autoresearch/openalex_to_bibtex.py`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py)

## Functions
- `format_authors(authorships)` — [`L69`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L69) — Format OpenAlex authorships to BibTeX author string.
- `get_journal_or_venue(work)` — [`L82`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L82) — Extract journal name or conference venue.
- `get_pages(work)` — [`L88`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L88) — Extract page numbers from biblio field.
- `get_volume_issue(work)` — [`L99`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L99) — Extract volume and number from biblio.
- `main()` — [`L174`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L174)
- `make_cite_key(work)` — [`L43`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L43) — Generate a citation key: firstauthorlastname + year + first_content_word.
- `normalize_ascii(text)` — [`L25`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L25) — Normalize unicode to ASCII-safe LaTeX-compatible text.
- `reconstruct_abstract(inverted_index)` — [`L163`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L163) — Reconstruct plaintext abstract from OpenAlex inverted index.
- `work_to_bibtex(work)` — [`L104`](../../../../../../raw/code/bilevel-autoresearch/paper/bilevel-autoresearch/openalex_to_bibtex.py#L104) — Convert a single OpenAlex work object to a BibTeX entry string.

