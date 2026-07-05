---
title: 'Module: ai_scientist/treesearch/utils/serialize.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/serialize.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.serialize`/
symbols:
  loads_json: loads_json().
  dumps_json: dumps_json().
  load_json: load_json().
  G: G.
  dump_json: dump_json().
  parse_markdown_to_dict: parse_markdown_to_dict().
---
# Module: [`ai_scientist/treesearch/utils/serialize.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py)

## Functions
- `dump_json(obj: dataclasses_json.DataClassJsonMixin, path: Path)` — [`L34`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L34)
- `dumps_json(obj: dataclasses_json.DataClassJsonMixin)` — [`L11`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L11) — Serialize dataclasses (such as Journals) to JSON. — documented in [ai_scientist-treesearch-journal](../../../../concepts/ai_scientist-treesearch-journal.md)
- `load_json(path: Path, cls: Type[G])` — [`L55`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L55)
- `loads_json(s: str, cls: Type[G])` — [`L42`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L42) — Deserialize JSON to AIDE dataclasses. — documented in [ai_scientist-treesearch-journal](../../../../concepts/ai_scientist-treesearch-journal.md)
- `parse_markdown_to_dict(content: str)` — [`L60`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L60) — Reads a file that contains lines of the form:

## Module values
- `G` — [`L39`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/serialize.py#L39)

