# Command Line Interface — PLEX_MEDIA_SERVER

**Upstream:** https://github.com/nicedoc/Plex-Media-Server

## Anticloud CLI

```bash
# Install
pip install anticloud-plex-media-server

# Run offline with PAX inference
anticloud-plex-media-server --offline --pax-local

# Run with AIOSS logging
anticloud-plex-media-server --aioss-log ./ledger.jsonl

# Single binary (after build)
./plex_media_server --config config.yaml
```

## Options

| Flag | Description |
| --- | --- |
| `--offline` | Disable all network calls |
| `--pax-local` | Use local PAX inference at 127.0.0.1:11434 |
| `--aioss-log PATH` | Write AIOSS audit chain to PATH |
| `--encrypt` | Enable AES-256 at rest for output files |
| `--gpu` | Force GPU inference |
| `--cpu` | Force CPU inference |
| `--config PATH` | Load configuration from YAML file |
