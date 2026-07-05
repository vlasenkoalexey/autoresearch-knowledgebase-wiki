---
title: 'Module: ai_scientist/treesearch/utils/__init__.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/__init__.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils`/
symbols:
  preproc_data: preproc_data().
  extract_archives: extract_archives().
  logger: logger.
  copytree: copytree().
  clean_up_dataset: clean_up_dataset().
---
# Module: [`ai_scientist/treesearch/utils/__init__.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py)

## Functions
- `clean_up_dataset(path: Path)` — [`L40`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py#L40) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `copytree(src: Path, dst: Path, use_symlinks=True)` — [`L9`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py#L9) — Copy contents of `src` to `dst`. Unlike shutil.copytree, the dst dir can exist and will be merged. — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `extract_archives(path: Path)` — [`L49`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py#L49) — unzips all .zip files within `path` and cleans up task dir — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)
- `preproc_data(path: Path)` — [`L98`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py#L98) — documented in [ai_scientist-treesearch-utils-config](../../../../concepts/ai_scientist-treesearch-utils-config.md)

## Module values
- `logger` — [`L6`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/__init__.py#L6)

