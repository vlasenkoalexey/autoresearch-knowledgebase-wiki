---
title: 'Module: tests/repl/test_custom_tools.py'
type: catalog
provenance: extracted
module: tests/repl/test_custom_tools.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.repl.test_custom_tools`/
symbols:
  TestCustomToolsWithContext.test_tools_can_access_context: TestCustomToolsWithContext#test_tools_can_access_context().
  TestCustomToolsWithContext.test_tools_with_string_context: TestCustomToolsWithContext#test_tools_with_string_context().
  TestCustomToolsEdgeCases.test_tool_with_closure: TestCustomToolsEdgeCases#test_tool_with_closure().
  TestCustomToolsEdgeCases.test_tool_returning_none: TestCustomToolsEdgeCases#test_tool_returning_none().
  TestCustomToolsEdgeCases.test_class_instance_as_tool: TestCustomToolsEdgeCases#test_class_instance_as_tool().
  TestParseToolEntry.test_plain_callable: TestParseToolEntry#test_plain_callable().
  TestParseToolEntry.test_dict_with_description: TestParseToolEntry#test_dict_with_description().
  TestLocalREPLCustomTools.test_callable_tool_available: TestLocalREPLCustomTools#test_callable_tool_available().
  TestLocalREPLCustomTools.test_callable_tool_with_args: TestLocalREPLCustomTools#test_callable_tool_with_args().
  TestLocalREPLCustomTools.test_non_callable_dict_available: TestLocalREPLCustomTools#test_non_callable_dict_available().
  TestLocalREPLCustomTools.test_non_callable_string_available: TestLocalREPLCustomTools#test_non_callable_string_available().
  TestLocalREPLCustomTools.test_tools_persist_across_executions: TestLocalREPLCustomTools#test_tools_persist_across_executions().
  TestLocalREPLCustomTools.test_empty_custom_tools: TestLocalREPLCustomTools#test_empty_custom_tools().
  TestLocalREPLCustomTools.test_none_custom_tools: TestLocalREPLCustomTools#test_none_custom_tools().
  TestLocalREPLCustomTools.test_builtin_functions_still_work: TestLocalREPLCustomTools#test_builtin_functions_still_work().
  TestCustomToolsEdgeCases.test_tool_that_raises_exception: TestCustomToolsEdgeCases#test_tool_that_raises_exception().
  TestCustomToolsEdgeCases.test_lambda_tool: TestCustomToolsEdgeCases#test_lambda_tool().
  TestCustomToolsEdgeCases.test_tool_name_shadowing_import: TestCustomToolsEdgeCases#test_tool_name_shadowing_import().
  TestParseToolEntry.test_plain_value: TestParseToolEntry#test_plain_value().
  TestParseToolEntry.test_dict_value_with_description: TestParseToolEntry#test_dict_value_with_description().
  TestParseToolEntry.test_dict_with_tool_but_no_description: TestParseToolEntry#test_dict_with_tool_but_no_description().
  TestParseToolEntry.test_plain_dict_without_tool_key: TestParseToolEntry#test_plain_dict_without_tool_key().
  TestParseCustomTools.test_mixed_tools: TestParseCustomTools#test_mixed_tools().
  TestToolsWithDescriptionsInREPL.test_callable_with_description_works: TestToolsWithDescriptionsInREPL#test_callable_with_description_works().
  TestToolsWithDescriptionsInREPL.test_value_with_description_works: TestToolsWithDescriptionsInREPL#test_value_with_description_works().
  TestToolsWithDescriptionsInREPL.test_mixed_tools_with_descriptions: TestToolsWithDescriptionsInREPL#test_mixed_tools_with_descriptions().
  TestLocalREPLCustomTools.test_supports_custom_tools_protocol: TestLocalREPLCustomTools#test_supports_custom_tools_protocol().
  TestParseToolEntry.func: TestParseToolEntry#func().
  custom_tools: custom_tools().
  TestValidateCustomTools.test_reserved_names_rejected: TestValidateCustomTools#test_reserved_names_rejected().
  TestExtractToolValue.test_plain_callable: TestExtractToolValue#test_plain_callable().
  TestExtractToolValue.test_dict_with_tool_key: TestExtractToolValue#test_dict_with_tool_key().
  TestExtractToolValue.func: TestExtractToolValue#func().
  TestValidateCustomTools.test_none_is_valid: TestValidateCustomTools#test_none_is_valid().
  TestValidateCustomTools.test_empty_dict_is_valid: TestValidateCustomTools#test_empty_dict_is_valid().
  TestValidateCustomTools.test_valid_tools_pass: TestValidateCustomTools#test_valid_tools_pass().
  TestValidateCustomTools.test_multiple_reserved_names_all_reported: TestValidateCustomTools#test_multiple_reserved_names_all_reported().
  TestValidateCustomTools.test_reserved_names_constant_is_frozen: TestValidateCustomTools#test_reserved_names_constant_is_frozen().
  TestLocalREPLCustomTools.test_reserved_name_raises_on_init: TestLocalREPLCustomTools#test_reserved_name_raises_on_init().
  TestCustomToolsEdgeCases.test_class_instance_as_tool.Adder.__call__: TestCustomToolsEdgeCases#test_class_instance_as_tool().Adder#__call__().
  TestExtractToolValue.test_plain_value: TestExtractToolValue#test_plain_value().
  TestExtractToolValue.test_plain_dict_without_tool_key: TestExtractToolValue#test_plain_dict_without_tool_key().
  TestParseCustomTools.test_none_returns_empty_list: TestParseCustomTools#test_none_returns_empty_list().
  TestParseCustomTools.test_empty_dict_returns_empty_list: TestParseCustomTools#test_empty_dict_returns_empty_list().
  TestFormatToolsForPrompt.test_none_returns_none: TestFormatToolsForPrompt#test_none_returns_none().
  TestFormatToolsForPrompt.test_empty_returns_none: TestFormatToolsForPrompt#test_empty_returns_none().
  TestFormatToolsForPrompt.test_callable_with_description: TestFormatToolsForPrompt#test_callable_with_description().
  TestFormatToolsForPrompt.test_callable_without_description: TestFormatToolsForPrompt#test_callable_without_description().
  TestFormatToolsForPrompt.test_value_with_description: TestFormatToolsForPrompt#test_value_with_description().
  TestFormatToolsForPrompt.test_value_without_description: TestFormatToolsForPrompt#test_value_without_description().
  TestFormatToolsForPrompt.test_multiple_tools_formatted: TestFormatToolsForPrompt#test_multiple_tools_formatted().
  TestToolsWithDescriptionsInREPL.test_described_tools_validate_reserved_names: TestToolsWithDescriptionsInREPL#test_described_tools_validate_reserved_names().
  sample_tool_function: sample_tool_function().
  another_tool_function: another_tool_function().
  TestCustomToolsWithContext.process_context: TestCustomToolsWithContext#process_context().
  TestCustomToolsWithContext.count_words: TestCustomToolsWithContext#count_words().
  TestCustomToolsEdgeCases.failing_tool: TestCustomToolsEdgeCases#failing_tool().
  TestCustomToolsEdgeCases.multiply: TestCustomToolsEdgeCases#multiply().
  TestCustomToolsEdgeCases.returns_none: TestCustomToolsEdgeCases#returns_none().
  TestCustomToolsEdgeCases.test_class_instance_as_tool.Adder: TestCustomToolsEdgeCases#test_class_instance_as_tool().Adder#
  Adder.n: Adder#n.
  TestParseCustomTools.func1: TestParseCustomTools#func1().
  TestParseCustomTools.func2: TestParseCustomTools#func2().
  TestValidateCustomTools: TestValidateCustomTools#
  TestLocalREPLCustomTools: TestLocalREPLCustomTools#
  TestCustomToolsWithContext: TestCustomToolsWithContext#
  TestCustomToolsEdgeCases: TestCustomToolsEdgeCases#
  TestCustomToolsEdgeCases.test_class_instance_as_tool.Adder.__init__: TestCustomToolsEdgeCases#test_class_instance_as_tool().Adder#__init__().
  TestParseToolEntry: TestParseToolEntry#
  TestExtractToolValue: TestExtractToolValue#
  TestParseCustomTools: TestParseCustomTools#
  TestFormatToolsForPrompt: TestFormatToolsForPrompt#
  TestToolsWithDescriptionsInREPL: TestToolsWithDescriptionsInREPL#
---
# Module: [`tests/repl/test_custom_tools.py`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py)

## Classes
### `Adder`
- def: [`tests/repl/test_custom_tools.py:300`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L300)
- signature: `class Adder:`
- members:
  - `n` — [`L302`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L302)
- protocol/private: `__call__`[`L304`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L304), `__init__`[`L301`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L301)
- used by: (1 test-only callers)

### `TestCustomToolsEdgeCases`
- def: [`tests/repl/test_custom_tools.py:241`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L241)
- doc: Edge case tests for custom tools.
- signature: `class TestCustomToolsEdgeCases:`
- members:
  - `failing_tool()` — [`L247`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L247)
  - `multiply(x)` — [`L262`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L262)
  - `returns_none()` — [`L276`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L276)
  - `test_class_instance_as_tool(self)` — [`L297`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L297) — Class instances with __call__ should work as tools.
  - `test_lambda_tool(self)` — [`L287`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L287) — Lambda functions should work as tools.
  - `test_tool_name_shadowing_import(self)` — [`L315`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L315) — Custom tools shouldn't prevent importing modules with same name.
  - `test_tool_returning_none(self)` — [`L273`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L273) — Tools returning None should work correctly.
  - `test_tool_that_raises_exception(self)` — [`L244`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L244) — Tools that raise exceptions should propagate errors properly.
  - `test_tool_with_closure(self)` — [`L258`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L258) — Tools with closures should work correctly.
- uses (calls/refs, reference-scoped): [`execute_code`](../../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../../rlm/core/types.md#REPLResult.stderr), [`locals`](../../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../../rlm/environments/local_repl.md#LocalREPL.cleanup)  (1 test-only)

### `TestCustomToolsWithContext`
- def: [`tests/repl/test_custom_tools.py:203`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L203)
- doc: Tests for custom tools interacting with context.
- signature: `class TestCustomToolsWithContext:`
- members:
  - `count_words(text)` — [`L226`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L226)
  - `process_context(ctx)` — [`L209`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L209)
  - `test_tools_can_access_context(self)` — [`L206`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L206) — Custom tools should be able to work with context data.
  - `test_tools_with_string_context(self)` — [`L223`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L223) — Custom tools should work with string context.
- uses (calls/refs, reference-scoped): [`execute_code`](../../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../../rlm/core/types.md#REPLResult.stderr), [`locals`](../../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestExtractToolValue`
- def: [`tests/repl/test_custom_tools.py:409`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L409)
- doc: Tests for extract_tool_value function.
- signature: `class TestExtractToolValue:`
- members:
  - `func(x)` — [`L420`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L420)
  - `test_dict_with_tool_key(self)` — [`L425`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L425) — Dict with 'tool' key should return just the tool value.
  - `test_plain_callable(self)` — [`L417`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L417) — Plain callable should be returned as-is.
  - `test_plain_dict_without_tool_key(self)` — [`L436`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L436) — Dict without 'tool' key should return whole dict.
  - `test_plain_value(self)` — [`L412`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L412) — Plain value should be returned as-is.
