---
title: 'Module: rdagent/components/agent/base.py'
type: catalog
provenance: extracted
module: rdagent/components/agent/base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.agent.base`/
symbols:
  PAIAgent.query: PAIAgent#query().
  PAIAgent: PAIAgent#
  PAIAgent.__init__: PAIAgent#__init__().
  PAIAgent._run_query: PAIAgent#_run_query().
  BaseAgent: BaseAgent#
  PAIAgent._cached_query: PAIAgent#_cached_query.
  BaseAgent.query: BaseAgent#query().
  PAIAgent.agent: PAIAgent#agent.
  PAIAgent.enable_cache: PAIAgent#enable_cache.
  BaseAgent.__init__: BaseAgent#__init__().
---
# Module: [`rdagent/components/agent/base.py`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py)

## Classes
### `BaseAgent`
- def: [`rdagent/components/agent/base.py:12`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L12)
- signature: `class BaseAgent:`
- members:
  - `query(self, query: str)` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L18)
- protocol/private: `__init__`[`L15`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L15)
- uses (calls/refs, reference-scoped): [`query`](base.md#PAIAgent.query), [`PAIAgent`](base.md#PAIAgent)
- used by: [`PAIAgent`](base.md#PAIAgent)

### `PAIAgent`  ·  implements/extends BaseAgent
- def: [`rdagent/components/agent/base.py:21`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L21)
- doc: Pydantic-AI agent with optional Prefect caching support
- signature: `class PAIAgent(BaseAgent):`
- members:
  - `__init__(self, system_prompt: str, toolsets: list[str | MCPServerStreamableHTTP], enable_cache: bool = False)` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L29) — Initialize Pydantic-AI agent
  - `_run_query(self, query: str)` — [`L56`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L56) — Internal query execution (no caching)
  - `query(self, query: str)` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L64) — Run agent query with optional caching
  - `agent` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L26)
  - `enable_cache` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L27)
- protocol/private: `_cached_query`[`L54`](../../../../../../../raw/code/rd-agent/rdagent/components/agent/base.py#L54)
- uses (calls/refs, reference-scoped): [`get_agent_model`](../../oai/backend/pydantic_ai.md#get_agent_model), [`query`](context7/__init__.md#Agent.query), [`Agent`](context7/__init__.md#Agent), [`Agent`](rag/__init__.md#Agent), [`BaseAgent`](base.md#BaseAgent)
- used by: [`hypothesis_gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`__init__`](context7/__init__.md#Agent.__init__), [`__init__`](rag/__init__.md#Agent.__init__), [`query`](context7/__init__.md#Agent.query), [`Agent`](context7/__init__.md#Agent), [`Agent`](rag/__init__.md#Agent), [`BaseAgent`](base.md#BaseAgent), [`query`](base.md#BaseAgent.query)

