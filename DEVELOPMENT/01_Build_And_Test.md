# Build and Test

**Project:** `PLEX_MEDIA_SERVER`
**Upstream:** https://github.com/nicedoc/Plex-Media-Server
**License:** GPL

## Quick Start

```bash
git clone https://github.com/nicedoc/Plex-Media-Server
cd Plex-Media-Server
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local script analysis, scene breakdown, and subtitles
2. AIOSS provenance chain for all production assets (C2PA aligned)
3. AES-256 encryption for pre-release content and DCP masters
4. Single-binary media management tool with no cloud dependency
5. Zero-cloud: all AI analysis, transcription, and subtitling run locally
6. GPU/CPU equalizer: video encoding and AI analysis scale to hardware
7. Open DCP/MXF format support replacing proprietary media asset management
8. Offline content delivery: local CDN mirror for on-set distribution

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
