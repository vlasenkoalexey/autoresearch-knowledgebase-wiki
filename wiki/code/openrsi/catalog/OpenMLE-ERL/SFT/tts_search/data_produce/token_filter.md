---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.token_filter`/
symbols:
  filter_by_token_length: filter_by_token_length().
  count_message_tokens: count_message_tokens().
  load_tokenizer: load_tokenizer().
  _init_worker: _init_worker().
  _count_one: _count_one().
  count_chat_template_tokens: count_chat_template_tokens().
  TokenFilterConfig: TokenFilterConfig#
  _import_auto_tokenizer: _import_auto_tokenizer().
  TokenFilterConfig.tokenizer_model: TokenFilterConfig#tokenizer_model.
  token_count_within_limit: token_count_within_limit().
  TokenFilterConfig.max_total_tokens: TokenFilterConfig#max_total_tokens.
  TokenFilterConfig.workers: TokenFilterConfig#workers.
  TokenFilterConfig.keep_equal: TokenFilterConfig#keep_equal.
  TOKENIZER.TOKENIZER: TOKENIZER.TOKENIZER.
  TokenFilterConfig.local_files_only: TokenFilterConfig#local_files_only.
  _import_auto_tokenizer.patched_version: _import_auto_tokenizer().patched_version().
  TokenFilterConfig.chunksize: TokenFilterConfig#chunksize.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py)

## Classes
### `TokenFilterConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py:44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L44)
- doc: Tokenizer length filtering configuration.
- signature: `class TokenFilterConfig:`
- members:
  - `chunksize` — [`L62`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L62)
  - `keep_equal` — [`L63`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L63)
  - `local_files_only` — [`L64`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L64)
  - `max_total_tokens` — [`L60`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L60)
  - `tokenizer_model` — [`L59`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L59)
  - `workers` — [`L61`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L61)
- used by: [`build_sft_dataset`](pipeline.md#build_sft_dataset), [`filter_by_token_length`](token_filter.md#filter_by_token_length), [`count_message_tokens`](token_filter.md#count_message_tokens)

## Functions
- `_count_one(item: tuple[int, list[dict[str, str]]])` — [`L122`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L122) — Count tokens for one chat row.
- `_import_auto_tokenizer()` — [`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L17) — Import AutoTokenizer in this local env with a known metadata mismatch.
- `_init_worker(tokenizer_model: str, local_files_only: bool)` — [`L67`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L67) — Initialize a process-local tokenizer.
- `count_chat_template_tokens(messages: list[dict[str, str]], tokenizer: Any)` — [`L98`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L98) — Count final SLIME chat-template tokens for one message list.
- `count_message_tokens(rows: list[dict[str, Any]], config: TokenFilterConfig)` — [`L135`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L135) — Return exact chat-template token counts for each row.
- `filter_by_token_length(rows: list[dict[str, Any]], config: TokenFilterConfig)` — [`L181`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L181) — Annotate rows with token length and split into kept/dropped rows.
- `load_tokenizer(tokenizer_model: str | Path, local_files_only: bool = True)` — [`L87`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L87) — Load the tokenizer used for SLIME message token accounting.
- `patched_version(distribution_name: str)` — [`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L23)
- `token_count_within_limit(token_count: Any, *, max_total_tokens: int = 32768, keep_equal: bool = True)` — [`L108`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L108) — Return whether a token count passes the configured SLIME limit.

## Module values
- `TOKENIZER` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/token_filter.py#L14)