- uses (calls/refs, reference-scoped): [`extract_tool_value`](../../rlm/environments/base_env.md#extract_tool_value)

### `TestFormatToolsForPrompt`
- def: [`tests/repl/test_custom_tools.py:481`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L481)
- doc: Tests for format_tools_for_prompt function.
- signature: `class TestFormatToolsForPrompt:`
- members:
  - `test_callable_with_description(self)` — [`L492`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L492) — Callable with description should show description.
  - `test_callable_without_description(self)` — [`L500`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L500) — Callable without description should show generic message.
  - `test_empty_returns_none(self)` — [`L488`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L488) — Empty tools should return None.
  - `test_multiple_tools_formatted(self)` — [`L524`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L524) — Multiple tools should all appear in output.
  - `test_none_returns_none(self)` — [`L484`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L484) — None tools should return None.
  - `test_value_with_description(self)` — [`L508`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L508) — Value with description should show description.
  - `test_value_without_description(self)` — [`L516`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L516) — Value without description should show type.
- uses (calls/refs, reference-scoped): [`format_tools_for_prompt`](../../rlm/environments/base_env.md#format_tools_for_prompt)

### `TestLocalREPLCustomTools`
- def: [`tests/repl/test_custom_tools.py:100`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L100)
- doc: Tests for custom tools in LocalREPL.
- signature: `class TestLocalREPLCustomTools:`
- members:
  - `test_builtin_functions_still_work(self, custom_tools)` — [`L186`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L186) — Built-in REPL functions should still work with custom tools.
  - `test_callable_tool_available(self, custom_tools)` — [`L109`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L109) — Callable tools should be available as functions.
  - `test_callable_tool_with_args(self, custom_tools)` — [`L119`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L119) — Callable tools should work with multiple arguments.
  - `test_empty_custom_tools(self)` — [`L166`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L166) — Empty custom_tools dict should work fine.
  - `test_non_callable_dict_available(self, custom_tools)` — [`L129`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L129) — Non-callable dict tools should be available as variables.
  - `test_non_callable_string_available(self, custom_tools)` — [`L139`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L139) — Non-callable string tools should be available as variables.
  - `test_none_custom_tools(self)` — [`L176`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L176) — None custom_tools should work fine (default behavior).
  - `test_reserved_name_raises_on_init(self)` — [`L160`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L160) — Using a reserved name should raise ValueError during initialization.
  - `test_supports_custom_tools_protocol(self)` — [`L103`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L103) — LocalREPL should implement SupportsCustomTools protocol.
  - `test_tools_persist_across_executions(self, custom_tools)` — [`L149`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L149) — Custom tools should remain available across multiple executions.
- uses (calls/refs, reference-scoped): [`execute_code`](../../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../../rlm/core/types.md#REPLResult.stderr), [`stdout`](../../rlm/core/types.md#REPLResult.stdout), [`locals`](../../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../../rlm/environments/local_repl.md#LocalREPL.cleanup), [`final_answer`](../../rlm/core/types.md#REPLResult.final_answer), [`SupportsCustomTools`](../../rlm/environments/base_env.md#SupportsCustomTools)

### `TestParseCustomTools`
- def: [`tests/repl/test_custom_tools.py:442`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L442)
- doc: Tests for parse_custom_tools function.
- signature: `class TestParseCustomTools:`
- members:
  - `func1(x)` — [`L456`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L456)
  - `func2(x)` — [`L459`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L459)
  - `test_empty_dict_returns_empty_list(self)` — [`L449`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L449) — Empty dict should return empty list.
  - `test_mixed_tools(self)` — [`L453`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L453) — Mix of plain and described tools.
  - `test_none_returns_empty_list(self)` — [`L445`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L445) — None should return empty list.
- uses (calls/refs, reference-scoped): [`description`](../../rlm/environments/base_env.md#ToolInfo.description), [`name`](../../rlm/environments/base_env.md#ToolInfo.name), [`parse_custom_tools`](../../rlm/environments/base_env.md#parse_custom_tools)

### `TestParseToolEntry`
- def: [`tests/repl/test_custom_tools.py:338`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L338)
- doc: Tests for parse_tool_entry function.
- signature: `class TestParseToolEntry:`
- members:
  - `func(x)` — [`L344`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L344)
  - `test_dict_value_with_description(self)` — [`L376`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L376) — Non-callable with description.
  - `test_dict_with_description(self)` — [`L363`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L363) — Dict with 'tool' and 'description' keys should extract both.
  - `test_dict_with_tool_but_no_description(self)` — [`L387`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L387) — Dict with 'tool' key but no description.
  - `test_plain_callable(self)` — [`L341`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L341) — Plain callable should have no description.
  - `test_plain_dict_without_tool_key(self)` — [`L399`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L399) — Plain dict without 'tool' key should be treated as data value.
  - `test_plain_value(self)` — [`L354`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L354) — Plain value should have no description.
- uses (calls/refs, reference-scoped): [`parse_tool_entry`](../../rlm/environments/base_env.md#parse_tool_entry), [`description`](../../rlm/environments/base_env.md#ToolInfo.description), [`name`](../../rlm/environments/base_env.md#ToolInfo.name), [`value`](../../rlm/environments/base_env.md#ToolInfo.value), [`is_callable`](../../rlm/environments/base_env.md#ToolInfo.is_callable)

### `TestToolsWithDescriptionsInREPL`
- def: [`tests/repl/test_custom_tools.py:542`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L542)
- doc: Tests for tools with descriptions in LocalREPL.
- signature: `class TestToolsWithDescriptionsInREPL:`
- members:
  - `test_callable_with_description_works(self)` — [`L545`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L545) — Callable tool with description should work in REPL.
  - `test_described_tools_validate_reserved_names(self)` — [`L596`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L596) — Described tools should still validate against reserved names.
  - `test_mixed_tools_with_descriptions(self)` — [`L573`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L573) — Mix of described and undescribed tools should work.
  - `test_value_with_description_works(self)` — [`L559`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L559) — Value tool with description should work in REPL.
- uses (calls/refs, reference-scoped): [`execute_code`](../../rlm/environments/local_repl.md#LocalREPL.execute_code), [`stderr`](../../rlm/core/types.md#REPLResult.stderr), [`locals`](../../rlm/environments/local_repl.md#LocalREPL.locals), [`LocalREPL`](../../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../../rlm/environments/local_repl.md#LocalREPL.cleanup)

### `TestValidateCustomTools`
- def: [`tests/repl/test_custom_tools.py:56`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L56)
- doc: Tests for the validate_custom_tools function.
- signature: `class TestValidateCustomTools:`
- members:
  - `test_empty_dict_is_valid(self)` — [`L63`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L63) — Empty dict should pass validation.
  - `test_multiple_reserved_names_all_reported(self)` — [`L79`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L79) — When multiple reserved names are used, all should be reported.
  - `test_none_is_valid(self)` — [`L59`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L59) — None custom_tools should pass validation.
  - `test_reserved_names_constant_is_frozen(self)` — [`L88`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L88) — RESERVED_TOOL_NAMES should be immutable.
  - `test_reserved_names_rejected(self, reserved_name)` — [`L72`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L72) — Each reserved name should be rejected.
  - `test_valid_tools_pass(self, custom_tools)` — [`L67`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L67) — Valid custom tools should pass validation.
- uses (calls/refs, reference-scoped): [`validate_custom_tools`](../../rlm/environments/base_env.md#validate_custom_tools), [`RESERVED_TOOL_NAMES`](../../rlm/environments/base_env.md#RESERVED_TOOL_NAMES.RESERVED_TOOL_NAMES)

## Functions
- `another_tool_function(a: str, b: str)` — [`L35`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L35) — Another test function.
- `custom_tools()` — [`L41`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L41) — Standard set of custom tools for testing.
- `sample_tool_function(x: int)` — [`L30`](../../../../../../raw/code/rlm/tests/repl/test_custom_tools.py#L30) — A simple test function.

