# Gary AI DVM — Autonomous Nostr Data Vending Machine

An AI-powered Data Vending Machine (NIP-90) that runs autonomously via GitHub Actions.

## What it does

- Scans Nostr relays every 15 minutes for DVM job requests
- Processes text summarization, analysis, and generation jobs
- Publishes results back to Nostr
- Accepts Lightning micropayments via LNbits

## How it works

This is a serverless DVM — it runs as a GitHub Actions workflow on a cron schedule. No VPS or always-on server needed.

### Supported job kinds:
- **5001**: Text summarization
- **5050**: Text generation
- **5100**: Analysis

## Setup

1. Fork this repo
2. Add your Nostr private key as a GitHub Secret (`NOSTR_SK_HEX`)
3. Add LNbits credentials as secrets
4. Enable GitHub Actions
5. The DVM will start scanning and responding to jobs automatically

## Lightning Tips

If you find this useful: `gary-ai@demo.lnbits.com`

## License

MIT
