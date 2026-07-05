---
title: 'Module: rdagent/utils/agent/apply_patch.py'
type: catalog
provenance: extracted
module: rdagent/utils/agent/apply_patch.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.agent.apply_patch`/
symbols:
  Parser.parse: Parser#parse().
  Parser._parse_update_file: Parser#_parse_update_file().
  patch_to_commit: patch_to_commit().
  text_to_patch: text_to_patch().
  DiffError: DiffError#
  apply_commit: apply_commit().
  _get_updated_file: _get_updated_file().
  Parser._parse_add_file: Parser#_parse_add_file().
  process_patch: process_patch().
  Parser._cur_line: Parser#_cur_line().
  ActionType: ActionType#
  apply_patch_from_text: apply_patch_from_text().
  peek_next_section: peek_next_section().
  main: main().
  Parser.is_done: Parser#is_done().
  Parser.read_str: Parser#read_str().
  PatchAction: PatchAction#
  Parser.patch: Parser#patch.
  Chunk.orig_index: Chunk#orig_index.
  Parser.index: Parser#index.
  FileChange.new_content: FileChange#new_content.
  Patch.actions: Patch#actions.
  Parser.prefix: Parser#prefix.
  Parser.read_line: Parser#read_line().
  FileChange: FileChange#
  Patch: Patch#
  Parser._norm: Parser#_norm().
  Parser.startswith: Parser#startswith().
  Commit: Commit#
  ActionType.UPDATE: ActionType#UPDATE.
  Chunk: Chunk#
  Parser.current_files: Parser#current_files.
  Parser.lines: Parser#lines.
  PatchAction.chunks: PatchAction#chunks.
  ActionType.ADD: ActionType#ADD.
  ActionType.DELETE: ActionType#DELETE.
  Commit.changes: Commit#changes.
  find_context: find_context().
  FileChange.move_path: FileChange#move_path.
  Chunk.del_lines: Chunk#del_lines.
  Chunk.ins_lines: Chunk#ins_lines.
  PatchAction.new_file: PatchAction#new_file.
  Parser: Parser#
  Parser.fuzz: Parser#fuzz.
  find_context_core: find_context_core().
  FileChange.old_content: FileChange#old_content.
  PatchAction.move_path: PatchAction#move_path.
  open_file: open_file().
  write_file: write_file().
  remove_file: remove_file().
  identify_files_needed: identify_files_needed().
  load_files: load_files().
  identify_files_added: identify_files_added().
---
# Module: [`rdagent/utils/agent/apply_patch.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py)

