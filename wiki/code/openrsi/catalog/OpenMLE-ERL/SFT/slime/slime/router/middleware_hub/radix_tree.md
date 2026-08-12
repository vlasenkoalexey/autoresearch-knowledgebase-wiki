---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.router.middleware_hub.radix_tree`/
symbols:
  StringRadixTrie.find_longest_prefix: StringRadixTrie#find_longest_prefix().
  StringRadixTrie._insert: StringRadixTrie#_insert().
  result: result.
  StringRadixTrie._print_node: StringRadixTrie#_print_node().
  removed: removed.
  StringRadixTrie.root: StringRadixTrie#root.
  StringRadixTrie.clear: StringRadixTrie#clear().
  StringRadixTrie._remove_node_and_descendants: StringRadixTrie#_remove_node_and_descendants().
  StringRadixTrie.insert: StringRadixTrie#insert().
  StringRadixTrie.retrieve_from_text: StringRadixTrie#retrieve_from_text().
  success: success.
  StringRadixTrie.get_stats: StringRadixTrie#get_stats().
  StringRadixTrie.gc_by_weight_version: StringRadixTrie#gc_by_weight_version().
  StringTreeNode: StringTreeNode#
  StringRadixTrie.remove: StringRadixTrie#remove().
  StringTreeNode.string_key: StringTreeNode#string_key.
  StringTreeNode.token_ids: StringTreeNode#token_ids.
  StringRadixTrie.pretty_print: StringRadixTrie#pretty_print().
  StringRadixTrie.verbose: StringRadixTrie#verbose.
  StringRadixTrie._find_node_by_text: StringRadixTrie#_find_node_by_text().
  StringRadixTrie._remove_node_from_parent: StringRadixTrie#_remove_node_from_parent().
  StringTreeNode.children: StringTreeNode#children.
  StringRadixTrie._clean_node_subtree: StringRadixTrie#_clean_node_subtree().
  trie: trie.
  StringTreeNode.loss_mask: StringTreeNode#loss_mask.
  StringRadixTrie._find_outdated_nodes: StringRadixTrie#_find_outdated_nodes().
  StringRadixTrie._validate_subtree_weight_versions: StringRadixTrie#_validate_subtree_weight_versions().
  gc_removed: gc_removed.
  value: value.
  StringTreeNode.logp: StringTreeNode#logp.
  StringTreeNode.touch: StringTreeNode#touch().
  StringRadixTrie.cur_cache_size: StringRadixTrie#cur_cache_size.
  StringRadixTrie.check_node: StringRadixTrie#check_node().
  StringTreeNode.validate_token_logp_consistency: StringTreeNode#validate_token_logp_consistency().
  StringTreeNode.parent: StringTreeNode#parent.
  StringTreeNode.has_value: StringTreeNode#has_value().
  StringRadixTrie._lock: StringRadixTrie#_lock.
  stats: stats.
  MatchResult.token_ids: MatchResult#token_ids.
  StringTreeNode.id: StringTreeNode#id.
  StringTreeNode.is_evictable: StringTreeNode#is_evictable().
  StringTreeNode.__lt__: StringTreeNode#__lt__().
  StringRadixTrie.cache_hits: StringRadixTrie#cache_hits.
  StringRadixTrie.validate_recursive: StringRadixTrie#validate_recursive().
  query: query.
  MatchResult.matched_prefix: MatchResult#matched_prefix.
  StringTreeNode.ref_count: StringTreeNode#ref_count.
  StringRadixTrie.total_entries: StringRadixTrie#total_entries.
  StringRadixTrie.cache_misses: StringRadixTrie#cache_misses.
  MatchResult.last_node: MatchResult#last_node.
  loss_mask: loss_mask.
  logp: logp.
  MatchResult: MatchResult#
  MatchResult.logp: MatchResult#logp.
  MatchResult.loss_mask: MatchResult#loss_mask.
  StringTreeNode.last_access_time: StringTreeNode#last_access_time.
  StringRadixTrie: StringRadixTrie#
  StringRadixTrie.max_cache_size: StringRadixTrie#max_cache_size.
  StringRadixTrie.gc_threshold_k: StringRadixTrie#gc_threshold_k.
  StringRadixTrie.tokenizer: StringRadixTrie#tokenizer.
  tokens: tokens.
  StringTreeNode.is_leaf: StringTreeNode#is_leaf().
  MatchResult.remaining_string: MatchResult#remaining_string.
  StringTreeNode.counter: StringTreeNode#counter.
  StringTreeNode.access_count: StringTreeNode#access_count.
  StringTreeNode.weight_version: StringTreeNode#weight_version.
  text: text.
  test_cases: test_cases.
  test_queries: test_queries.
  key: key.
  StringTreeNode.__init__: StringTreeNode#__init__().
  StringRadixTrie.__init__: StringRadixTrie#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py)

## Classes
### `MatchResult`
- def: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py:15`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L15)
- doc: Result of prefix matching operation.
- signature: `class MatchResult:`
- members:
  - `last_node` — [`L23`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L23)
  - `logp` — [`L20`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L20)
  - `loss_mask` — [`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L21)
  - `matched_prefix` — [`L18`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L18)
  - `remaining_string` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L22)
  - `token_ids` — [`L19`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L19)
- uses (calls/refs, reference-scoped): [`StringTreeNode`](radix_tree.md#StringTreeNode)
- used by: [`find_longest_prefix`](radix_tree.md#StringRadixTrie.find_longest_prefix), [`result`](radix_tree.md#result), [`removed`](radix_tree.md#removed), [`retrieve_from_text`](radix_tree.md#StringRadixTrie.retrieve_from_text), [`_find_node_by_text`](radix_tree.md#StringRadixTrie._find_node_by_text)

### `StringRadixTrie`
- def: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py:96`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L96)
- doc: String-based Radix Trie for efficient prefix matching and token caching.
- signature: `class StringRadixTrie:`
- members:
  - `__init__(self, max_cache_size: int = 10000, gc_threshold_k: int = 5, tokenizer=None, verbose: bool = False)` — [`L107`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L107) — Initialize the String Radix Trie.
  - `_clean_node_subtree(self, node: StringTreeNode)` — [`L387`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L387) — Clean a node and all its descendants.
  - `_find_node_by_text(self, text: str)` — [`L374`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L374) — Find node by exact text match.
  - `_find_outdated_nodes(self, gc_threshold: int)` — [`L473`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L473) — Find nodes that should be removed based on weight version threshold.
  - `_insert(self, text: str, token_ids: list[int], logp: list[float], loss_mask: list[int], weight_version: int | None = None)` — [`L276`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L276) — Insert tokens - skip tokens for existing nodes just like we skip text.
  - `_print_node(self, node: StringTreeNode, depth: int)` — [`L561`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L561) — Recursively print node structure.
  - `_remove_node_and_descendants(self, node: StringTreeNode)` — [`L400`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L400) — Remove a node and all its descendants from the trie.
  - `_remove_node_from_parent(self, node: StringTreeNode)` — [`L431`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L431) — Remove a node from its parent's children list.
  - `_validate_subtree_weight_versions(self, node: StringTreeNode)` — [`L503`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L503) — Validate that all nodes in subtree have weight_version <= parent weight_version.
  - `check_node(node)` — [`L484`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L484)
  - `clear(self)` — [`L540`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L540) — Clear all entries from the trie.
  - `find_longest_prefix(self, text: str)` — [`L135`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L135) — Find the longest cached prefix for the given text.
  - `gc_by_weight_version(self, current_weight_version: int | None = None)` — [`L439`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L439) — Perform garbage collection based on weight version.
  - `get_stats(self)` — [`L524`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L524) — Get cache statistics.
  - `insert(self, text: str, token_ids: list[int], logp: list[float] | None = None, loss_mask: list[int] | None = None, weight_version: int | None = None)` — [`L201`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L201) — Insert a string and its corresponding token IDs, log probabilities, and loss mask into the trie.
  - `pretty_print(self)` — [`L551`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L551) — Print the trie structure in a readable format.
  - `remove(self, text: str)` — [`L353`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L353) — Remove a string and all nodes with this text as prefix from the trie.
  - `retrieve_from_text(self, text: str, return_logprob: bool = True)` — [`L579`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L579) — Get tokens from text by looking up in radix tree or using tokenizer.
  - `validate_recursive(current_node, parent_weight_version)` — [`L510`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L510)
  - `cache_hits` — [`L128`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L128)
  - `cache_misses` — [`L129`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L129)
  - `cur_cache_size` — [`L130`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L130)
  - `gc_threshold_k` — [`L117`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L117)
  - `max_cache_size` — [`L116`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L116)
  - `root` — [`L122`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L122)
  - `tokenizer` — [`L118`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L118)
  - `total_entries` — [`L127`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L127)
  - `verbose` — [`L119`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L119)
