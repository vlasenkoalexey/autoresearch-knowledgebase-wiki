---
title: 'Module: ai_scientist/tools/base_tool.py'
type: catalog
provenance: extracted
module: ai_scientist/tools/base_tool.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.tools.base_tool`/BaseTool#
symbols:
  BaseTool: ''
  BaseTool.use_tool: use_tool().
  BaseTool.name: name.
  BaseTool.description: description.
  BaseTool.__init__: __init__().
  BaseTool.parameters: parameters.
---
# Module: [`ai_scientist/tools/base_tool.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py)

## Classes
### `BaseTool`  ·  implements/extends ABC
- def: [`ai_scientist/tools/base_tool.py:5`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L5) — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
- doc: An abstract base class for defining custom tools.
- signature: `class BaseTool(ABC):`
- members:
  - `use_tool(self, **kwargs)` — [`L26`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L26) — Abstract method that should be implemented by subclasses to define the functionality of the tool. — documented in [ai_scientist-perform_ideation_temp_free](../../../concepts/ai_scientist-perform_ideation_temp_free.md)
  - `description` — [`L22`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L22)
  - `name` — [`L21`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L21)
  - `parameters` — [`L23`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L23)
- protocol/private: `__init__`[`L20`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/tools/base_tool.py#L20)
- uses (calls/refs, reference-scoped): [`use_tool`](semantic_scholar.md#SemanticScholarSearchTool.use_tool), [`SemanticScholarSearchTool`](semantic_scholar.md#SemanticScholarSearchTool)
- used by: [`generate_temp_free_idea`](../perform_ideation_temp_free.md#generate_temp_free_idea), [`tool_descriptions`](../perform_ideation_temp_free.md#tool_descriptions), [`tools_dict`](../perform_ideation_temp_free.md#tools_dict), [`tool_names`](../perform_ideation_temp_free.md#tool_names), [`SemanticScholarSearchTool`](semantic_scholar.md#SemanticScholarSearchTool), [`__init__`](semantic_scholar.md#SemanticScholarSearchTool.__init__)