## Classes
### `ActionType`  ·  implements/extends Enum, str
- def: [`rdagent/utils/agent/apply_patch.py:21`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L21) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class ActionType(str, Enum):`
- members:
  - `ADD` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L22) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `DELETE` — [`L23`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L23) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `UPDATE` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L24) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- used by: [`_parse_update_file`](apply_patch.md#Parser._parse_update_file), [`parse`](apply_patch.md#Parser.parse), [`patch_to_commit`](apply_patch.md#patch_to_commit), [`apply_commit`](apply_patch.md#apply_commit), [`_get_updated_file`](apply_patch.md#_get_updated_file), [`_parse_add_file`](apply_patch.md#Parser._parse_add_file), [`PatchAction`](apply_patch.md#PatchAction), [`FileChange`](apply_patch.md#FileChange)

### `Chunk`
- def: [`rdagent/utils/agent/apply_patch.py:51`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L51) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class Chunk:`
- members:
  - `del_lines` — [`L53`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L53) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `ins_lines` — [`L54`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L54) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `orig_index` — [`L52`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L52) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- used by: [`_parse_update_file`](apply_patch.md#Parser._parse_update_file), [`_get_updated_file`](apply_patch.md#_get_updated_file), [`peek_next_section`](apply_patch.md#peek_next_section), [`chunks`](apply_patch.md#PatchAction.chunks)

### `Commit`
- def: [`rdagent/utils/agent/apply_patch.py:36`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L36) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class Commit:`
- members:
  - `changes` — [`L37`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L37)
- uses (calls/refs, reference-scoped): [`FileChange`](apply_patch.md#FileChange)
- used by: [`patch_to_commit`](apply_patch.md#patch_to_commit), [`apply_commit`](apply_patch.md#apply_commit)

### `DiffError`  ·  implements/extends ValueError
- def: [`rdagent/utils/agent/apply_patch.py:43`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L43) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- doc: Any problem detected while parsing or applying a patch.
- signature: `class DiffError(ValueError):`
- used by: [`_parse_update_file`](apply_patch.md#Parser._parse_update_file), [`parse`](apply_patch.md#Parser.parse), [`patch_to_commit`](apply_patch.md#patch_to_commit), [`text_to_patch`](apply_patch.md#text_to_patch), [`apply_commit`](apply_patch.md#apply_commit), [`_get_updated_file`](apply_patch.md#_get_updated_file), [`_parse_add_file`](apply_patch.md#Parser._parse_add_file), [`process_patch`](apply_patch.md#process_patch), [`_cur_line`](apply_patch.md#Parser._cur_line), [`apply_patch_from_text`](apply_patch.md#apply_patch_from_text), [`main`](apply_patch.md#main), [`peek_next_section`](apply_patch.md#peek_next_section)

### `FileChange`
- def: [`rdagent/utils/agent/apply_patch.py:28`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L28) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class FileChange:`
- members:
  - `move_path` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L32)
  - `new_content` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L31) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `old_content` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L30) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- uses (calls/refs, reference-scoped): [`ActionType`](apply_patch.md#ActionType)
- used by: [`patch_to_commit`](apply_patch.md#patch_to_commit), [`apply_commit`](apply_patch.md#apply_commit), [`Commit`](apply_patch.md#Commit)

### `Parser`
- def: [`rdagent/utils/agent/apply_patch.py:74`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L74) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class Parser:`
- members:
  - `_norm(line: str)` — [`L89`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L89) — Strip CR so comparisons work for both LF and CRLF input. — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `is_done(self, prefixes: tuple[str, ...] | None = None)` — [`L94`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L94) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `parse(self)` — [`L124`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L124) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `read_line(self)` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L117) — Return the current raw line and advance. — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `read_str(self, prefix: str)` — [`L104`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L104) — Consume the current line if it starts with *prefix* and return the text — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `startswith(self, prefix: str | tuple[str, ...])` — [`L101`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L101)
  - `current_files` — [`L75`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L75) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `fuzz` — [`L79`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L79) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `index` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L77) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `lines` — [`L76`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L76) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `patch` — [`L78`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L78) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `prefix` — [`L80`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L80) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- protocol/private: `_cur_line`[`L83`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L83), `_parse_add_file`[`L225`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L225), `_parse_update_file`[`L173`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L173)
- uses (calls/refs, reference-scoped): [`DiffError`](apply_patch.md#DiffError), [`ActionType`](apply_patch.md#ActionType), [`peek_next_section`](apply_patch.md#peek_next_section), [`PatchAction`](apply_patch.md#PatchAction), [`orig_index`](apply_patch.md#Chunk.orig_index), [`actions`](apply_patch.md#Patch.actions), [`Patch`](apply_patch.md#Patch), [`UPDATE`](apply_patch.md#ActionType.UPDATE), [`chunks`](apply_patch.md#PatchAction.chunks), [`ADD`](apply_patch.md#ActionType.ADD), [`DELETE`](apply_patch.md#ActionType.DELETE), [`find_context`](apply_patch.md#find_context), [`new_file`](apply_patch.md#PatchAction.new_file), [`move_path`](apply_patch.md#PatchAction.move_path)
- used by: [`text_to_patch`](apply_patch.md#text_to_patch)

### `Patch`
- def: [`rdagent/utils/agent/apply_patch.py:66`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L66) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class Patch:`
- members:
  - `actions` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L67) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- uses (calls/refs, reference-scoped): [`PatchAction`](apply_patch.md#PatchAction)
- used by: [`parse`](apply_patch.md#Parser.parse), [`patch_to_commit`](apply_patch.md#patch_to_commit), [`text_to_patch`](apply_patch.md#text_to_patch), [`patch`](apply_patch.md#Parser.patch)

### `PatchAction`
- def: [`rdagent/utils/agent/apply_patch.py:58`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L58) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- signature: `class PatchAction:`
- members:
  - `chunks` — [`L61`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L61) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `move_path` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L62) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
  - `new_file` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L60) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- uses (calls/refs, reference-scoped): [`ActionType`](apply_patch.md#ActionType), [`Chunk`](apply_patch.md#Chunk)
- used by: [`_parse_update_file`](apply_patch.md#Parser._parse_update_file), [`parse`](apply_patch.md#Parser.parse), [`patch_to_commit`](apply_patch.md#patch_to_commit), [`_get_updated_file`](apply_patch.md#_get_updated_file), [`_parse_add_file`](apply_patch.md#Parser._parse_add_file), [`Patch`](apply_patch.md#Patch)

## Functions
- `_get_updated_file(text: str, action: PatchAction, path: str)` — [`L358`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L358) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `apply_commit(commit: Commit, write_fn: Callable[[str, str], None], remove_fn: Callable[[str], None], inplace: bool = False)` — [`L457`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L457)
- `apply_patch_from_text(patch_text: str, inplace: bool = False, prefix: Path | None = None)` — [`L523`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L523) — Apply patch text to filesystem, same as main() but with parameter input
- `find_context(lines: list[str], context: list[str], start: int, eof: bool)` — [`L260`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L260) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `find_context_core(lines: list[str], context: list[str], start: int)` — [`L240`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L240) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `identify_files_added(text: str, prefix: Path | None = None)` — [`L440`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L440)
- `identify_files_needed(text: str, prefix: Path | None = None)` — [`L428`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L428)
- `load_files(paths: list[str], open_fn: Callable[[str], str])` — [`L453`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L453)
- `main()` — [`L535`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L535)
- `open_file(path: str)` — [`L504`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L504)
- `patch_to_commit(patch: Patch, orig: dict[str, str])` — [`L385`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L385) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `peek_next_section(lines: list[str], index: int)` — [`L275`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L275) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `process_patch(text: str, open_fn: Callable[[str], str], write_fn: Callable[[str, str], None], remove_fn: Callable[[str], None], inplace: bool = False, prefix: Path | None = None)` — [`L483`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L483) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `remove_file(path: str)` — [`L516`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L516)
- `text_to_patch(text: str, orig: dict[str, str], prefix: Path | None = None)` — [`L414`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L414) — documented in [rdagent-utils-agent-apply_patch](../../../../concepts/rdagent-utils-agent-apply_patch.md)
- `write_file(path: str, content: str)` — [`L509`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/apply_patch.py#L509)

