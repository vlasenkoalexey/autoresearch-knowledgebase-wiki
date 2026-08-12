---
title: 'Module: tests/test_types.py'
type: catalog
provenance: extracted
module: tests/test_types.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_types`/Test
symbols:
  TestRLMChatCompletion.test_metadata_roundtrip: RLMChatCompletion#test_metadata_roundtrip().
  TestRLMIteration.test_to_dict: RLMIteration#test_to_dict().
  TestRLMChatCompletion.test_metadata_default_none: RLMChatCompletion#test_metadata_default_none().
  TestRLMMetadata.test_to_dict: RLMMetadata#test_to_dict().
  TestUsageSummary.test_to_dict: UsageSummary#test_to_dict().
  TestModelUsageSummary.test_to_dict: ModelUsageSummary#test_to_dict().
  TestModelUsageSummary.test_from_dict: ModelUsageSummary#test_from_dict().
  TestCodeBlock.test_to_dict: CodeBlock#test_to_dict().
  TestRLMIteration.test_basic_creation: RLMIteration#test_basic_creation().
  TestRLMIteration.test_with_final_answer: RLMIteration#test_with_final_answer().
  TestUsageSummary.test_from_dict: UsageSummary#test_from_dict().
  TestREPLResult.test_basic_creation: REPLResult#test_basic_creation().
  TestQueryMetadata.test_string_prompt: QueryMetadata#test_string_prompt().
  TestSerializeValue.test_callable: SerializeValue#test_callable().
  TestREPLResult.test_to_dict: REPLResult#test_to_dict().
  TestSerializeValue.test_primitives: SerializeValue#test_primitives().
  TestSerializeValue.test_list: SerializeValue#test_list().
  TestSerializeValue.test_dict: SerializeValue#test_dict().
  TestREPLResult.test_str_representation: REPLResult#test_str_representation().
  TestSerializeValue.my_func: SerializeValue#my_func().
  TestSerializeValue: SerializeValue#
  TestModelUsageSummary: ModelUsageSummary#
  TestUsageSummary: UsageSummary#
  TestREPLResult: REPLResult#
  TestCodeBlock: CodeBlock#
  TestRLMIteration: RLMIteration#
  TestRLMChatCompletion: RLMChatCompletion#
  TestQueryMetadata: QueryMetadata#
  TestRLMMetadata: RLMMetadata#
---
# Module: [`tests/test_types.py`](../../../../../raw/code/rlm/tests/test_types.py)

## Classes
### `TestCodeBlock`
- def: [`tests/test_types.py:116`](../../../../../raw/code/rlm/tests/test_types.py#L116)
- doc: Tests for CodeBlock.
- signature: `class TestCodeBlock:`
- members:
  - `test_to_dict(self)` — [`L119`](../../../../../raw/code/rlm/tests/test_types.py#L119)
- uses (calls/refs, reference-scoped): [`REPLResult`](../rlm/core/types.md#REPLResult), [`result`](../rlm/core/types.md#CodeBlock.result), [`CodeBlock`](../rlm/core/types.md#CodeBlock), [`code`](../rlm/core/types.md#CodeBlock.code), [`to_dict`](../rlm/core/types.md#CodeBlock.to_dict)

### `TestModelUsageSummary`
- def: [`tests/test_types.py:43`](../../../../../raw/code/rlm/tests/test_types.py#L43)
- doc: Tests for ModelUsageSummary.
- signature: `class TestModelUsageSummary:`
- members:
  - `test_from_dict(self)` — [`L55`](../../../../../raw/code/rlm/tests/test_types.py#L55)
  - `test_to_dict(self)` — [`L46`](../../../../../raw/code/rlm/tests/test_types.py#L46)
- uses (calls/refs, reference-scoped): [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`to_dict`](../rlm/core/types.md#ModelUsageSummary.to_dict), [`from_dict`](../rlm/core/types.md#ModelUsageSummary.from_dict)

### `TestQueryMetadata`
- def: [`tests/test_types.py:193`](../../../../../raw/code/rlm/tests/test_types.py#L193)
- doc: Tests for QueryMetadata.
- signature: `class TestQueryMetadata:`
- members:
  - `test_string_prompt(self)` — [`L196`](../../../../../raw/code/rlm/tests/test_types.py#L196)
- uses (calls/refs, reference-scoped): [`context_lengths`](../rlm/core/types.md#QueryMetadata.context_lengths), [`QueryMetadata`](../rlm/core/types.md#QueryMetadata), [`context_type`](../rlm/core/types.md#QueryMetadata.context_type), [`context_total_length`](../rlm/core/types.md#QueryMetadata.context_total_length)

### `TestREPLResult`
- def: [`tests/test_types.py:93`](../../../../../raw/code/rlm/tests/test_types.py#L93)
- doc: Tests for REPLResult.
- signature: `class TestREPLResult:`
- members:
  - `test_basic_creation(self)` — [`L96`](../../../../../raw/code/rlm/tests/test_types.py#L96)
  - `test_str_representation(self)` — [`L109`](../../../../../raw/code/rlm/tests/test_types.py#L109)
  - `test_to_dict(self)` — [`L102`](../../../../../raw/code/rlm/tests/test_types.py#L102)
- uses (calls/refs, reference-scoped): [`stderr`](../rlm/core/types.md#REPLResult.stderr), [`stdout`](../rlm/core/types.md#REPLResult.stdout), [`REPLResult`](../rlm/core/types.md#REPLResult), [`to_dict`](../rlm/core/types.md#REPLResult.to_dict), [`locals`](../rlm/core/types.md#REPLResult.locals)

### `TestRLMChatCompletion`
- def: [`tests/test_types.py:160`](../../../../../raw/code/rlm/tests/test_types.py#L160)
- doc: Tests for RLMChatCompletion.
- signature: `class TestRLMChatCompletion:`
- members:
  - `test_metadata_default_none(self)` — [`L163`](../../../../../raw/code/rlm/tests/test_types.py#L163)
  - `test_metadata_roundtrip(self)` — [`L176`](../../../../../raw/code/rlm/tests/test_types.py#L176)
- uses (calls/refs, reference-scoped): [`response`](../rlm/core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../rlm/core/types.md#RLMChatCompletion), [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`metadata`](../rlm/core/types.md#RLMChatCompletion.metadata), [`usage_summary`](../rlm/core/types.md#RLMChatCompletion.usage_summary), [`execution_time`](../rlm/core/types.md#RLMChatCompletion.execution_time), [`to_dict`](../rlm/core/types.md#RLMChatCompletion.to_dict), [`prompt`](../rlm/core/types.md#RLMChatCompletion.prompt), [`root_model`](../rlm/core/types.md#RLMChatCompletion.root_model), [`from_dict`](../rlm/core/types.md#RLMChatCompletion.from_dict)

### `TestRLMIteration`
- def: [`tests/test_types.py:127`](../../../../../raw/code/rlm/tests/test_types.py#L127)
- doc: Tests for RLMIteration.
- signature: `class TestRLMIteration:`
- members:
  - `test_basic_creation(self)` — [`L130`](../../../../../raw/code/rlm/tests/test_types.py#L130)
  - `test_to_dict(self)` — [`L144`](../../../../../raw/code/rlm/tests/test_types.py#L144)
  - `test_with_final_answer(self)` — [`L135`](../../../../../raw/code/rlm/tests/test_types.py#L135)
- uses (calls/refs, reference-scoped): [`REPLResult`](../rlm/core/types.md#REPLResult), [`RLMIteration`](../rlm/core/types.md#RLMIteration), [`code_blocks`](../rlm/core/types.md#RLMIteration.code_blocks), [`result`](../rlm/core/types.md#CodeBlock.result), [`response`](../rlm/core/types.md#RLMIteration.response), [`CodeBlock`](../rlm/core/types.md#CodeBlock), [`to_dict`](../rlm/core/types.md#RLMIteration.to_dict), [`prompt`](../rlm/core/types.md#RLMIteration.prompt), [`code`](../rlm/core/types.md#CodeBlock.code), [`final_answer`](../rlm/core/types.md#RLMIteration.final_answer), [`iteration_time`](../rlm/core/types.md#RLMIteration.iteration_time)

### `TestRLMMetadata`
- def: [`tests/test_types.py:203`](../../../../../raw/code/rlm/tests/test_types.py#L203)
- doc: Tests for RLMMetadata.
- signature: `class TestRLMMetadata:`
- members:
  - `test_to_dict(self)` — [`L206`](../../../../../raw/code/rlm/tests/test_types.py#L206)
- uses (calls/refs, reference-scoped): [`to_dict`](../rlm/core/types.md#RLMMetadata.to_dict), [`RLMMetadata`](../rlm/core/types.md#RLMMetadata), [`backend`](../rlm/core/types.md#RLMMetadata.backend), [`backend_kwargs`](../rlm/core/types.md#RLMMetadata.backend_kwargs), [`environment_type`](../rlm/core/types.md#RLMMetadata.environment_type), [`max_depth`](../rlm/core/types.md#RLMMetadata.max_depth), [`max_iterations`](../rlm/core/types.md#RLMMetadata.max_iterations), [`environment_kwargs`](../rlm/core/types.md#RLMMetadata.environment_kwargs), [`root_model`](../rlm/core/types.md#RLMMetadata.root_model)

### `TestSerializeValue`
- def: [`tests/test_types.py:16`](../../../../../raw/code/rlm/tests/test_types.py#L16)
- doc: Tests for _serialize_value helper.
- signature: `class TestSerializeValue:`
- members:
  - `my_func()` — [`L35`](../../../../../raw/code/rlm/tests/test_types.py#L35)
  - `test_callable(self)` — [`L34`](../../../../../raw/code/rlm/tests/test_types.py#L34)
  - `test_dict(self)` — [`L30`](../../../../../raw/code/rlm/tests/test_types.py#L30)
  - `test_list(self)` — [`L26`](../../../../../raw/code/rlm/tests/test_types.py#L26)
  - `test_primitives(self)` — [`L19`](../../../../../raw/code/rlm/tests/test_types.py#L19)
- uses (calls/refs, reference-scoped): [`_serialize_value`](../rlm/core/types.md#_serialize_value)

### `TestUsageSummary`
- def: [`tests/test_types.py:67`](../../../../../raw/code/rlm/tests/test_types.py#L67)
- doc: Tests for UsageSummary.
- signature: `class TestUsageSummary:`
- members:
  - `test_from_dict(self)` — [`L78`](../../../../../raw/code/rlm/tests/test_types.py#L78)
  - `test_to_dict(self)` — [`L70`](../../../../../raw/code/rlm/tests/test_types.py#L70)
- uses (calls/refs, reference-scoped): [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`model_usage_summaries`](../rlm/core/types.md#UsageSummary.model_usage_summaries), [`total_calls`](../rlm/core/types.md#ModelUsageSummary.total_calls), [`total_input_tokens`](../rlm/core/types.md#ModelUsageSummary.total_input_tokens), [`total_output_tokens`](../rlm/core/types.md#ModelUsageSummary.total_output_tokens), [`to_dict`](../rlm/core/types.md#UsageSummary.to_dict), [`from_dict`](../rlm/core/types.md#UsageSummary.from_dict)

