---
title: 'Module: rdagent/components/agent/context7/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/agent/context7/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.agent.context7`/Agent#
symbols:
  Agent.__init__: __init__().
  Agent._build_enhanced_query: _build_enhanced_query().
  Agent.query: query().
  Agent: ''
---
# Module: [`rdagent/components/agent/context7/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/agent/context7/__init__.py)

## Classes
### `Agent`  ·  implements/extends PAIAgent
- def: [`rdagent/components/agent/context7/__init__.py:11`](../../../../../../../../raw/code/rd-agent/rdagent/components/agent/context7/__init__.py#L11)
- doc: A specific agent for context7
- signature: `class Agent(PAIAgent):`
- members:
  - `_build_enhanced_query(self, error_message: str, full_code: Optional[str] = None)` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/agent/context7/__init__.py#L25) — Build enhanced query using experimental prompt templates.
  - `query(self, query: str)` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/components/agent/context7/__init__.py#L46) — Parameters
- protocol/private: `__init__`[`L16`](../../../../../../../../raw/code/rd-agent/rdagent/components/agent/context7/__init__.py#L16)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`query`](../base.md#PAIAgent.query), [`PAIAgent`](../base.md#PAIAgent), [`__init__`](../base.md#PAIAgent.__init__), [`SETTINGS`](conf.md#SETTINGS), [`enable_cache`](conf.md#Settings.enable_cache), [`timeout`](conf.md#Settings.timeout), [`url`](conf.md#Settings.url)
- used by: [`evaluate`](../../coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`query`](../base.md#PAIAgent.query), [`PAIAgent`](../base.md#PAIAgent)  (2 test-only)

