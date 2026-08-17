# Adwa Money Printer

AI short-video factory running on **free GitHub Actions runners**. Feed it a topic via Workflow Dispatch, it generates a complete HD short video (script via Gemini, voice via edge-tts, footage via Pexels) and hands you the MP4 as an artifact.

## How to use

1. In this repo, go to **Actions** → **MPT Video Factory** → **Run workflow**
2. Enter a **topic** (e.g. `5 surprising facts about space`)
3. Optionally set language (default `en-US`)
4. Run. When finished, the MP4 is under **Artifacts** → `generated-short`

## Required secrets

- `GEMINI_API_KEY` — Google AI Studio key (script generation)
- `PEXELS_API_KEY` — pexels.com key (stock footage)

Both free tiers. Set in Settings → Secrets and variables → Actions.

## Config
`config.toml` is generated from secrets at runtime. Full MPT config reference: https://github.com/harry0703/MoneyPrinterTurbo
