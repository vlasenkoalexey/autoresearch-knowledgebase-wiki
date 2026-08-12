---
title: 'Module: utils/agent_infrastructure/vlm_backends.py'
type: catalog
provenance: extracted
module: utils/agent_infrastructure/vlm_backends.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.agent_infrastructure.vlm_backends`/
symbols:
  logger: logger.
  OpenRouterBackend.get_query: OpenRouterBackend#get_query().
  OpenRouterBackend.get_text_query: OpenRouterBackend#get_text_query().
  OpenAIBackend.get_query: OpenAIBackend#get_query().
  AnthropicBackend.get_query: AnthropicBackend#get_query().
  OpenAIBackend.get_text_query: OpenAIBackend#get_text_query().
  AnthropicBackend.get_text_query: AnthropicBackend#get_text_query().
  GeminiBackend.get_query: GeminiBackend#get_query().
  VertexBackend.get_query: VertexBackend#get_query().
  GeminiBackend.get_text_query: GeminiBackend#get_text_query().
  OpenAIBackend._tools_openai: OpenAIBackend#_tools_openai.
  AnthropicBackend._tools_anthropic: AnthropicBackend#_tools_anthropic.
  OpenRouterBackend._tools_openrouter: OpenRouterBackend#_tools_openrouter.
  VLM.get_text_query: VLM#get_text_query().
  VLMBackend: VLMBackend#
  GeminiBackend._setup_function_calling: GeminiBackend#_setup_function_calling().
  ThreadSafeGenerativeModelWrapper._prediction_client: ThreadSafeGenerativeModelWrapper#_prediction_client().
  VLM.BACKENDS: VLM#BACKENDS.
  VLM.backend: VLM#backend.
  VertexBackend._call_generate_content: VertexBackend#_call_generate_content().
  VertexBackend.get_text_query: VertexBackend#get_text_query().
  GeminiBackend._build_model_with_optional_cache: GeminiBackend#_build_model_with_optional_cache().
  VLM.get_query: VLM#get_query().
  OpenRouterBackend.model_name: OpenRouterBackend#model_name.
  VertexBackend.system_instruction: VertexBackend#system_instruction.
  VertexBackend.model: VertexBackend#model.
  GeminiBackend.tools: GeminiBackend#tools.
  VLM: VLM#
  VLMBackend.get_query: VLMBackend#get_query().
  VLMBackend.get_text_query: VLMBackend#get_text_query().
  OpenAIBackend.model_name: OpenAIBackend#model_name.
  OpenAIBackend._call_responses: OpenAIBackend#_call_responses().
  AnthropicBackend._call_messages: AnthropicBackend#_call_messages().
  OpenRouterBackend._call_completion: OpenRouterBackend#_call_completion().
  ThreadSafeGenerativeModelWrapper.generate_content: ThreadSafeGenerativeModelWrapper#generate_content().
  GeminiBackend.model_name: GeminiBackend#model_name.
  GeminiBackend.model: GeminiBackend#model.
  GeminiBackend._call_generate_content: GeminiBackend#_call_generate_content().
  _extract_thinking_from_gemini_like_response: _extract_thinking_from_gemini_like_response().
  AnthropicBackend.model_name: AnthropicBackend#model_name.
  OpenAIBackend._setup_function_calling: OpenAIBackend#_setup_function_calling().
  AnthropicBackend._setup_function_calling: AnthropicBackend#_setup_function_calling().
  OpenRouterBackend._setup_function_calling: OpenRouterBackend#_setup_function_calling().
  _openrouter_response_adapter: _openrouter_response_adapter().
  _openai_tool_call_part: _openai_tool_call_part().
  _openai_text_part: _openai_text_part().
  VLM.system_instruction: VLM#system_instruction.
  OpenAIBackend.tools: OpenAIBackend#tools.
  AnthropicBackend.tools: AnthropicBackend#tools.
  OpenRouterBackend.tools: OpenRouterBackend#tools.
  VertexBackend._tools_vertex: VertexBackend#_tools_vertex.
  GeminiBackend.system_instruction: GeminiBackend#system_instruction.
  _thinking_from_content_parts: _thinking_from_content_parts().
  _openai_responses_adapter: _openai_responses_adapter().
  OpenAIBackend._convert_tools_to_openai_format: OpenAIBackend#_convert_tools_to_openai_format().
  _anthropic_response_adapter: _anthropic_response_adapter().
  AnthropicBackend._convert_tools_to_anthropic_format: AnthropicBackend#_convert_tools_to_anthropic_format().
  OpenRouterBackend.system_instruction: OpenRouterBackend#system_instruction.
  OpenRouterBackend._format_system_message_for_caching: OpenRouterBackend#_format_system_message_for_caching().
  OpenRouterBackend._convert_tools_to_openrouter_format: OpenRouterBackend#_convert_tools_to_openrouter_format().
  VertexBackend._prepare_image: VertexBackend#_prepare_image().
  retry_with_exponential_backoff: retry_with_exponential_backoff().
  _normalize_token_counts: _normalize_token_counts().
  OpenAIBackend.system_instruction: OpenAIBackend#system_instruction.
  OpenAIBackend._build_prompt_cache_key: OpenAIBackend#_build_prompt_cache_key().
  OpenRouterBackend.client: OpenRouterBackend#client.
  OpenRouterBackend._build_prompt_cache_key: OpenRouterBackend#_build_prompt_cache_key().
  VertexBackend.model_name: VertexBackend#model_name.
  VertexBackend._setup_function_calling: VertexBackend#_setup_function_calling().
  GeminiBackend._system_cache_ttl_seconds: GeminiBackend#_system_cache_ttl_seconds.
  ThreadSafeGenerativeModelWrapper._prediction_client_value: ThreadSafeGenerativeModelWrapper#_prediction_client_value.
  GeminiBackend._uses_cached_content_context: GeminiBackend#_uses_cached_content_context.
  VLM.backend_type: VLM#backend_type.
  OpenAIBackend._prompt_cache_key: OpenAIBackend#_prompt_cache_key.
  OpenAIBackend.api_key: OpenAIBackend#api_key.
  OpenAIBackend._extract_thinking_from_response: OpenAIBackend#_extract_thinking_from_response().
  AnthropicBackend.api_key: AnthropicBackend#api_key.
  AnthropicBackend._extract_thinking_from_response: AnthropicBackend#_extract_thinking_from_response().
  OpenRouterBackend._prompt_cache_key: OpenRouterBackend#_prompt_cache_key.
  OpenRouterBackend.api_key: OpenRouterBackend#api_key.
  OpenRouterBackend._extract_thinking_from_response: OpenRouterBackend#_extract_thinking_from_response().
  GeminiBackend.api_key: GeminiBackend#api_key.
  GeminiBackend._extract_thinking_from_response: GeminiBackend#_extract_thinking_from_response().
  AnthropicBackend.system_instruction: AnthropicBackend#system_instruction.
  OpenAIBackend: OpenAIBackend#
  OpenAIBackend.client: OpenAIBackend#client.
  AnthropicBackend: AnthropicBackend#
  AnthropicBackend.client: AnthropicBackend#client.
  OpenRouterBackend: OpenRouterBackend#
  OpenRouterBackend._is_claude_model: OpenRouterBackend#_is_claude_model().
  ThreadSafeGenerativeModelWrapper.heartbeat_logger: ThreadSafeGenerativeModelWrapper#heartbeat_logger().
  VertexBackend: VertexBackend#
  VertexBackend._extract_thinking_from_response: VertexBackend#_extract_thinking_from_response().
  GeminiBackend: GeminiBackend#
  VLM._auto_detect_backend: VLM#_auto_detect_backend().
  _extract_openrouter_cached_tokens: _extract_openrouter_cached_tokens().
  ThreadSafeGenerativeModelWrapper._model: ThreadSafeGenerativeModelWrapper#_model.
  VertexBackend.tools: VertexBackend#tools.
  FunctionCallPart.args: FunctionCallPart#args.
  OpenAIBackend.errors: OpenAIBackend#errors.
  AnthropicBackend.errors: AnthropicBackend#errors.
  ThreadSafeGenerativeModelWrapper.__getattr__: ThreadSafeGenerativeModelWrapper#__getattr__().
  OpenAIBackend._prepare_image_base64: OpenAIBackend#_prepare_image_base64().
  AnthropicBackend._prepare_image_base64: AnthropicBackend#_prepare_image_base64().
  _anthropic_error_message: _anthropic_error_message().
  _openrouter_error_message: _openrouter_error_message().
  _extract_openrouter_cache_write_tokens: _extract_openrouter_cache_write_tokens().
  OpenRouterBackend._prepare_image_base64: OpenRouterBackend#_prepare_image_base64().
  ThreadSafeGenerativeModelWrapper._access_count: ThreadSafeGenerativeModelWrapper#_access_count.
  ThreadSafeGenerativeModelWrapper._init_time: ThreadSafeGenerativeModelWrapper#_init_time.
  VertexBackend._extract_text_from_response: VertexBackend#_extract_text_from_response().
  GeminiBackend._prepare_image: GeminiBackend#_prepare_image().
  GeminiBackend._extract_text_from_response: GeminiBackend#_extract_text_from_response().
  VLM.model_name: VLM#model_name.
  retry_with_exponential_backoff.wrapper: retry_with_exponential_backoff().wrapper().
  _openai_tool_call_part.FunctionCallPart: _openai_tool_call_part().FunctionCallPart#
  _format_function_call_for_thinking: _format_function_call_for_thinking().
  OpenAIBackend._build_json_schema_properties: OpenAIBackend#_build_json_schema_properties().
  AnthropicBackend._build_input_schema: AnthropicBackend#_build_input_schema().
  AnthropicBackend._format_system_for_caching: AnthropicBackend#_format_system_for_caching().
  OpenRouterBackend._build_json_schema_properties: OpenRouterBackend#_build_json_schema_properties().
  ThreadSafeGenerativeModelWrapper: ThreadSafeGenerativeModelWrapper#
  ThreadSafeGenerativeModelWrapper._prediction_client_lock: ThreadSafeGenerativeModelWrapper#_prediction_client_lock.
  VertexBackend._convert_parameters_format: VertexBackend#_convert_parameters_format().
  GeminiBackend.genai: GeminiBackend#genai.
  VLM.tools: VLM#tools.
  _openai_tool_call_part.FunctionCallPart.__init__: _openai_tool_call_part().FunctionCallPart#__init__().
  FunctionCallPart.name: FunctionCallPart#name.
  OpenAIBackend.__init__: OpenAIBackend#__init__().
  AnthropicBackend.__init__: AnthropicBackend#__init__().
  OpenRouterBackend.__init__: OpenRouterBackend#__init__().
  ThreadSafeGenerativeModelWrapper.__init__: ThreadSafeGenerativeModelWrapper#__init__().
  VertexBackend.__init__: VertexBackend#__init__().
  GeminiBackend.__init__: GeminiBackend#__init__().
  VLM.__init__: VLM#__init__().
---
# Module: [`utils/agent_infrastructure/vlm_backends.py`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py)

## Classes
### `AnthropicBackend`  ·  implements/extends VLMBackend
- def: [`utils/agent_infrastructure/vlm_backends.py:608`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L608)
- doc: Anthropic Messages API backend with tool calling and system prompt.
- signature: `class AnthropicBackend(VLMBackend):`
- members:
  - `_build_input_schema(self, params: dict)` — [`L647`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L647) — Build JSON Schema properties from Gemini-style params. Returns (properties, required).
  - `_call_messages(self, system: Optional[str], messages: list, tools: Optional[list] = None)` — [`L701`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L701) — Call Anthropic Messages API with caching enabled for system prompt.
  - `_convert_tools_to_anthropic_format(self)` — [`L670`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L670) — Convert Gemini-style tool declarations to Anthropic input_schema format.
  - `_extract_thinking_from_response(self, response)` — [`L729`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L729) — Extract reasoning for logging from adapter (all parts, including parallel tool calls).
  - `_format_system_for_caching(self, system: Optional[str])` — [`L683`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L683) — Format system prompt with cache_control for Anthropic API.
  - `_prepare_image_base64(self, img: Union[Image.Image, np.ndarray])` — [`L717`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L717) — Prepare image as base64 string.
  - `_setup_function_calling(self)` — [`L642`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L642) — Update tools when agent dynamically updates tool list.
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L733`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L733) — Process image(s) and text. Returns adapter if tools, else string.
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L820`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L820) — Process text-only prompt. Returns adapter if tools, else string.
  - `api_key` — [`L624`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L624)
  - `client` — [`L629`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L629)
  - `errors` — [`L630`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L630)
  - `model_name` — [`L621`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L621)
  - `system_instruction` — [`L623`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L623)
  - `tools` — [`L622`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L622)
- protocol/private: `__init__`[`L615`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L615), `_tools_anthropic`[`L633`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L633)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`log_llm_interaction`](../data_persistence/llm_logger.md#log_llm_interaction), [`VLMBackend`](vlm_backends.md#VLMBackend), [`log_llm_error`](../data_persistence/llm_logger.md#log_llm_error), [`_extract_thinking_from_gemini_like_response`](vlm_backends.md#_extract_thinking_from_gemini_like_response), [`_anthropic_response_adapter`](vlm_backends.md#_anthropic_response_adapter), [`retry_with_exponential_backoff`](vlm_backends.md#retry_with_exponential_backoff), [`_anthropic_error_message`](vlm_backends.md#_anthropic_error_message)
- used by: [`VLMBackend`](vlm_backends.md#VLMBackend), [`BACKENDS`](vlm_backends.md#VLM.BACKENDS), [`get_query`](vlm_backends.md#VLMBackend.get_query), [`get_text_query`](vlm_backends.md#VLMBackend.get_text_query)

### `FunctionCallPart`
- def: [`utils/agent_infrastructure/vlm_backends.py:76`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L76)
- signature: `class FunctionCallPart:`
- members:
  - `args` — [`L79`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L79)
  - `name` — [`L78`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L78)
- protocol/private: `__init__`[`L77`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L77)

### `GeminiBackend`  ·  implements/extends VLMBackend
- def: [`utils/agent_infrastructure/vlm_backends.py:2112`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2112)
- doc: Google Gemini API backend
- signature: `class GeminiBackend(VLMBackend):`
- members:
  - `_build_model_with_optional_cache(self, genai, model_name: str, model_kwargs: Dict[str, Any])` — [`L2166`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2166) — Build Gemini model and explicitly cache static system instruction when supported.
  - `_call_generate_content(self, content_parts)` — [`L2249`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2249) — Calls the generate_content method with exponential backoff for rate limits.
  - `_extract_text_from_response(self, response)` — [`L2222`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2222) — Extract text from Gemini response, handling multiple parts
  - `_extract_thinking_from_response(self, response)` — [`L2245`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2245) — Extract thinking for logging (all parts; multiple tool calls in one turn).
  - `_prepare_image(self, img: Union[Image.Image, np.ndarray])` — [`L2203`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2203) — Prepare image for Gemini API - upscale to 4x resolution (HD)
  - `_setup_function_calling(self)` — [`L2155`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2155) — Update the model with current tools
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L2320`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2320) — Process an image (or list of images) and text prompt using Gemini API
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L2458`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2458) — Process a text-only prompt using Gemini API
  - `api_key` — [`L2125`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2125)
  - `genai` — [`L2153`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2153)
  - `model` — [`L2143`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2143)
  - `model_name` — [`L2121`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2121)
  - `system_instruction` — [`L2123`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2123)
  - `tools` — [`L2122`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2122)
- protocol/private: `__init__`[`L2115`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2115), `_system_cache_ttl_seconds`[`L2136`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2136), `_uses_cached_content_context`[`L2124`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2124)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`log_llm_interaction`](../data_persistence/llm_logger.md#log_llm_interaction), [`VLMBackend`](vlm_backends.md#VLMBackend), [`_extract_thinking_from_gemini_like_response`](vlm_backends.md#_extract_thinking_from_gemini_like_response), [`_normalize_token_counts`](vlm_backends.md#_normalize_token_counts)
- used by: [`VLMBackend`](vlm_backends.md#VLMBackend), [`BACKENDS`](vlm_backends.md#VLM.BACKENDS), [`get_query`](vlm_backends.md#VLMBackend.get_query), [`get_text_query`](vlm_backends.md#VLMBackend.get_text_query)

### `OpenAIBackend`  ·  implements/extends VLMBackend
- def: [`utils/agent_infrastructure/vlm_backends.py:228`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L228)
- doc: OpenAI API backend with tool calling and system instructions.
- signature: `class OpenAIBackend(VLMBackend):`
- members:
  - `_build_json_schema_properties(self, params: dict)` — [`L296`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L296) — Build JSON Schema properties from Gemini-style params. Returns (properties, required).
  - `_build_prompt_cache_key(self)` — [`L269`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L269) — Build stable cache key for static system instruction.
  - `_call_responses(self, instructions: str | None, input_data, tools: list = None)` — [`L320`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L320) — Calls the Responses API (v1/responses) with optional tools.
  - `_convert_tools_to_openai_format(self)` — [`L277`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L277) — Convert Gemini-style tool declarations to OpenAI format.
  - `_extract_thinking_from_response(self, response)` — [`L352`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L352) — Extract reasoning for logging from response/adapter (all parts, including parallel tool calls).
  - `_prepare_image_base64(self, img: Union[Image.Image, np.ndarray])` — [`L339`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L339) — Prepare image as base64 string
  - `_setup_function_calling(self)` — [`L264`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L264) — Update tools (called when agent dynamically updates tool list).
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L356`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L356) — Process an image (or list of images) and text prompt using OpenAI API.
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L465`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L465) — Process a text-only prompt using OpenAI API.
  - `api_key` — [`L246`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L246)
  - `client` — [`L251`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L251)
  - `errors` — [`L252`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L252)
  - `model_name` — [`L242`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L242)
  - `system_instruction` — [`L244`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L244)
  - `tools` — [`L243`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L243)
- protocol/private: `__init__`[`L235`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L235), `_prompt_cache_key`[`L245`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L245), `_tools_openai`[`L255`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L255)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`log_llm_interaction`](../data_persistence/llm_logger.md#log_llm_interaction), [`VLMBackend`](vlm_backends.md#VLMBackend), [`log_llm_error`](../data_persistence/llm_logger.md#log_llm_error), [`_extract_thinking_from_gemini_like_response`](vlm_backends.md#_extract_thinking_from_gemini_like_response), [`_openai_responses_adapter`](vlm_backends.md#_openai_responses_adapter), [`retry_with_exponential_backoff`](vlm_backends.md#retry_with_exponential_backoff), [`_normalize_token_counts`](vlm_backends.md#_normalize_token_counts)
- used by: [`VLMBackend`](vlm_backends.md#VLMBackend), [`BACKENDS`](vlm_backends.md#VLM.BACKENDS), [`get_query`](vlm_backends.md#VLMBackend.get_query), [`get_text_query`](vlm_backends.md#VLMBackend.get_text_query)

### `OpenRouterBackend`  ·  implements/extends VLMBackend
- def: [`utils/agent_infrastructure/vlm_backends.py:1029`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1029)
- doc: OpenRouter API backend with tool calling and system instructions.
- signature: `class OpenRouterBackend(VLMBackend):`
- members:
  - `_build_json_schema_properties(self, params: dict)` — [`L1109`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1109) — Build JSON Schema properties from Gemini-style params. Returns (properties, required).
  - `_build_prompt_cache_key(self)` — [`L1071`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1071) — Build stable cache key for static system instruction.
  - `_call_completion(self, messages, tools=None)` — [`L1165`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1165) — Calls chat.completions with optional tools and system message.
  - `_convert_tools_to_openrouter_format(self)` — [`L1132`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1132) — Convert Gemini-style tool declarations to OpenAI Chat Completions format (nested function).
  - `_extract_thinking_from_response(self, response)` — [`L1160`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1160) — Extract reasoning for logging from adapter (all parts, including parallel tool calls).
  - `_format_system_message_for_caching(self)` — [`L1084`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1084) — Format system message with cache_control for Claude models.
  - `_is_claude_model(self)` — [`L1079`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1079) — Check if the model is an Anthropic Claude model (requires explicit cache_control).
  - `_prepare_image_base64(self, img: Union[Image.Image, np.ndarray])` — [`L1148`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1148) — Prepare image as base64 string.
  - `_setup_function_calling(self)` — [`L1066`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1066) — Update tools when agent dynamically updates tool list.
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L1175`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1175) — Process image(s) and text. Returns adapter if tools, else string.
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L1288`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1288) — Process text-only prompt. Returns adapter if tools, else string.
  - `api_key` — [`L1046`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1046)
  - `client` — [`L1051`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1051)
  - `model_name` — [`L1042`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1042)
  - `system_instruction` — [`L1044`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1044)
  - `tools` — [`L1043`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1043)
- protocol/private: `__init__`[`L1036`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1036), `_prompt_cache_key`[`L1045`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1045), `_tools_openrouter`[`L1057`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1057)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`log_llm_interaction`](../data_persistence/llm_logger.md#log_llm_interaction), [`VLMBackend`](vlm_backends.md#VLMBackend), [`log_llm_error`](../data_persistence/llm_logger.md#log_llm_error), [`_extract_thinking_from_gemini_like_response`](vlm_backends.md#_extract_thinking_from_gemini_like_response), [`_openrouter_response_adapter`](vlm_backends.md#_openrouter_response_adapter), [`retry_with_exponential_backoff`](vlm_backends.md#retry_with_exponential_backoff), [`_normalize_token_counts`](vlm_backends.md#_normalize_token_counts), [`_extract_openrouter_cached_tokens`](vlm_backends.md#_extract_openrouter_cached_tokens), [`_extract_openrouter_cache_write_tokens`](vlm_backends.md#_extract_openrouter_cache_write_tokens), [`_openrouter_error_message`](vlm_backends.md#_openrouter_error_message)
- used by: [`VLMBackend`](vlm_backends.md#VLMBackend), [`BACKENDS`](vlm_backends.md#VLM.BACKENDS), [`get_query`](vlm_backends.md#VLMBackend.get_query), [`get_text_query`](vlm_backends.md#VLMBackend.get_text_query)

### `ThreadSafeGenerativeModelWrapper`
- def: [`utils/agent_infrastructure/vlm_backends.py:1383`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1383)
- doc: Thread-safe wrapper for GenerativeModel that protects _prediction_client access.
- signature: `class ThreadSafeGenerativeModelWrapper:`
- members:
  - `__getattr__(self, name)` — [`L1453`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1453) — Delegate all other attributes to the wrapped model
  - `_prediction_client(self)` — [`L1406`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1406) — Thread-safe access to _prediction_client using double-check locking pattern
  - `generate_content(self, *args, **kwargs)` — [`L1457`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1457) — Delegate generate_content calls to wrapped model with detailed logging
  - `heartbeat_logger()` — [`L1486`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1486) — Background thread to log heartbeats during long-running calls
- protocol/private: `__init__`[`L1399`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1399), `_access_count`[`L1402`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1402), `_init_time`[`L1403`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1403), `_model`[`L1400`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1400), `_prediction_client_lock`[`L1397`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1397), `_prediction_client_value`[`L1401`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1401)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger)
- used by: [`_call_generate_content`](vlm_backends.md#VertexBackend._call_generate_content), [`model`](vlm_backends.md#VertexBackend.model)

### `VLM`
- def: [`utils/agent_infrastructure/vlm_backends.py:2567`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2567)
- doc: Main VLM class that supports multiple backends
- signature: `class VLM:`
- members:
  - `__init__(self, model_name: str, backend: str = "openai", port: int = 8010, tools: list = None, system_instruction: str = None, **kwargs)` — [`L2578`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2578) — Initialize VLM with specified backend
  - `_auto_detect_backend(self, model_name: str)` — [`L2618`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2618) — Auto-detect backend based on model name
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L2633`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2633) — Process an image (or list of images) and text prompt
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L2660`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2660) — Process a text-only prompt
  - `BACKENDS` — [`L2570`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2570)
  - `backend` — [`L2612`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2612)
  - `backend_type` — [`L2599`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2599)
  - `model_name` — [`L2598`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2598)
  - `system_instruction` — [`L2601`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2601)
  - `tools` — [`L2600`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2600)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`log_llm_error`](../data_persistence/llm_logger.md#log_llm_error), [`AnthropicBackend`](vlm_backends.md#AnthropicBackend), [`GeminiBackend`](vlm_backends.md#GeminiBackend), [`OpenAIBackend`](vlm_backends.md#OpenAIBackend), [`OpenRouterBackend`](vlm_backends.md#OpenRouterBackend), [`VertexBackend`](vlm_backends.md#VertexBackend)
- used by: [`_run_planner_loop`](../../agents/PokeAgent.md#PokeAgent._run_planner_loop), [`_run_battler_loop`](../../agents/PokeAgent.md#PokeAgent._run_battler_loop), [`_evolve_subagents`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_subagents), [`_evolve_skills`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_skills), [`_get_subagent_vlm`](../../agents/PokeAgent.md#PokeAgent._get_subagent_vlm), [`_evolve_memory`](../../agents/utils/harness_evolver.md#HarnessEvolver._evolve_memory), [`optimize_prompt`](../../agents/utils/prompt_optimizer.md#PromptOptimizer.optimize_prompt), [`_run_one_step_subagent`](../../agents/PokeAgent.md#PokeAgent._run_one_step_subagent), [`vlm`](../../agents/PokeAgent.md#PokeAgent.vlm), [`vlm`](../../agents/vision_only_agent.md#VisionOnlyAgent.vlm), [`system_prompt_content`](../../agents/utils/prompt_optimizer.md#PromptOptimizer.system_prompt_content), [`_run_local_subagent`](../../agents/vision_only_agent.md#VisionOnlyAgent._run_local_subagent), [`_local_subagent_vlm`](../../agents/vision_only_agent.md#VisionOnlyAgent._local_subagent_vlm), [`_preprocess_bootstrap_prompt`](../stores/bootstrap.md#_preprocess_bootstrap_prompt), [`call_vlm_with_image`](../../agents/PokeAgent.md#PokeAgent.call_vlm_with_image), [`call_vlm_with_image`](../../agents/vision_only_agent.md#VisionOnlyAgent.call_vlm_with_image), [`call_vlm_with_text`](../../agents/PokeAgent.md#PokeAgent.call_vlm_with_text), [`call_vlm_with_text`](../../agents/vision_only_agent.md#VisionOnlyAgent.call_vlm_with_text), [`vlm`](../../agents/utils/prompt_optimizer.md#PromptOptimizer.vlm)  (1 test-only)

### `VLMBackend`  ·  implements/extends ABC
- def: [`utils/agent_infrastructure/vlm_backends.py:54`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L54)
- doc: Abstract base class for VLM backends
- signature: `class VLMBackend(ABC):`
- members:
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L58`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L58) — Process an image (or list of images) and text prompt
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L68`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L68) — Process a text-only prompt
- uses (calls/refs, reference-scoped): [`get_query`](vlm_backends.md#OpenRouterBackend.get_query), [`get_text_query`](vlm_backends.md#OpenRouterBackend.get_text_query), [`get_query`](vlm_backends.md#AnthropicBackend.get_query), [`get_query`](vlm_backends.md#OpenAIBackend.get_query), [`get_text_query`](vlm_backends.md#AnthropicBackend.get_text_query), [`get_text_query`](vlm_backends.md#OpenAIBackend.get_text_query), [`get_query`](vlm_backends.md#GeminiBackend.get_query), [`get_query`](vlm_backends.md#VertexBackend.get_query), [`get_text_query`](vlm_backends.md#GeminiBackend.get_text_query), [`get_text_query`](vlm_backends.md#VertexBackend.get_text_query), [`AnthropicBackend`](vlm_backends.md#AnthropicBackend), [`GeminiBackend`](vlm_backends.md#GeminiBackend), [`OpenAIBackend`](vlm_backends.md#OpenAIBackend), [`OpenRouterBackend`](vlm_backends.md#OpenRouterBackend), [`VertexBackend`](vlm_backends.md#VertexBackend)
- used by: [`AnthropicBackend`](vlm_backends.md#AnthropicBackend), [`GeminiBackend`](vlm_backends.md#GeminiBackend), [`OpenAIBackend`](vlm_backends.md#OpenAIBackend), [`OpenRouterBackend`](vlm_backends.md#OpenRouterBackend), [`VertexBackend`](vlm_backends.md#VertexBackend)

### `VertexBackend`  ·  implements/extends VLMBackend
- def: [`utils/agent_infrastructure/vlm_backends.py:1596`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1596)
- doc: Google Gemini API with Vertex backend using vertexai.generative_models
- signature: `class VertexBackend(VLMBackend):`
- members:
  - `_call_generate_content(self, content_parts)` — [`L1771`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1771) — Calls the generate_content method using the VertexAI SDK pattern.
  - `_convert_parameters_format(self, gemini_params)` — [`L1678`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1678) — Convert Gemini tool parameters to VertexAI format
  - `_extract_text_from_response(self, response)` — [`L1747`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1747) — Extract text from VertexAI response, handling multiple parts
  - `_extract_thinking_from_response(self, response)` — [`L1743`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1743) — Extract thinking for logging (all parts; multiple tool calls in one turn).
  - `_prepare_image(self, img: Union[Image.Image, np.ndarray])` — [`L1712`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1712) — Prepare image for Gemini API - upscale to 4x resolution (HD)
  - `_setup_function_calling(self)` — [`L1652`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1652) — Setup function calling for VertexAI using FunctionDeclaration and Tool objects
  - `get_query(self, img: Union[Image.Image, np.ndarray, List[Union[Image.Image, np.ndarray]]], text: str, module_name: str = "Unknown")` — [`L1905`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1905) — Process an image (or list of images) and text prompt using VertexAI
  - `get_text_query(self, text: str, module_name: str = "Unknown")` — [`L2034`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L2034) — Process a text-only prompt using VertexAI
  - `model` — [`L1639`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1639)
  - `model_name` — [`L1616`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1616)
  - `system_instruction` — [`L1618`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1618)
  - `tools` — [`L1617`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1617)
- protocol/private: `__init__`[`L1609`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1609), `_tools_vertex`[`L1670`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L1670)
- uses (calls/refs, reference-scoped): [`logger`](vlm_backends.md#logger), [`get_cache_directory`](../data_persistence/run_data_manager.md#get_cache_directory), [`log_llm_interaction`](../data_persistence/llm_logger.md#log_llm_interaction), [`VLMBackend`](vlm_backends.md#VLMBackend), [`_prediction_client`](vlm_backends.md#ThreadSafeGenerativeModelWrapper._prediction_client), [`generate_content`](vlm_backends.md#ThreadSafeGenerativeModelWrapper.generate_content), [`_extract_thinking_from_gemini_like_response`](vlm_backends.md#_extract_thinking_from_gemini_like_response), [`retry_with_exponential_backoff`](vlm_backends.md#retry_with_exponential_backoff), [`ThreadSafeGenerativeModelWrapper`](vlm_backends.md#ThreadSafeGenerativeModelWrapper)
- used by: [`VLMBackend`](vlm_backends.md#VLMBackend), [`BACKENDS`](vlm_backends.md#VLM.BACKENDS), [`get_query`](vlm_backends.md#VLMBackend.get_query), [`get_text_query`](vlm_backends.md#VLMBackend.get_text_query)

## Functions
- `_anthropic_error_message(exc: Exception)` — [`L891`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L891) — Build a detailed error message from an Anthropic API exception (including 400 body).
- `_anthropic_response_adapter(response)` — [`L558`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L558) — Adapt Anthropic Messages API output to Gemini-like structure for agents.
- `_extract_openrouter_cache_write_tokens(usage)` — [`L964`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L964) — Extract cache_write_tokens from OpenRouter usage.prompt_tokens_details.
- `_extract_openrouter_cached_tokens(usage)` — [`L947`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L947) — Extract cached_tokens from OpenRouter usage.prompt_tokens_details.
- `_extract_thinking_from_gemini_like_response(response)` — [`L140`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L140) — Shared extractor for adapters/responses with candidates[0].content.parts.
- `_format_function_call_for_thinking(function_call)` — [`L95`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L95) — One-line summary of a single function_call for agent-thinking / JSONL logging.
- `_normalize_token_counts(prompt_tokens: int, completion_tokens: int, total_tokens: int)` — [`L151`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L151) — Normalize provider token counters to a consistent billing shape.
- `_openai_responses_adapter(response)` — [`L170`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L170) — Adapt OpenAI Responses API output to Gemini-like structure for agents.
- `_openai_text_part(text: str)` — [`L87`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L87) — Create a Gemini-compatible text part for agent consumption.
- `_openai_tool_call_part(name: str, args: Dict[str, Any])` — [`L73`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L73) — Create a Gemini-compatible part object for agent consumption.
- `_openrouter_error_message(exc: Exception)` — [`L920`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L920) — Build a detailed error message from OpenRouter/OpenAI API exception (including 400 body).
- `_openrouter_response_adapter(response)` — [`L977`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L977) — Adapt OpenRouter/OpenAI Chat Completions response to Gemini-like structure for agents.
- `_thinking_from_content_parts(parts)` — [`L119`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L119) — Aggregate every text and function_call part (parallel tool calls in one model turn).
- `retry_with_exponential_backoff(func, initial_delay: float = 1, exponential_base: float = 2, jitter: bool = True, max_retries: int = 10, errors: tuple = (Exception,))` — [`L25`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L25) — Retry a function with exponential backoff.
- `wrapper(*args, **kwargs)` — [`L35`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L35)

## Module values
- `logger` — [`L18`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/vlm_backends.py#L18)

