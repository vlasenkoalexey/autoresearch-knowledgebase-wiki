---
title: 'Module: OpenMLE-Gym/openmle_gym/leaderboard.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/leaderboard.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.leaderboard`/
symbols:
  download_leaderboards: download_leaderboards().
  _extract_csv: _extract_csv().
  _looks_like_csv: _looks_like_csv().
  BASE_URL: BASE_URL.
  _load_auth: _load_auth().
  _make_session: _make_session().
---
# Module: [`OpenMLE-Gym/openmle_gym/leaderboard.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py)

## Functions
- `_extract_csv(content: bytes, slug: str)` — [`L92`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L92)
- `_load_auth(kaggle_json: str | Path | None = None)` — [`L23`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L23)
- `_looks_like_csv(content: bytes)` — [`L74`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L74)
- `_make_session()` — [`L50`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L50)
- `download_leaderboards(slugs_file: str | Path, out_dir: str | Path, kaggle_json: str | Path | None = None, timeout: int = 120, sleep_seconds: float = 1, execute: bool = False)` — [`L110`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L110)

## Module values
- `BASE_URL` — [`L20`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/leaderboard.py#L20)

