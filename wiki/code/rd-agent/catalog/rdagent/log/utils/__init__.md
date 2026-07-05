---
title: 'Module: rdagent/log/utils/__init__.py'
type: catalog
provenance: extracted
module: rdagent/log/utils/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.utils`/
symbols:
  LogColors: LogColors#
  LogColors.END: LogColors#END.
  dict_get_with_warning: dict_get_with_warning().
  LogColors.CYAN: LogColors#CYAN.
  extract_json: extract_json().
  extract_loopid_func_name: extract_loopid_func_name().
  extract_evoid: extract_evoid().
  LogColors.render: LogColors#render().
  is_valid_session: is_valid_session().
  get_caller_info: get_caller_info().
  gen_datetime: gen_datetime().
  LogColors.get_all_colors: LogColors#get_all_colors().
  LogColors.MAGENTA: LogColors#MAGENTA.
  LogColors.GREEN: LogColors#GREEN.
  LogColors.BLUE: LogColors#BLUE.
  LogColors.BOLD: LogColors#BOLD.
  CallerInfo: CallerInfo#
  LogColors.RED: LogColors#RED.
  LogColors.YELLOW: LogColors#YELLOW.
  LogColors.remove_ansi_codes: LogColors#remove_ansi_codes().
  LogColors.WHITE: LogColors#WHITE.
  LogColors.GRAY: LogColors#GRAY.
  LogColors.BLACK: LogColors#BLACK.
  LogColors.ITALIC: LogColors#ITALIC.
  CallerInfo.line: CallerInfo#line.
  CallerInfo.name: CallerInfo#name.
---
# Module: [`rdagent/log/utils/__init__.py`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py)

## Classes
### `CallerInfo`  ·  implements/extends _TypedDict
- def: [`rdagent/log/utils/__init__.py:63`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L63)
- signature: `class CallerInfo(TypedDict):`
- members:
  - `line` — [`L65`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L65)
  - `name` — [`L66`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L66)
- used by: [`get_caller_info`](__init__.md#get_caller_info)

### `LogColors`
- def: [`rdagent/log/utils/__init__.py:9`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L9) — documented in [rdagent-oai-backend-base](../../../../concepts/rdagent-oai-backend-base.md)
- doc: ANSI color codes for use in console output.
- signature: `class LogColors:`
- members:
  - `get_all_colors(cls: type[LogColors])` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L30)
  - `remove_ansi_codes(s: str)` — [`L55`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L55) — It is for removing ansi ctrl characters in the string(e.g. colored text)
  - `render(self, text: str, color: str = "", style: str = "")` — [`L35`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L35) — render text by input color and style.
  - `BLACK` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L22)
  - `BLUE` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L17)
  - `BOLD` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L24)
  - `CYAN` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L19)
  - `END` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L27) — documented in [rdagent-oai-backend-base](../../../../concepts/rdagent-oai-backend-base.md)
  - `GRAY` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L21)
  - `GREEN` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L15)
  - `ITALIC` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L25)
  - `MAGENTA` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L18)
  - `RED` — [`L14`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L14)
  - `WHITE` — [`L20`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L20)
  - `YELLOW` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L16)
- used by: [`_create_chat_completion_inner_function`](../../oai/backend/deprec.md#DeprecBackend._create_chat_completion_inner_function), [`_create_chat_completion_auto_continue`](../../oai/backend/base.md#APIBackend._create_chat_completion_auto_continue), [`_create_chat_completion_inner_function`](../../oai/backend/litellm.md#LiteLLMAPIBackend._create_chat_completion_inner_function), [`_create_embedding_inner_function`](../../oai/backend/litellm.md#LiteLLMAPIBackend._create_embedding_inner_function), [`_calculate_token_from_messages`](../../oai/backend/litellm.md#LiteLLMAPIBackend._calculate_token_from_messages), [`_build_log_messages`](../../oai/backend/base.md#APIBackend._build_log_messages), [`stdout_win`](../ui/ds_trace.md#stdout_win)

## Functions
- `dict_get_with_warning(d: dict, key: str, default: Any = None)` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L117) — Motivation:
- `extract_evoid(tag: str)` — [`L93`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L93) — extract evo id from the tag in Message
- `extract_json(log_content: str)` — [`L99`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L99)
- `extract_loopid_func_name(tag: str)` — [`L87`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L87) — extract loop id and function name from the tag in Message
- `gen_datetime(dt: datetime | None = None)` — [`L106`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L106) — Generate a datetime object in UTC timezone.
- `get_caller_info(level: int = 2)` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L69)
- `is_valid_session(log_path: Path)` — [`L83`](../../../../../../../raw/code/rd-agent/rdagent/log/utils/__init__.py#L83)

