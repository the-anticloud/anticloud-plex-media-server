# Independent Insurance — PLEX_MEDIA_SERVER

**Project:** PLEX_MEDIA_SERVER  
**Category:** MOVIES_MEDIA  
**Upstream:** https://github.com/plexinc/pms-docker  
**Pinned commit:** `653dcadd70f39c032fe5aea72a3fad8b2bd87162`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | PLEX_MEDIA_SERVER with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg
