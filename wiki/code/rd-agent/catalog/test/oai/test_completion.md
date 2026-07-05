---
title: 'Module: test/oai/test_completion.py'
type: catalog
provenance: extracted
module: test/oai/test_completion.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.oai.test_completion`/Test
symbols:
  TestChatCompletion.test_response_format_with_basemodel: ChatCompletion#test_response_format_with_basemodel().
  TestChatCompletion.test_chat_completion: ChatCompletion#test_chat_completion().
  TestChatCompletion.test_chat_completion_json_mode: ChatCompletion#test_chat_completion_json_mode().
  TestChatCompletion.test_build_messages_and_calculate_token: ChatCompletion#test_build_messages_and_calculate_token().
  TestChatCompletion.test_json_mode_with_specific_target_type: ChatCompletion#test_json_mode_with_specific_target_type().
  TestPersonModel: PersonModel#
  TestPersonModel.name: PersonModel#name.
  TestPersonModel.age: PersonModel#age.
  TestPersonModel.skills: PersonModel#skills.
  TestChatCompletion: ChatCompletion#
---
# Module: [`test/oai/test_completion.py`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py)

## Classes
### `TestChatCompletion`  ·  implements/extends TestCase
- def: [`test/oai/test_completion.py:18`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L18)
- signature: `class TestChatCompletion(unittest.TestCase):`
- members:
  - `test_build_messages_and_calculate_token(self)` — [`L41`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L41)
  - `test_chat_completion(self)` — [`L19`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L19)
  - `test_chat_completion_json_mode(self)` — [`L29`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L29)
  - `test_json_mode_with_specific_target_type(self)` — [`L48`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L48) — Test json_mode=True with specific json_target_type
  - `test_response_format_with_basemodel(self)` — [`L68`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L68) — Test response_format with BaseModel (if supported)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../rdagent/oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../rdagent/oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`build_messages_and_calculate_token`](../../rdagent/oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`supports_response_schema`](../../rdagent/oai/backend/base.md#APIBackend.supports_response_schema)  (1 test-only)

### `TestPersonModel`  ·  implements/extends BaseModel
- def: [`test/oai/test_completion.py:10`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L10)
- doc: This is a test Pydantic model
- signature: `class TestPersonModel(BaseModel):`
- members:
  - `age` — [`L14`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L14)
  - `name` — [`L13`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L13)
  - `skills` — [`L15`](../../../../../../raw/code/rd-agent/test/oai/test_completion.py#L15)
- used by: (1 test-only callers)

