# SoTranscribe — sotranscribe.com

Sovereign transcription. Self-host or hosted on Austrian and Swiss servers — outside U.S. CLOUD Act reach.

The first product of **SoTranscribe GmbH (in Gründung)**, a Vienna-based startup spun out of [idea2.life](https://idea2.life) within the [EvoBioSys](https://evobiosys.org) network.

## What lives in this repo

This is the **marketing site** at https://sotranscribe.com. The actual SoTranscribe product source (Whisper Large v3 + pyannote pipeline, Rust backend, React frontend) will live in a separate `evobiosys/sotranscribe-app` repo — coming once the hosted tier launches.

```
.
├── CNAME              sotranscribe.com
├── _config.yml        Jekyll passthrough
├── index.html         hero + value prop + 3 promises + how it works + pricing + FAQ
├── about.html         founders, lineage, mission
├── advanced.html      technical write-up — pipeline, jurisdiction, hardware research
├── imprint.html       legal notice (EU mandatory)
├── privacy.html       GDPR-compliant privacy notice
└── assets/
    ├── css/sotranscribe.css
    └── img/sotranscribe/{logo.svg, favicon.svg, favicon.ico, og.png}
```

## Local preview

```sh
cd /root/projects/sotranscribe && python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

GitHub Pages auto-builds on push to `main`. CNAME is wired to `sotranscribe.com` via Infomaniak DNS.

## License

Site content © 2026 SoTranscribe GmbH (in Gründung). The eventual SoTranscribe product source code will be published under the [EvoBioSys License](https://github.com/evobiosys/license).
