---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/router/router.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/router/router.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.router.router`/
symbols:
  SlimeRouter._health_check_loop: SlimeRouter#_health_check_loop().
  SlimeRouter.worker_request_counts: SlimeRouter#worker_request_counts.
  SlimeRouter._setup_routes: SlimeRouter#_setup_routes().
  SlimeRouter.proxy: SlimeRouter#proxy().
  SlimeRouter.app: SlimeRouter#app.
  SlimeRouter.client: SlimeRouter#client.
  parser: parser.
  run_router: run_router().
  SlimeRouter._check_worker_health: SlimeRouter#_check_worker_health().
  SlimeRouter.add_worker: SlimeRouter#add_worker().
  args: args.
  logger: logger.
  SlimeRouter._use_url: SlimeRouter#_use_url().
  SlimeRouter.dead_workers: SlimeRouter#dead_workers.
  SlimeRouter.worker_failure_counts: SlimeRouter#worker_failure_counts.
  SlimeRouter._start_background_health_check: SlimeRouter#_start_background_health_check().
  SlimeRouter.list_workers: SlimeRouter#list_workers().
  SlimeRouter._finish_url: SlimeRouter#_finish_url().
  SlimeRouter.args: SlimeRouter#args.
  SlimeRouter.verbose: SlimeRouter#verbose.
  SlimeRouter.retrieve_from_text: SlimeRouter#retrieve_from_text().
  SlimeRouter: SlimeRouter#
  SlimeRouter.__init__: SlimeRouter#__init__().
  SlimeRouter.max_weight_version: SlimeRouter#max_weight_version.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/router/router.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py)

## Classes
### `SlimeRouter`
- def: [`OpenMLE-ERL/SFT/slime/slime/router/router.py:28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L28)
- members:
  - `__init__(self, args, verbose=False)` — [`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L29) — Initialize the slime-router with SGLang router address
  - `_check_worker_health(self, url)` — [`L78`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L78) — Encapsulated health check logic for better maintainability.
  - `_finish_url(self, url)` — [`L242`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L242) — Mark the request to the given URL as finished
  - `_health_check_loop(self)` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L89) — Background loop to monitor worker health and adjust routing pool.
  - `_setup_routes(self)` — [`L66`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L66) — Setup all the HTTP routes
  - `_use_url(self)` — [`L225`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L225) — Select worker URL with minimal active requests.
  - `add_worker(self, request: Request)` — [`L169`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L169) — Add a new worker to the router.
  - `list_workers(self, request: Request)` — [`L199`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L199) — List all registered workers
  - `proxy(self, request: Request, path: str)` — [`L131`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L131) — Proxy all other requests to the SGLang router
  - `retrieve_from_text(self, request: Request)` — [`L203`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L203) — Get token information from text input
  - `app` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L34)
  - `args` — [`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L31)
  - `client` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L53)
  - `dead_workers` — [`L42`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L42)
  - `max_weight_version` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L43)
  - `verbose` — [`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L32)
  - `worker_failure_counts` — [`L40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L40)
  - `worker_request_counts` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L38)
- protocol/private: `_start_background_health_check`[`L75`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L75)
- uses (calls/refs, reference-scoped): `status_code`, [`load_function`](../utils/misc.md#load_function), [`logger`](router.md#logger), `headers`
- used by: [`run_router`](router.md#run_router)

## Functions
- `run_router(args)` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L17) — Run the Slime router with the specified configuration.

## Module values
- `args` — [`L258`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L258)
- `logger` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L14)
- `parser` — [`L250`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/router/router.py#L250)

