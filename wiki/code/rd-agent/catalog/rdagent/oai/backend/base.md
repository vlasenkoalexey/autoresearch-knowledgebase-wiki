---
title: 'Module: rdagent/oai/backend/base.py'
type: catalog
provenance: extracted
module: rdagent/oai/backend/base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.oai.backend.base`/
symbols:
  APIBackend.build_messages_and_create_chat_completion: APIBackend#build_messages_and_create_chat_completion().
  APIBackend._create_chat_completion_auto_continue: APIBackend#_create_chat_completion_auto_continue().
  APIBackend._try_create_chat_completion_or_embedding: APIBackend#_try_create_chat_completion_or_embedding().
  ChatSession.build_chat_completion: ChatSession#build_chat_completion().
  APIBackend.chat_token_limit: APIBackend#chat_token_limit().
  SQliteLazyCache.c: SQliteLazyCache#c.
  ChatSession.build_chat_completion_message: ChatSession#build_chat_completion_message().
  APIBackend.use_embedding_cache: APIBackend#use_embedding_cache.
  APIBackend.build_messages_and_calculate_token: APIBackend#build_messages_and_calculate_token().
  APIBackend.build_chat_session: APIBackend#build_chat_session().
  APIBackend._create_embedding_with_cache: APIBackend#_create_embedding_with_cache().
  APIBackend._build_log_messages: APIBackend#_build_log_messages().
  APIBackend.create_embedding: APIBackend#create_embedding().
  APIBackend: APIBackend#
  APIBackend._build_messages: APIBackend#_build_messages().
  JSONParser.strategies: JSONParser#strategies.
  CodeBlockParser.parse: CodeBlockParser#parse().
  SessionChatHistoryCache.cache: SessionChatHistoryCache#cache.
  APIBackend.cache: APIBackend#cache.
  SQliteLazyCache.chat_set: SQliteLazyCache#chat_set().
  SQliteLazyCache.embedding_set: SQliteLazyCache#embedding_set().
  APIBackend.supports_response_schema: APIBackend#supports_response_schema().
  ChatSession.system_prompt: ChatSession#system_prompt.
  APIBackend.dump_chat_cache: APIBackend#dump_chat_cache.
  APIBackend.use_chat_cache: APIBackend#use_chat_cache.
  APIBackend.dump_embedding_cache: APIBackend#dump_embedding_cache.
  openai_imported: openai_imported.
  JSONParser._direct_parse: JSONParser#_direct_parse().
  JSONParser.parse: JSONParser#parse().
  JSONParser._fix_python_syntax: JSONParser#_fix_python_syntax().
  JSONParser._extract_with_fix_combined: JSONParser#_extract_with_fix_combined().
  CodeBlockParser._lang_aliases: CodeBlockParser#_lang_aliases.
  SQliteLazyCache.chat_get: SQliteLazyCache#chat_get().
  SQliteLazyCache.embedding_get: SQliteLazyCache#embedding_get().
  SQliteLazyCache.message_set: SQliteLazyCache#message_set().
  SessionChatHistoryCache.message_get: SessionChatHistoryCache#message_get().
  SessionChatHistoryCache.message_set: SessionChatHistoryCache#message_set().
  APIBackend.cache_file_location: APIBackend#cache_file_location.
  APIBackend.retry_wait_seconds: APIBackend#retry_wait_seconds.
  APIBackend._add_json_in_prompt: APIBackend#_add_json_in_prompt().
  APIBackend._calculate_token_from_messages: APIBackend#_calculate_token_from_messages().
  APIBackend._create_embedding_inner_function: APIBackend#_create_embedding_inner_function().
  APIBackend._create_chat_completion_inner_function: APIBackend#_create_chat_completion_inner_function().
  SQliteLazyCache.conn: SQliteLazyCache#conn.
  ChatSession.build_chat_completion_message_and_calculate_token: ChatSession#build_chat_completion_message_and_calculate_token().
  SQliteLazyCache: SQliteLazyCache#
  SessionChatHistoryCache: SessionChatHistoryCache#
  ChatSession.conversation_id: ChatSession#conversation_id.
  JSONParser._extract_from_code_block: JSONParser#_extract_from_code_block().
  CodeBlockParser._get_language_aliases: CodeBlockParser#_get_language_aliases().
  SQliteLazyCache.message_get: SQliteLazyCache#message_get().
  ChatSession.get_conversation_id: ChatSession#get_conversation_id().
  CodeBlockParser.language: CodeBlockParser#language.
  JSONParser._fix_python_booleans: JSONParser#_fix_python_booleans().
  ChatSession: ChatSession#
  ChatSession.api_backend: ChatSession#api_backend.
  APIBackend.__init__: APIBackend#__init__().
  JSONParser: JSONParser#
  JSONParser.add_json_in_prompt: JSONParser#add_json_in_prompt.
  JSONParser._extract_first_json: JSONParser#_extract_first_json().
  CodeBlockParser: CodeBlockParser#
  CodeBlockParser.SUPPORTED_LANGUAGES: CodeBlockParser#SUPPORTED_LANGUAGES.
  CodeBlockParser.fallback_to_raw: CodeBlockParser#fallback_to_raw.
  JSONParser.__init__: JSONParser#__init__().
  CodeBlockParser.__init__: CodeBlockParser#__init__().
  SQliteLazyCache.__init__: SQliteLazyCache#__init__().
  SQliteLazyCache.cache_location: SQliteLazyCache#cache_location.
  SessionChatHistoryCache.__init__: SessionChatHistoryCache#__init__().
  ChatSession.__init__: ChatSession#__init__().
  ChatSession.display_history: ChatSession#display_history().
---
# Module: [`rdagent/oai/backend/base.py`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py)

## Classes
### `APIBackend`  ·  implements/extends ABC
- def: [`rdagent/oai/backend/base.py:353`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L353)
- doc: Abstract base class for LLM API backends
- signature: `class APIBackend(ABC):`
- members:
  - `_add_json_in_prompt(self, messages: list[dict[str, Any]])` — [`L615`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L615) — add json related content in the prompt if add_json_in_prompt is True
  - `_build_messages(self, user_prompt: str, system_prompt: str | None = None, former_messages: list[dict[str, Any]] | None = None, *, shrink_multiple_break: bool = False)` — [`L392`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L392) — build the messages to avoid implementing several redundant lines of code — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `_calculate_token_from_messages(self, messages: list[dict[str, Any]])` — [`L764`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L764) — Calculate the token count from messages
  - `_create_chat_completion_auto_continue(self, messages: list[dict[str, Any]], json_mode: bool = False, chat_cache_prefix: str = "", seed: Optional[int] = None, json_target_type: Optional[str] = None, add_json_in_prompt: bool = False, response_format: Optional[Union[dict, Type[BaseModel]]] = None, code_block_language: Optional[str] = None, code_block_fallback: bool = False, **kwargs: Any)` — [`L625`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L625) — Call the chat completion function and automatically continue the conversation if the finish_reason is length. — documented in [rdagent-log](../../../../concepts/rdagent-log.md)
  - `_create_chat_completion_inner_function(self, messages: list[dict[str, Any]], response_format: Optional[Union[dict, Type[BaseModel]]] = None, *args, **kwargs)` — [`L778`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L778) — Call the chat completion function
  - `_create_embedding_inner_function(self, input_content_list: list[str])` — [`L771`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L771) — Call the embedding function
  - `_try_create_chat_completion_or_embedding(self, max_retry: int = 10, chat_completion: bool = False, embedding: bool = False, *args, **kwargs)` — [`L520`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L520) — This function to share operation between embedding and chat completion — documented in [rdagent-log-timer](../../../../concepts/rdagent-log-timer.md)
  - `build_chat_session(self, conversation_id: str | None = None, session_system_prompt: str | None = None)` — [`L381`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L381) — conversation_id is a 256-bit string created by uuid.uuid4() and is also — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `build_messages_and_calculate_token(self, user_prompt: str, system_prompt: str | None, former_messages: list[dict[str, Any]] | None = None, *, shrink_multiple_break: bool = False)` — [`L505`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L505)
  - `build_messages_and_create_chat_completion(self, user_prompt: str, system_prompt: str | None = None, former_messages: list | None = None, chat_cache_prefix: str = "", shrink_multiple_break: bool = False, *args, **kwargs)` — [`L440`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L440) — Responseible for building messages and logging messages — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `chat_token_limit(self)` — [`L791`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L791) — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `create_embedding(self, input_content: str | list[str], *args, **kwargs)` — [`L493`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L493)
  - `supports_response_schema(self)` — [`L757`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L757) — Check if the backend supports function calling
  - `cache` — [`L377`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L377)
  - `cache_file_location` — [`L376`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L376)
  - `dump_chat_cache` — [`L367`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L367)
  - `dump_embedding_cache` — [`L369`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L369)
  - `retry_wait_seconds` — [`L379`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L379)
  - `use_chat_cache` — [`L368`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L368) — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `use_embedding_cache` — [`L372`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L372)
- protocol/private: `__init__`[`L360`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L360), `_build_log_messages`[`L429`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L429), `_create_embedding_with_cache`[`L733`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L733)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`LLM_SETTINGS`](../llm_conf.md#LLM_SETTINGS), [`warning`](../../log/logger.md#RDAgentLog.warning), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`_create_chat_completion_inner_function`](deprec.md#DeprecBackend._create_chat_completion_inner_function), [`LogColors`](../../log/utils/__init__.md#LogColors), [`_create_chat_completion_inner_function`](litellm.md#LiteLLMAPIBackend._create_chat_completion_inner_function), [`RD_Agent_TIMER_wrapper`](../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`timer`](../../log/timer.md#RDAgentTimerWrapper.timer), [`END`](../../log/utils/__init__.md#LogColors.END), [`_create_embedding_inner_function`](litellm.md#LiteLLMAPIBackend._create_embedding_inner_function), [`log_llm_chat_content`](../llm_conf.md#LLMSettings.log_llm_chat_content), [`started`](../../log/timer.md#RDAgentTimer.started), [`_calculate_token_from_messages`](deprec.md#DeprecBackend._calculate_token_from_messages), [`_calculate_token_from_messages`](litellm.md#LiteLLMAPIBackend._calculate_token_from_messages), [`add_duration`](../../log/timer.md#RDAgentTimer.add_duration), [`LLM_CACHE_SEED_GEN`](../../core/utils.md#LLM_CACHE_SEED_GEN), [`CYAN`](../../log/utils/__init__.md#LogColors.CYAN), [`_create_embedding_inner_function`](deprec.md#DeprecBackend._create_embedding_inner_function), [`parse`](base.md#CodeBlockParser.parse), [`chat_set`](base.md#SQliteLazyCache.chat_set), [`embedding_set`](base.md#SQliteLazyCache.embedding_set), [`dump_chat_cache`](../llm_conf.md#LLMSettings.dump_chat_cache), [`use_chat_cache`](../llm_conf.md#LLMSettings.use_chat_cache), [`chat_token_limit`](litellm.md#LiteLLMAPIBackend.chat_token_limit), [`supports_response_schema`](litellm.md#LiteLLMAPIBackend.supports_response_schema), [`use_auto_chat_cache_seed_gen`](../llm_conf.md#LLMSettings.use_auto_chat_cache_seed_gen), [`openai_imported`](base.md#openai_imported), [`chat_get`](base.md#SQliteLazyCache.chat_get), [`embedding_get`](base.md#SQliteLazyCache.embedding_get), [`parse`](base.md#JSONParser.parse), [`LiteLLMAPIBackend`](litellm.md#LiteLLMAPIBackend), [`SQliteLazyCache`](base.md#SQliteLazyCache), [`truncate_content_list`](../utils/embedding.md#truncate_content_list), [`PolicyError`](../../core/exception.md#PolicyError), [`system_prompt_role`](../llm_conf.md#LLMSettings.system_prompt_role), [`DeprecBackend`](deprec.md#DeprecBackend), [`MAGENTA`](../../log/utils/__init__.md#LogColors.MAGENTA), [`embedding_model`](../llm_conf.md#LLMSettings.embedding_model)  (+19 more)
- used by: [`responses`](../../app/CI/run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`hypothesis_gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`_gen_hypothesis`](../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`_create_chat_completion_inner_function`](deprec.md#DeprecBackend._create_chat_completion_inner_function), [`implement_data`](../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`hypothesis_select_with_llm`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`task_gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.task_gen), [`gen`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV1ExpGen.gen), [`generate_feedback`](../../scenarios/data_science/dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/finetune/dev/feedback.md#FTExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`implement_one_task`](../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`_generate_and_run_script`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`implement_one_task`](../../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llamafactory_config_with_llm`](../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`implement_one_task`](../../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`generate_feedback`](../../scenarios/qlib/developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../../scenarios/qlib/developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`implement_one_task`](../../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`_create_chat_completion_inner_function`](litellm.md#LiteLLMAPIBackend._create_chat_completion_inner_function), [`hypothesis_rewrite`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`implement_one_task`](../../components/coder/model_coder/evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`build_cls_from_json_with_retry`](../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`_generate_code`](../../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`evaluate`](../../components/coder/model_coder/eva_utils.md#ModelCodeEvaluator.evaluate), [`llm_log_win`](../../log/ui/ds_trace.md#llm_log_win), [`task_gen`](../../scenarios/data_science/proposal/exp_gen/draft/draft.md#DSDraftV2ExpGen.task_gen), [`sample_ideas`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.sample_ideas), [`_analysis_competition_description`](../../scenarios/kaggle/experiment/scenario.md#KGScenario._analysis_competition_description), [`evaluate`](../../components/coder/model_coder/eva_utils.md#ModelFinalEvaluator.evaluate), [`identify_feedback_problem`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.identify_feedback_problem), [`identify_scenario_problem`](../../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.identify_scenario_problem), [`evaluate`](../../components/coder/factor_coder/eva_utils.md#FactorCodeEvaluator.evaluate), [`convert`](../../components/coder/data_science/share/notebook.md#NotebookConverter.convert), [`get_sota_exp_to_submit`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#AutoSOTAexpSelector.get_sota_exp_to_submit), [`filter_redundant_text`](../../utils/__init__.md#filter_redundant_text)  (+52 more; 13 test-only)

### `ChatSession`
- def: [`rdagent/oai/backend/base.py:286`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L286)
- signature: `class ChatSession:`
- members:
  - `build_chat_completion(self, user_prompt: str, *args, **kwargs)` — [`L309`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L309) — this function is to build the session messages — documented in [rdagent-app-CI-run](../../../../concepts/rdagent-app-CI-run.md)
  - `build_chat_completion_message(self, user_prompt: str)` — [`L292`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L292) — documented in [rdagent-oai-llm_conf](../../../../concepts/rdagent-oai-llm_conf.md)
  - `build_chat_completion_message_and_calculate_token(self, user_prompt: str)` — [`L305`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L305)
  - `display_history(self)` — [`L348`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L348)
  - `get_conversation_id(self)` — [`L345`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L345)
  - `api_backend` — [`L290`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L290)
  - `conversation_id` — [`L288`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L288)
  - `system_prompt` — [`L289`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L289)
- protocol/private: `__init__`[`L287`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L287)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`LLM_SETTINGS`](../llm_conf.md#LLM_SETTINGS), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`tag`](../../log/logger.md#RDAgentLog.tag), [`message_get`](base.md#SessionChatHistoryCache.message_get), [`message_set`](base.md#SessionChatHistoryCache.message_set), [`SessionChatHistoryCache`](base.md#SessionChatHistoryCache), [`system_prompt_role`](../llm_conf.md#LLMSettings.system_prompt_role), [`default_system_prompt`](../llm_conf.md#LLMSettings.default_system_prompt)
- used by: [`responses`](../../app/CI/run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`_gen_hypothesis`](../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`implement_one_task`](../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llamafactory_config_with_llm`](../../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`_generate_code`](../../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`__check_factor_duplication_simulate_json_mode`](../../scenarios/qlib/factor_experiment_loader/pdf_loader.md#__check_factor_duplication_simulate_json_mode), [`analyze_one_document`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.analyze_one_document), [`extract_model_from_doc`](../../components/coder/model_coder/task_loader.md#extract_model_from_doc), [`build_chat_session`](base.md#APIBackend.build_chat_session), [`__extract_factors_formulation_from_content`](../../scenarios/qlib/factor_experiment_loader/pdf_loader.md#__extract_factors_formulation_from_content), [`__extract_factors_name_and_desc_from_content`](../../scenarios/qlib/factor_experiment_loader/pdf_loader.md#__extract_factors_name_and_desc_from_content)  (1 test-only)

### `CodeBlockParser`
- def: [`rdagent/oai/backend/base.py:139`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L139)
- doc: Generic code block extractor supporting multiple languages.
- signature: `class CodeBlockParser:`
- members:
  - `__init__(self, language: str = "python", fallback_to_raw: bool = False)` — [`L150`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L150) — Args:
  - `_get_language_aliases(self, language: str)` — [`L161`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L161) — Get all possible aliases for the language.
  - `parse(self, content: str)` — [`L168`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L168) — Parse content and extract code block with exact language tag.
  - `SUPPORTED_LANGUAGES` — [`L145`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L145)
  - `fallback_to_raw` — [`L158`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L158)
  - `language` — [`L157`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L157)
- protocol/private: `_lang_aliases`[`L159`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L159)
- uses (calls/refs, reference-scoped): [`CodeBlockParseError`](../../core/exception.md#CodeBlockParseError)
- used by: [`_create_chat_completion_auto_continue`](base.md#APIBackend._create_chat_completion_auto_continue)

### `JSONParser`
- def: [`rdagent/oai/backend/base.py:37`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L37)
- doc: JSON parser supporting multiple strategies
- signature: `class JSONParser:`
- members:
  - `_direct_parse(self, content: str)` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L71) — Strategy 1: Direct parsing (including handling extra data)
  - `_extract_first_json(response: str)` — [`L132`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L132) — Extract the first complete JSON object, ignoring extra content
  - `_extract_from_code_block(self, content: str)` — [`L81`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L81) — Strategy 2: Extract JSON from code block
  - `_extract_with_fix_combined(self, content: str)` — [`L95`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L95) — Strategy 4: Combined strategy - fix Python syntax first, then extract the first JSON object
  - `_fix_python_booleans(json_str: str)` — [`L107`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L107) — Safely fix Python-style booleans to JSON standard format using tokenize
  - `_fix_python_syntax(self, content: str)` — [`L90`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L90) — Strategy 3: Fix Python syntax before parsing
  - `parse(self, content: str)` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L49) — Parse JSON content, automatically trying multiple strategies
  - `add_json_in_prompt` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L47)
  - `strategies` — [`L41`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L41)
- protocol/private: `__init__`[`L40`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L40)
- used by: [`_create_chat_completion_auto_continue`](base.md#APIBackend._create_chat_completion_auto_continue)

### `SQliteLazyCache`  ·  implements/extends SingletonBaseClass
- def: [`rdagent/oai/backend/base.py:195`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L195)
- signature: `class SQliteLazyCache(SingletonBaseClass):`
- members:
  - `chat_get(self, key: str)` — [`L230`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L230)
  - `chat_set(self, key: str, value: str)` — [`L242`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L242)
  - `embedding_get(self, key: str)` — [`L236`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L236)
  - `embedding_set(self, content_to_embedding_dict: dict)` — [`L251`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L251)
  - `message_get(self, conversation_id: str)` — [`L260`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L260)
  - `message_set(self, conversation_id: str, message_value: list[dict[str, Any]])` — [`L265`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L265)
  - `c` — [`L202`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L202)
  - `cache_location` — [`L198`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L198)
  - `conn` — [`L201`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L201)
- protocol/private: `__init__`[`L196`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L196)
- uses (calls/refs, reference-scoped): [`SingletonBaseClass`](../../core/utils.md#SingletonBaseClass), [`md5_hash`](../../utils/__init__.md#md5_hash)
- used by: [`_create_chat_completion_auto_continue`](base.md#APIBackend._create_chat_completion_auto_continue), [`SingletonBaseClass`](../../core/utils.md#SingletonBaseClass), [`_create_embedding_with_cache`](base.md#APIBackend._create_embedding_with_cache), [`cache`](base.md#SessionChatHistoryCache.cache), [`cache`](base.md#APIBackend.cache), [`message_get`](base.md#SessionChatHistoryCache.message_get), [`message_set`](base.md#SessionChatHistoryCache.message_set)

### `SessionChatHistoryCache`  ·  implements/extends SingletonBaseClass
- def: [`rdagent/oai/backend/base.py:274`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L274)
- signature: `class SessionChatHistoryCache(SingletonBaseClass):`
- members:
  - `__init__(self)` — [`L275`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L275) — load all history conversation json file from self.session_cache_location
  - `message_get(self, conversation_id: str)` — [`L279`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L279)
  - `message_set(self, conversation_id: str, message_value: list[dict[str, Any]])` — [`L282`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L282)
  - `cache` — [`L277`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L277)
- uses (calls/refs, reference-scoped): [`LLM_SETTINGS`](../llm_conf.md#LLM_SETTINGS), [`SingletonBaseClass`](../../core/utils.md#SingletonBaseClass), [`message_set`](base.md#SQliteLazyCache.message_set), [`SQliteLazyCache`](base.md#SQliteLazyCache), [`message_get`](base.md#SQliteLazyCache.message_get), [`prompt_cache_path`](../llm_conf.md#LLMSettings.prompt_cache_path)
- used by: [`build_chat_completion`](base.md#ChatSession.build_chat_completion), [`SingletonBaseClass`](../../core/utils.md#SingletonBaseClass), [`build_chat_completion_message`](base.md#ChatSession.build_chat_completion_message)

## Module values
- `openai_imported` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/oai/backend/base.py#L32)

