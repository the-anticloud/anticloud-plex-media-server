# Educators — PLEX_MEDIA_SERVER

**Project:** PLEX_MEDIA_SERVER  
**Category:** MOVIES_MEDIA  
**Upstream:** https://github.com/plexinc/pms-docker  
**Pinned commit:** `653dcadd70f39c032fe5aea72a3fad8b2bd87162`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`  
**Date:** October 2026

## Teaching with PLEX_MEDIA_SERVER

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
