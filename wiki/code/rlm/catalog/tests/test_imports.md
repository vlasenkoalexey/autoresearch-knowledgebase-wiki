---
title: 'Module: tests/test_imports.py'
type: catalog
provenance: extracted
module: tests/test_imports.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_imports`/Test
symbols:
  TestCoreImports.test_core_types_import: CoreImports#test_core_types_import().
  TestImportCompleteness.test_all_environment_classes_importable: ImportCompleteness#test_all_environment_classes_importable().
  TestCoreImports.test_core_comms_utils_import: CoreImports#test_core_comms_utils_import().
  TestUtilsImports.test_prompts_import: UtilsImports#test_prompts_import().
  TestImportCompleteness.test_all_client_classes_importable: ImportCompleteness#test_all_client_classes_importable().
  TestEnvironmentImports.test_base_env_import: EnvironmentImports#test_base_env_import().
  TestUtilsImports.test_parsing_import: UtilsImports#test_parsing_import().
  TestImportConflicts.test_no_naming_conflicts_across_modules: ImportConflicts#test_no_naming_conflicts_across_modules().
  TestImportConflicts.test_all_declarations_match_exports: ImportConflicts#test_all_declarations_match_exports().
  TestTopLevelImports.test_rlm_import: TopLevelImports#test_rlm_import().
  TestTopLevelImports.test_rlm_rlm_import: TopLevelImports#test_rlm_rlm_import().
  TestTopLevelImports.test_rlm_core_rlm_import: TopLevelImports#test_rlm_core_rlm_import().
  TestClientImports.test_base_lm_import: ClientImports#test_base_lm_import().
  TestClientImports.test_openai_client_import: ClientImports#test_openai_client_import().
  TestClientImports.test_anthropic_client_import: ClientImports#test_anthropic_client_import().
  TestClientImports.test_portkey_client_import: ClientImports#test_portkey_client_import().
  TestClientImports.test_get_client_function: ClientImports#test_get_client_function().
  TestCoreImports.test_core_rlm_import: CoreImports#test_core_rlm_import().
  TestCoreImports.test_core_lm_handler_import: CoreImports#test_core_lm_handler_import().
  TestEnvironmentImports.test_local_repl_import: EnvironmentImports#test_local_repl_import().
  TestEnvironmentImports.test_modal_repl_import: EnvironmentImports#test_modal_repl_import().
  TestEnvironmentImports.test_docker_repl_import: EnvironmentImports#test_docker_repl_import().
  TestEnvironmentImports.test_prime_repl_import: EnvironmentImports#test_prime_repl_import().
  TestEnvironmentImports.test_get_environment_function: EnvironmentImports#test_get_environment_function().
  TestLoggerImports.test_logger_module_import: LoggerImports#test_logger_module_import().
  TestLoggerImports.test_rlm_logger_import: LoggerImports#test_rlm_logger_import().
  TestLoggerImports.test_verbose_import: LoggerImports#test_verbose_import().
  TestUtilsImports.test_rlm_utils_import: UtilsImports#test_rlm_utils_import().
  TestImportConflicts.test_no_duplicate_names_in_rlm_all: ImportConflicts#test_no_duplicate_names_in_rlm_all().
  TestImportConflicts.test_no_duplicate_names_in_logger_all: ImportConflicts#test_no_duplicate_names_in_logger_all().
  TestTopLevelImports: TopLevelImports#
  TestClientImports: ClientImports#
  TestClientImports.test_clients_module_import: ClientImports#test_clients_module_import().
  TestCoreImports: CoreImports#
  TestEnvironmentImports: EnvironmentImports#
  TestEnvironmentImports.test_environments_module_import: EnvironmentImports#test_environments_module_import().
  TestLoggerImports: LoggerImports#
  TestUtilsImports: UtilsImports#
  TestImportConflicts: ImportConflicts#
  TestImportConflicts.test_no_circular_imports: ImportConflicts#test_no_circular_imports().
  TestImportCompleteness: ImportCompleteness#
---
# Module: [`tests/test_imports.py`](../../../../../raw/code/rlm/tests/test_imports.py)

## Classes
### `TestClientImports`
- def: [`tests/test_imports.py:33`](../../../../../raw/code/rlm/tests/test_imports.py#L33)
- doc: Test client module imports.
- signature: `class TestClientImports:`
- members:
  - `test_anthropic_client_import(self)` — [`L56`](../../../../../raw/code/rlm/tests/test_imports.py#L56) — Test AnthropicClient import.
  - `test_base_lm_import(self)` — [`L43`](../../../../../raw/code/rlm/tests/test_imports.py#L43) — Test BaseLM import.
  - `test_clients_module_import(self)` — [`L36`](../../../../../raw/code/rlm/tests/test_imports.py#L36) — Test that clients module can be imported.
  - `test_get_client_function(self)` — [`L70`](../../../../../raw/code/rlm/tests/test_imports.py#L70) — Test get_client function import.
  - `test_openai_client_import(self)` — [`L49`](../../../../../raw/code/rlm/tests/test_imports.py#L49) — Test OpenAIClient import.
  - `test_portkey_client_import(self)` — [`L63`](../../../../../raw/code/rlm/tests/test_imports.py#L63) — Test PortkeyClient import.
- uses (calls/refs, reference-scoped): [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`get_client`](../rlm/clients/__init__.md#get_client), [`OpenAIClient`](../rlm/clients/openai.md#OpenAIClient), [`PortkeyClient`](../rlm/clients/portkey.md#PortkeyClient), [`AnthropicClient`](../rlm/clients/anthropic.md#AnthropicClient)

### `TestCoreImports`
- def: [`tests/test_imports.py:77`](../../../../../raw/code/rlm/tests/test_imports.py#L77)
- doc: Test core module imports.
- signature: `class TestCoreImports:`
- members:
  - `test_core_comms_utils_import(self)` — [`L114`](../../../../../raw/code/rlm/tests/test_imports.py#L114) — Test comms_utils imports.
  - `test_core_lm_handler_import(self)` — [`L108`](../../../../../raw/code/rlm/tests/test_imports.py#L108) — Test LMHandler import.
  - `test_core_rlm_import(self)` — [`L102`](../../../../../raw/code/rlm/tests/test_imports.py#L102) — Test core RLM import.
  - `test_core_types_import(self)` — [`L80`](../../../../../raw/code/rlm/tests/test_imports.py#L80) — Test core types imports.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`UsageSummary`](../rlm/core/types.md#UsageSummary), [`ModelUsageSummary`](../rlm/core/types.md#ModelUsageSummary), [`REPLResult`](../rlm/core/types.md#REPLResult), [`send_lm_request_batched`](../rlm/core/comms_utils.md#send_lm_request_batched), [`send_lm_request`](../rlm/core/comms_utils.md#send_lm_request), [`RLMIteration`](../rlm/core/types.md#RLMIteration), [`LMHandler`](../rlm/core/lm_handler.md#LMHandler), [`LMRequest`](../rlm/core/comms_utils.md#LMRequest), [`LMResponse`](../rlm/core/comms_utils.md#LMResponse), [`CodeBlock`](../rlm/core/types.md#CodeBlock), [`QueryMetadata`](../rlm/core/types.md#QueryMetadata), [`RLMMetadata`](../rlm/core/types.md#RLMMetadata), [`socket_send`](../rlm/core/comms_utils.md#socket_send), [`ClientBackend`](../rlm/core/types.md#ClientBackend), [`socket_recv`](../rlm/core/comms_utils.md#socket_recv)

### `TestEnvironmentImports`
- def: [`tests/test_imports.py:133`](../../../../../raw/code/rlm/tests/test_imports.py#L133)
- doc: Test environment module imports.
- signature: `class TestEnvironmentImports:`
- members:
  - `test_base_env_import(self)` — [`L144`](../../../../../raw/code/rlm/tests/test_imports.py#L144) — Test BaseEnv import.
  - `test_docker_repl_import(self)` — [`L165`](../../../../../raw/code/rlm/tests/test_imports.py#L165) — Test DockerREPL import.
  - `test_environments_module_import(self)` — [`L136`](../../../../../raw/code/rlm/tests/test_imports.py#L136) — Test that environments module can be imported.
  - `test_get_environment_function(self)` — [`L178`](../../../../../raw/code/rlm/tests/test_imports.py#L178) — Test get_environment function import.
  - `test_local_repl_import(self)` — [`L152`](../../../../../raw/code/rlm/tests/test_imports.py#L152) — Test LocalREPL import.
  - `test_modal_repl_import(self)` — [`L158`](../../../../../raw/code/rlm/tests/test_imports.py#L158) — Test ModalREPL import.
  - `test_prime_repl_import(self)` — [`L171`](../../../../../raw/code/rlm/tests/test_imports.py#L171) — Test PrimeREPL import.
- uses (calls/refs, reference-scoped): [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`get_environment`](../rlm/environments/__init__.md#get_environment), [`IsolatedEnv`](../rlm/environments/base_env.md#IsolatedEnv), [`DockerREPL`](../rlm/environments/docker_repl.md#DockerREPL), [`NonIsolatedEnv`](../rlm/environments/base_env.md#NonIsolatedEnv), [`BaseEnv`](../rlm/environments/base_env.md#BaseEnv), [`ModalREPL`](../rlm/environments/modal_repl.md#ModalREPL), [`PrimeREPL`](../rlm/environments/prime_repl.md#PrimeREPL)

### `TestImportCompleteness`
- def: [`tests/test_imports.py:421`](../../../../../raw/code/rlm/tests/test_imports.py#L421)
- doc: Test that all expected imports are available.
- signature: `class TestImportCompleteness:`
- members:
  - `test_all_client_classes_importable(self)` — [`L424`](../../../../../raw/code/rlm/tests/test_imports.py#L424) — Test that all client classes can be imported.
  - `test_all_environment_classes_importable(self)` — [`L456`](../../../../../raw/code/rlm/tests/test_imports.py#L456) — Test that all environment classes can be imported.
- uses (calls/refs, reference-scoped): [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`BaseLM`](../rlm/clients/base_lm.md#BaseLM), [`IsolatedEnv`](../rlm/environments/base_env.md#IsolatedEnv), [`DockerREPL`](../rlm/environments/docker_repl.md#DockerREPL), [`OpenAIClient`](../rlm/clients/openai.md#OpenAIClient), [`NonIsolatedEnv`](../rlm/environments/base_env.md#NonIsolatedEnv), [`BaseEnv`](../rlm/environments/base_env.md#BaseEnv), [`PortkeyClient`](../rlm/clients/portkey.md#PortkeyClient), [`ModalREPL`](../rlm/environments/modal_repl.md#ModalREPL), [`AnthropicClient`](../rlm/clients/anthropic.md#AnthropicClient), [`PrimeREPL`](../rlm/environments/prime_repl.md#PrimeREPL)

### `TestImportConflicts`
- def: [`tests/test_imports.py:246`](../../../../../raw/code/rlm/tests/test_imports.py#L246)
- doc: Test for import conflicts and naming issues.
- signature: `class TestImportConflicts:`
- members:
  - `test_all_declarations_match_exports(self)` — [`L269`](../../../../../raw/code/rlm/tests/test_imports.py#L269) — Test that __all__ declarations match actual exports.
  - `test_no_circular_imports(self)` — [`L286`](../../../../../raw/code/rlm/tests/test_imports.py#L286) — Test that modules can be imported without circular import errors.
  - `test_no_duplicate_names_in_logger_all(self)` — [`L259`](../../../../../raw/code/rlm/tests/test_imports.py#L259) — Test that __all__ in rlm.logger.__init__ has no duplicates.
  - `test_no_duplicate_names_in_rlm_all(self)` — [`L249`](../../../../../raw/code/rlm/tests/test_imports.py#L249) — Test that __all__ in rlm.__init__ has no duplicates.
  - `test_no_naming_conflicts_across_modules(self)` — [`L346`](../../../../../raw/code/rlm/tests/test_imports.py#L346) — Test that there are no naming conflicts across different modules.
- uses (calls/refs, reference-scoped): [`__all__`](../rlm/logger/__init__.md#__all__), [`__all__`](../rlm/__init__.md#__all__), [`__all__`](../rlm/environments/__init__.md#__all__)

### `TestLoggerImports`
- def: [`tests/test_imports.py:185`](../../../../../raw/code/rlm/tests/test_imports.py#L185)
- doc: Test logger module imports.
- signature: `class TestLoggerImports:`
- members:
  - `test_logger_module_import(self)` — [`L188`](../../../../../raw/code/rlm/tests/test_imports.py#L188) — Test that logger module can be imported.
  - `test_rlm_logger_import(self)` — [`L197`](../../../../../raw/code/rlm/tests/test_imports.py#L197) — Test RLMLogger import.
  - `test_verbose_import(self)` — [`L203`](../../../../../raw/code/rlm/tests/test_imports.py#L203) — Test VerbosePrinter import.
- uses (calls/refs, reference-scoped): [`RLMLogger`](../rlm/logger/rlm_logger.md#RLMLogger), [`VerbosePrinter`](../rlm/logger/verbose.md#VerbosePrinter), [`__all__`](../rlm/logger/__init__.md#__all__)

### `TestTopLevelImports`
- def: [`tests/test_imports.py:10`](../../../../../raw/code/rlm/tests/test_imports.py#L10)
- doc: Test top-level package imports.
- signature: `class TestTopLevelImports:`
- members:
  - `test_rlm_core_rlm_import(self)` — [`L26`](../../../../../raw/code/rlm/tests/test_imports.py#L26) — Test that RLM can be imported from rlm.core.rlm.
  - `test_rlm_import(self)` — [`L13`](../../../../../raw/code/rlm/tests/test_imports.py#L13) — Test that main rlm package can be imported.
  - `test_rlm_rlm_import(self)` — [`L20`](../../../../../raw/code/rlm/tests/test_imports.py#L20) — Test that RLM class can be imported from rlm.
- uses (calls/refs, reference-scoped): [`RLM`](../rlm/core/rlm.md#RLM), [`__all__`](../rlm/__init__.md#__all__)

### `TestUtilsImports`
- def: [`tests/test_imports.py:210`](../../../../../raw/code/rlm/tests/test_imports.py#L210)
- doc: Test utils module imports.
- signature: `class TestUtilsImports:`
- members:
  - `test_parsing_import(self)` — [`L213`](../../../../../raw/code/rlm/tests/test_imports.py#L213) — Test parsing module import.
  - `test_prompts_import(self)` — [`L225`](../../../../../raw/code/rlm/tests/test_imports.py#L225) — Test prompts module import.
  - `test_rlm_utils_import(self)` — [`L239`](../../../../../raw/code/rlm/tests/test_imports.py#L239) — Test rlm_utils module import.
- uses (calls/refs, reference-scoped): [`format_iteration`](../rlm/utils/parsing.md#format_iteration), [`format_execution_result`](../rlm/utils/parsing.md#format_execution_result), [`build_rlm_system_prompt`](../rlm/utils/prompts.md#build_rlm_system_prompt), [`find_code_blocks`](../rlm/utils/parsing.md#find_code_blocks), [`build_user_prompt`](../rlm/utils/prompts.md#build_user_prompt), [`RLM_SYSTEM_PROMPT`](../rlm/utils/prompts.md#RLM_SYSTEM_PROMPT), [`filter_sensitive_keys`](../rlm/utils/rlm_utils.md#filter_sensitive_keys), [`USER_PROMPT`](../rlm/utils/prompts.md#USER_PROMPT)

