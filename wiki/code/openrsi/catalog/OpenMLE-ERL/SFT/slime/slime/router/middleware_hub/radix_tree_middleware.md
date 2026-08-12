---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.router.middleware_hub.radix_tree_middleware`/
symbols:
  postprocess_sample_with_radix_tree: postprocess_sample_with_radix_tree().
  RadixTreeMiddleware.dispatch: RadixTreeMiddleware#dispatch().
  RadixTreeMiddleware.radix_tree: RadixTreeMiddleware#radix_tree.
  RadixTreeMiddleware.tokenizer: RadixTreeMiddleware#tokenizer.
  _filter_headers: _filter_headers().
  _materialize_response: _materialize_response().
  RadixTreeMiddleware.router: RadixTreeMiddleware#router.
  HOP_BY_HOP: HOP_BY_HOP.
  RadixTreeMiddleware.args: RadixTreeMiddleware#args.
  RadixTreeMiddleware: RadixTreeMiddleware#
  RadixTreeMiddleware.__init__: RadixTreeMiddleware#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py)

## Classes
### `RadixTreeMiddleware`  ·  implements/extends BaseHTTPMiddleware
- def: [`OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py:59`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L59)
- signature: `class RadixTreeMiddleware(BaseHTTPMiddleware):`
- members:
  - `dispatch(self, request: Request, call_next)` — [`L68`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L68)
  - `args` — [`L63`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L63)
  - `radix_tree` — [`L65`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L65)
  - `router` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L62)
  - `tokenizer` — [`L64`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L64)
- protocol/private: `__init__`[`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L60)
- uses (calls/refs, reference-scoped): [`insert`](radix_tree.md#StringRadixTrie.insert), [`retrieve_from_text`](radix_tree.md#StringRadixTrie.retrieve_from_text), [`_materialize_response`](radix_tree_middleware.md#_materialize_response), [`StringRadixTrie`](radix_tree.md#StringRadixTrie), `body`, `_json`

## Functions
- `_filter_headers(headers)` — [`L30`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L30) — Filter out hop-by-hop headers that should not be forwarded.
- `_materialize_response(resp)` — [`L35`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L35) — Convert streaming-like Response into a regular Response/JSONResponse safely.
- `postprocess_sample_with_radix_tree(args, sample: Sample, output: dict)` — [`L158`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L158)

## Module values
- `HOP_BY_HOP` — [`L17`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/middleware_hub/radix_tree_middleware.py#L17)

