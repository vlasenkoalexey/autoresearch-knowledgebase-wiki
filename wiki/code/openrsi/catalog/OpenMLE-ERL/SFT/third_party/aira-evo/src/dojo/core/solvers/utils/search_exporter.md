---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.search_exporter`/
symbols:
  test_export_and_reconstruct_search_data: test_export_and_reconstruct_search_data().
  export_search_results: export_search_results().
  SearchExporter.gather_and_export_search_results: SearchExporter#gather_and_export_search_results().
  SearchExporter.__init__: SearchExporter#__init__().
  SearchExporter: SearchExporter#
  SearchExporter.journal: SearchExporter#journal.
  SearchExporter.cfg: SearchExporter#cfg.
  logger: logger.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py)

## Classes
### `SearchExporter`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py:26`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L26)
- signature: `class SearchExporter:`
- members:
  - `gather_and_export_search_results(self, tree_path: str | Path | None = None, output_file: str | Path | None = None)` — [`L31`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L31) — Gather search data into a dictionary structure and optionally
  - `cfg` — [`L29`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L29)
  - `journal` — [`L28`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L28)
- protocol/private: `__init__`[`L27`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L27)
- uses (calls/refs, reference-scoped): [`Journal`](journal.md#Journal), [`generate`](tree_export.md#generate), [`export_data`](journal.md#Journal.export_data), [`logger`](search_exporter.md#logger)
- used by: [`test_export_and_reconstruct_search_data`](search_exporter.md#test_export_and_reconstruct_search_data), [`export_search_results`](search_exporter.md#export_search_results)

## Functions
- `export_search_results(cfg: DictConfig, journal: Journal, logger: CollectiveLogger, search_method: str)` — [`L77`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L77)
- `test_export_and_reconstruct_search_data()` — [`L99`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L99)

## Module values
- `logger` — [`L23`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/search_exporter.py#L23)

