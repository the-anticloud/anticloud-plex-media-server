# Ethics — PLEX_MEDIA_SERVER

**Project:** PLEX_MEDIA_SERVER  
**Category:** MOVIES_MEDIA  
**Upstream:** https://github.com/plexinc/pms-docker  
**Pinned commit:** `653dcadd70f39c032fe5aea72a3fad8b2bd87162`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `fbd5c6c81bb1a78466b09190e61defb5b78c6996177b91b15d3ef9155b331a70`  
**Date:** October 2026

## Position

PLEX_MEDIA_SERVER is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
