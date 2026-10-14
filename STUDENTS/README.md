# Students — PLEX_MEDIA_SERVER

**Project:** PLEX_MEDIA_SERVER  
**Category:** MOVIES_MEDIA  
**Upstream:** https://github.com/plexinc/pms-docker  
**Pinned commit:** `653dcadd70f39c032fe5aea72a3fad8b2bd87162`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `653dcadd70f39c032fe5aea72a3fad8b2bd87162`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
