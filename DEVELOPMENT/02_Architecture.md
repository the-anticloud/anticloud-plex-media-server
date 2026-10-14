# Technical Architecture — PLEX_MEDIA_SERVER

**Upstream:** [https://github.com/nicedoc/Plex-Media-Server](https://github.com/nicedoc/Plex-Media-Server)
**License:** GPL
**Category:** MOVIES_MEDIA
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

(swap) Use: github.com/nicedoc/emby-server — Emby media server

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local script analysis, scene breakdown, and subtitles
2. AIOSS provenance chain for all production assets (C2PA aligned)
3. AES-256 encryption for pre-release content and DCP masters
4. Single-binary media management tool with no cloud dependency
5. Zero-cloud: all AI analysis, transcription, and subtitling run locally
6. GPU/CPU equalizer: video encoding and AI analysis scale to hardware
7. Open DCP/MXF format support replacing proprietary media asset management
8. Offline content delivery: local CDN mirror for on-set distribution

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_plex_media_server.spec` or `go build -o plex_media_server`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |