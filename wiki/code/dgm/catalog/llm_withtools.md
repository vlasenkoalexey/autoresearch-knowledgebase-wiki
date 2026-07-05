---
title: 'Module: llm_withtools.py'
type: catalog
provenance: extracted
module: llm_withtools.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 llm_withtools/
symbols:
  chat_with_agent: chat_with_agent().
  chat_with_agent_manualtools: chat_with_agent_manualtools().
  chat_with_agent_claude: chat_with_agent_claude().
  chat_with_agent_openai: chat_with_agent_openai().
  convert_msg_history: convert_msg_history().
  get_response_withtools: get_response_withtools().
  check_for_tool_use: check_for_tool_use().
  msg: msg.
  CLAUDE_MODEL: CLAUDE_MODEL.
  convert_tool_info: convert_tool_info().
  convert_tool_info.add_additional_properties: convert_tool_info().add_additional_properties().
  convert_msg_history_claude: convert_msg_history_claude().
  OPENAI_MODEL: OPENAI_MODEL.
  process_tool_call: process_tool_call().
  convert_block_claude: convert_block_claude().
  convert_msg_history_openai: convert_msg_history_openai().
---
# Module: [`llm_withtools.py`](../../../../raw/code/dgm/llm_withtools.py)

## Functions
- `add_additional_properties(d)` — [`L122`](../../../../raw/code/dgm/llm_withtools.py#L122) — documented in [coding_agent](../concepts/coding_agent.md)
- `chat_with_agent(msg, model=CLAUDE_MODEL, msg_history=None, logging=print, convert=False)` — [`L514`](../../../../raw/code/dgm/llm_withtools.py#L514) — documented in [coding_agent](../concepts/coding_agent.md)
- `chat_with_agent_claude(msg, model='bedrock/us.anthropic.claude-3-5-sonnet-20241022-v2:0', msg_history=None, logging=print)` — [`L338`](../../../../raw/code/dgm/llm_withtools.py#L338) — documented in [coding_agent](../concepts/coding_agent.md)
- `chat_with_agent_manualtools(msg, model, msg_history=None, logging=print)` — [`L282`](../../../../raw/code/dgm/llm_withtools.py#L282) — documented in [coding_agent](../concepts/coding_agent.md)
- `chat_with_agent_openai(msg, model='o3-mini-2025-01-31', msg_history=None, logging=print)` — [`L427`](../../../../raw/code/dgm/llm_withtools.py#L427) — documented in [coding_agent](../concepts/coding_agent.md)
- `check_for_tool_use(response, model='')` — [`L67`](../../../../raw/code/dgm/llm_withtools.py#L67) — Checks if the response contains a tool call. — documented in [coding_agent](../concepts/coding_agent.md)
- `convert_block_claude(block)` — [`L148`](../../../../raw/code/dgm/llm_withtools.py#L148) — Convert a single block of content from Claude into a standard format. — documented in [coding_agent](../concepts/coding_agent.md)
- `convert_msg_history(msg_history, model=None)` — [`L271`](../../../../raw/code/dgm/llm_withtools.py#L271) — Convert message history from the model-specific format to a generic format. — documented in [coding_agent](../concepts/coding_agent.md)
- `convert_msg_history_claude(msg_history)` — [`L190`](../../../../raw/code/dgm/llm_withtools.py#L190) — Convert Claude-style message history into a generic format. — documented in [coding_agent](../concepts/coding_agent.md)
- `convert_msg_history_openai(msg_history)` — [`L211`](../../../../raw/code/dgm/llm_withtools.py#L211) — Convert OpenAI-style message history into a generic format. — documented in [coding_agent](../concepts/coding_agent.md)
- `convert_tool_info(tool_info, model=None)` — [`L110`](../../../../raw/code/dgm/llm_withtools.py#L110) — Converts tool_info from Claude format to the given model's format. — documented in [coding_agent](../concepts/coding_agent.md)
- `get_response_withtools(client, model, messages, tools, tool_choice, logging=None, max_retry=3)` — [`L31`](../../../../raw/code/dgm/llm_withtools.py#L31) — documented in [coding_agent](../concepts/coding_agent.md)
- `process_tool_call(tools_dict, tool_name, tool_input)` — [`L16`](../../../../raw/code/dgm/llm_withtools.py#L16) — documented in [coding_agent](../concepts/coding_agent.md)

## Module values
- `CLAUDE_MODEL` — [`L13`](../../../../raw/code/dgm/llm_withtools.py#L13) — documented in [coding_agent](../concepts/coding_agent.md)
- `OPENAI_MODEL` — [`L14`](../../../../raw/code/dgm/llm_withtools.py#L14)
- `msg` — [`L552`](../../../../raw/code/dgm/llm_withtools.py#L552) — documented in [llm_withtools](../concepts/llm_withtools.md)

