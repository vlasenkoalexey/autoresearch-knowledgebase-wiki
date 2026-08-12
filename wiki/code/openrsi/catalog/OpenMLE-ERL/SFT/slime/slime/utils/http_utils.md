---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.http_utils`/
symbols:
  post: post().
  init_http_client: init_http_client().
  get_host_info: get_host_info().
  _init_ray_distributed_post: _init_ray_distributed_post().
  _post_actors._post_actors: _post_actors._post_actors.
  _post: _post().
  _next_actor: _next_actor().
  find_available_port: find_available_port().
  get: get().
  _init_ray_distributed_post._HttpPosterActor.do_post: _init_ray_distributed_post()._HttpPosterActor#do_post().
  _http_client._http_client: _http_client._http_client.
  get_host_info._resolve_ip: get_host_info()._resolve_ip().
  logger: logger.
  _wrap_ipv6: _wrap_ipv6().
  _client_concurrency._client_concurrency: _client_concurrency._client_concurrency.
  _post_actor_idx._post_actor_idx: _post_actor_idx._post_actor_idx.
  is_port_available: is_port_available().
  _distributed_post_enabled._distributed_post_enabled: _distributed_post_enabled._distributed_post_enabled.
  run_router: run_router().
  get_host_info._is_loopback: get_host_info()._is_loopback().
  SLIME_HOST_IP_ENV: SLIME_HOST_IP_ENV.
  _init_ray_distributed_post._HttpPosterActor: _init_ray_distributed_post()._HttpPosterActor#
  _HttpPosterActor._client: _HttpPosterActor#_client.
  terminate_process: terminate_process().
  _init_ray_distributed_post._HttpPosterActor.__init__: _init_ray_distributed_post()._HttpPosterActor#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py)

## Classes
### `_HttpPosterActor`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py:240`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L240)
- signature: `class _HttpPosterActor:`
- members:
  - `do_post(self, url, payload, max_retries=60, headers=None)` — [`L248`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L248)
- protocol/private: `__init__`[`L241`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L241), `_client`[`L243`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L243)
- uses (calls/refs, reference-scoped): [`_post`](http_utils.md#_post)
- used by: [`_init_ray_distributed_post`](http_utils.md#_init_ray_distributed_post)

## Functions
- `_init_ray_distributed_post(args)` — [`L220`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L220) — Initialize one or more Ray async actors per node for HTTP POST.
- `_is_loopback(ip)` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L48)
- `_next_actor()` — [`L156`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L156)
- `_post(client, url, payload, max_retries=60, headers=None)` — [`L165`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L165)
- `_resolve_ip(family, test_target_ip)` — [`L51`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L51) — Attempt to get the local LAN IP for the specific family (IPv4/IPv6).
- `_wrap_ipv6(host)` — [`L108`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L108) — Wrap IPv6 address in [] if needed.
- `find_available_port(base_port: int)` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L17)
- `get(url)` — [`L291`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L291)
- `get_host_info()` — [`L42`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L42)
- `init_http_client(args)` — [`L201`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L201) — Initialize HTTP client and optionally enable distributed POST via Ray.
- `is_port_available(port)` — [`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L28) — Return whether a port is available.
- `post(url, payload, max_retries=60, headers=None)` — [`L273`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L273)
- `run_router(args)` — [`L117`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L117)
- `terminate_process(process: multiprocessing.Process, timeout: float = 1)` — [`L130`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L130) — Terminate a process gracefully, with forced kill as fallback.

## Module values
- `SLIME_HOST_IP_ENV` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L14)
- `_client_concurrency` — [`L148`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L148)
- `_distributed_post_enabled` — [`L151`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L151)
- `_http_client` — [`L147`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L147)
- `_post_actor_idx` — [`L153`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L153)
- `_post_actors` — [`L152`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L152)
- `logger` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/http_utils.py#L12)

