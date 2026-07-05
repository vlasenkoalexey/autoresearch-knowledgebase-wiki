---
title: 'Module: ai_scientist/tools/semantic_scholar.py'
type: catalog
provenance: extracted
module: ai_scientist/tools/semantic_scholar.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.tools.semantic_scholar`/
symbols:
  SemanticScholarSearchTool.search_for_papers: SemanticScholarSearchTool#search_for_papers().
  search_for_papers: search_for_papers().
  SemanticScholarSearchTool.S2_API_KEY: SemanticScholarSearchTool#S2_API_KEY.
  SemanticScholarSearchTool.use_tool: SemanticScholarSearchTool#use_tool().
  SemanticScholarSearchTool: SemanticScholarSearchTool#
  SemanticScholarSearchTool.__init__: SemanticScholarSearchTool#__init__().
  on_backoff: on_backoff().
  SemanticScholarSearchTool.max_results: SemanticScholarSearchTool#max_results.
  SemanticScholarSearchTool.format_papers: SemanticScholarSearchTool#format_papers().
---
# Module: [`ai_scientist/tools/semantic_scholar.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py)

## Classes
### `SemanticScholarSearchTool`  ·  implements/extends BaseTool
- def: [`ai_scientist/tools/semantic_scholar.py:19`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L19) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
- signature: `class SemanticScholarSearchTool(BaseTool):`
- members:
  - `format_papers(self, papers: List[Dict])` — [`L87`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L87) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
  - `search_for_papers(self, query: str)` — [`L57`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L57) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
  - `use_tool(self, query: str)` — [`L45`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L45) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
  - `S2_API_KEY` — [`L38`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L38) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
  - `max_results` — [`L37`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L37)
- protocol/private: `__init__`[`L20`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L20)
- uses (calls/refs, reference-scoped): [`BaseTool`](base_tool.md#BaseTool), [`on_backoff`](semantic_scholar.md#on_backoff), [`__init__`](base_tool.md#BaseTool.__init__)
- used by: [`BaseTool`](base_tool.md#BaseTool), [`semantic_scholar_tool`](../perform_ideation_temp_free.md#semantic_scholar_tool), [`use_tool`](base_tool.md#BaseTool.use_tool)

## Functions
- `on_backoff(details: Dict)` — [`L12`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L12) — documented in [ai_scientist-perform_icbinb_writeup](../../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `search_for_papers(query, result_limit=10)` — [`L104`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/semantic_scholar.py#L104) — documented in [ai_scientist-perform_icbinb_writeup](../../../concepts/ai_scientist-perform_icbinb_writeup.md)

