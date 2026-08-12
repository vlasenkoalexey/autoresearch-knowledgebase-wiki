---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.operators.memory`/
symbols:
  create_memory_op: create_memory_op().
  get_node_summary: get_node_summary().
  generate_journal_summary: generate_journal_summary().
  generate_ancestral_summary: generate_ancestral_summary().
  get_sibling_summary: get_sibling_summary().
  MEM_OPS: MEM_OPS.
  simple_memory: simple_memory().
  ancestral_memory: ancestral_memory().
  sibling_memory: sibling_memory().
  create_memory_op.memory_op: create_memory_op().memory_op().
  no_memory: no_memory().
  log: log.
  truncate_string: truncate_string().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py)

## Functions
- `ancestral_memory(journal: Journal, node: Optional[Node] = None, **kwargs)` — [`L184`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L184)
- `create_memory_op(cfg: Optional[MemoryOpConfig])` — [`L28`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L28)
- `generate_ancestral_summary(node: Optional[Node], include_code: bool = False, include_buggy_nodes: bool = True, only_plans: bool = False, until_successful_parent: bool = True)` — [`L129`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L129) — Generate a summary of the ancestral journal for the agent.
- `generate_journal_summary(journal: Journal, include_code: bool = False, include_buggy_nodes: bool = False, only_plans: bool = False)` — [`L103`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L103) — Generate a summary of the journal for the agent.
- `get_node_summary(node: Node, include_code: bool = False, only_plans: bool = False)` — [`L65`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L65) — Generate a summary of the node for the agent.
- `get_sibling_summary(parent_node: Optional[Node], include_code: bool = False, include_buggy_nodes: bool = True, only_plans: bool = True)` — [`L200`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L200)
- `memory_op(journal: Journal, node: Optional[Node] = None)` — [`L37`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L37)
- `no_memory(journal: Journal, node: Optional[Node] = None, **kwargs)` — [`L192`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L192)
- `sibling_memory(journal: Journal, node: Optional[Node] = None, **kwargs)` — [`L227`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L227)
- `simple_memory(journal: Journal, node: Optional[Node] = None, max_length: Optional[int] = None, **kwargs)` — [`L169`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L169)
- `truncate_string(s: str, max_prefix: int = 100, max_suffix: int = 100)` — [`L56`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L56) — Truncate a string to 200 characters and add ellipsis.

## Module values
- `MEM_OPS` — [`L238`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L238)
- `log` — [`L23`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/operators/memory.py#L23)

