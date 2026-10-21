# Rapidcut

**Convert raw phone footage into lightweight proxy files for lag-free editing.**

🌐 **Website & download:** [rapidcut.vercel.app](https://rapidcut.vercel.app)
⬇️ **Download for Windows:** [Rapidcut-Setup-1.0.4.exe](https://github.com/OscarWhiteman/rapidcut-releases/releases/download/v1.0.4/Rapidcut-Setup-1.0.4.exe) · [all releases](https://github.com/OscarWhiteman/rapidcut-releases/releases)

---

## Screenshots

<!-- TODO: add screenshots, e.g. ![Main window](screenshots/main.png) -->
_Screenshots coming soon._

## Key features

- **One-click proxy generation.** Turns heavy phone footage (HEVC, high-bitrate, variable frame rate) into smooth, edit-friendly proxy files.
- **Built for NLE workflows.** Proxies drop straight into DaVinci Resolve and Premiere Pro.
- **Batch queue.** Add many clips at once and let Rapidcut work through them.
- **Conversion history and settings.** See what you've converted and adjust output to suit your workflow.
- **Free tier plus Pro subscription.** Free monthly conversions with no account needed to download; Pro unlocks unlimited conversions.
- **Native Windows desktop app** with a custom title bar and dark UI.

## Tech stack

| Area | Technology |
|---|---|
| Desktop shell | **Electron** (v28) |
| Video processing | **FFmpeg** via `fluent-ffmpeg`, `ffmpeg-static`, `ffprobe-static` |
| Accounts & data | **Supabase** (Postgres + Edge Functions) |
| Payments | **Stripe** (hosted Checkout, subscription webhooks via a Supabase Edge Function) |
| Packaging | electron-builder (NSIS installer) |
| Landing page | Static site on Vercel |

## Installation

1. Download [Rapidcut-Setup-1.0.4.exe](https://github.com/OscarWhiteman/rapidcut-releases/releases/download/v1.0.4/Rapidcut-Setup-1.0.4.exe) (or the newest from [Releases](https://github.com/OscarWhiteman/rapidcut-releases/releases)).
2. Run the installer. Windows SmartScreen may warn because the app isn't code-signed yet: click **More info → Run anyway**.

## About the source code

Rapidcut is a commercial product, so its source code is kept in a private repository. This repo hosts only public release builds and documentation. If you're an employer or collaborator and want to see the code, get in touch and I'm happy to walk through it.