- protocol/private: `_lock`[`L133`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L133)
- uses (calls/refs, reference-scoped): [`StringTreeNode`](radix_tree.md#StringTreeNode), [`string_key`](radix_tree.md#StringTreeNode.string_key), [`token_ids`](radix_tree.md#StringTreeNode.token_ids), [`children`](radix_tree.md#StringTreeNode.children), [`loss_mask`](radix_tree.md#StringTreeNode.loss_mask), [`logp`](radix_tree.md#StringTreeNode.logp), [`touch`](radix_tree.md#StringTreeNode.touch), [`has_value`](radix_tree.md#StringTreeNode.has_value), [`parent`](radix_tree.md#StringTreeNode.parent), [`token_ids`](radix_tree.md#MatchResult.token_ids), [`matched_prefix`](radix_tree.md#MatchResult.matched_prefix), [`ref_count`](radix_tree.md#StringTreeNode.ref_count), [`last_node`](radix_tree.md#MatchResult.last_node), [`MatchResult`](radix_tree.md#MatchResult), [`logp`](radix_tree.md#MatchResult.logp), [`loss_mask`](radix_tree.md#MatchResult.loss_mask), [`access_count`](radix_tree.md#StringTreeNode.access_count), [`remaining_string`](radix_tree.md#MatchResult.remaining_string), [`weight_version`](radix_tree.md#StringTreeNode.weight_version)
- used by: [`result`](radix_tree.md#result), [`removed`](radix_tree.md#removed), [`success`](radix_tree.md#success), [`dispatch`](radix_tree_middleware.md#RadixTreeMiddleware.dispatch), [`radix_tree`](radix_tree_middleware.md#RadixTreeMiddleware.radix_tree), [`trie`](radix_tree.md#trie), [`gc_removed`](radix_tree.md#gc_removed), [`stats`](radix_tree.md#stats)

### `StringTreeNode`
- def: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py:26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L26)
- members:
  - `__lt__(self, other: StringTreeNode)` — [`L91`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L91) — For heap operations - least recently used first.
  - `has_value(self)` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L62) — Check if this node has token IDs stored.
  - `is_evictable(self)` — [`L82`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L82) — Check if this node can be evicted.
  - `is_leaf(self)` — [`L57`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L57) — Check if this node is a leaf node.
  - `touch(self)` — [`L86`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L86) — Update access time and count.
  - `validate_token_logp_consistency(self)` — [`L66`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L66) — Validate that token_ids, logp, and loss_mask have consistent lengths.
  - `access_count` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L44)
  - `children` — [`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L33)
  - `counter` — [`L29`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L29)
  - `id` — [`L53`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L53)
  - `last_access_time` — [`L43`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L43)
  - `logp` — [`L39`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L39)
  - `loss_mask` — [`L40`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L40)
  - `parent` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L34)
  - `ref_count` — [`L47`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L47)
  - `string_key` — [`L37`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L37)
  - `token_ids` — [`L38`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L38)
  - `weight_version` — [`L50`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L50)
- protocol/private: `__init__`[`L31`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L31)
- used by: [`find_longest_prefix`](radix_tree.md#StringRadixTrie.find_longest_prefix), [`_insert`](radix_tree.md#StringRadixTrie._insert), [`_print_node`](radix_tree.md#StringRadixTrie._print_node), [`root`](radix_tree.md#StringRadixTrie.root), [`clear`](radix_tree.md#StringRadixTrie.clear), [`_remove_node_and_descendants`](radix_tree.md#StringRadixTrie._remove_node_and_descendants), [`_find_node_by_text`](radix_tree.md#StringRadixTrie._find_node_by_text), [`_remove_node_from_parent`](radix_tree.md#StringRadixTrie._remove_node_from_parent), [`_clean_node_subtree`](radix_tree.md#StringRadixTrie._clean_node_subtree), [`_find_outdated_nodes`](radix_tree.md#StringRadixTrie._find_outdated_nodes), [`_validate_subtree_weight_versions`](radix_tree.md#StringRadixTrie._validate_subtree_weight_versions), [`last_node`](radix_tree.md#MatchResult.last_node)

## Module values
- `gc_removed` — [`L680`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L680)
- `key` — [`L675`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L675)
- `logp` — [`L633`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L633)
- `loss_mask` — [`L635`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L635)
- `query` — [`L653`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L653)
- `removed` — [`L664`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L664)
- `result` — [`L654`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L654)
- `stats` — [`L674`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L674)
- `success` — [`L636`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L636)
- `test_cases` — [`L625`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L625)
- `test_queries` — [`L644`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L644)
- `text` — [`L633`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L633)
- `tokens` — [`L633`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L633)
- `trie` — [`L622`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L622)
- `value` — [`L675`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree.py#L675)

