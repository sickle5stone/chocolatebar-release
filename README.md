# ChocolateBar — Issue Tracker

> See the menu bar icons your notch is hiding.

**ChocolateBar** is a native macOS utility that adds a second row below your menu bar. The icons macOS pushes behind the notch show up there — and so do your open application windows. Click one and the real thing opens.

🌐 **Get ChocolateBar**: [chocolatebar.app](https://chocolatebar.app) — this is the only place to download.
💬 **Report a bug or request a feature**: [open an issue](https://github.com/sickle5stone/chocolatebar-release/issues/new/choose)
📧 **Private support / licensing**: [support@chocolatebar.app](mailto:support@chocolatebar.app)

> **About this repository**
> This repo is the **public issue tracker** for ChocolateBar. It contains no source code and no downloadable binaries. ChocolateBar is closed-source commercial software; the codebase is private. The app itself is distributed exclusively from [chocolatebar.app](https://chocolatebar.app).

---

## What ChocolateBar does

- **Hidden icons, surfaced.** A second row beneath your menu bar that never hides. Every status item, in one glance.
- **Open windows, one click.** Active application windows live in the same strip. No Cmd-Tab roulette, no Dock detour.
- **Click to activate.** Clicking an icon triggers the real menu bar item via the macOS Accessibility API. No shims.
- **Zero configuration.** Auto-detects new menu bar items and windows the moment apps add them. Install, grant, done.

## System requirements

| | |
|---|---|
| **macOS** | 13 Ventura — 15 Sequoia |
| **Architecture** | Apple Silicon (M1, M2, M3, M4 — including Pro & Max) |
| **Download size** | ~5 MB |
| **Memory** | < 30 MB at idle |
| **Permissions** | Accessibility (required to read other apps' menu bar items) |

## Install

Download ChocolateBar from [chocolatebar.app](https://chocolatebar.app). After the DMG downloads:

1. Double-click the DMG to mount it.
2. Drag **ChocolateBar.app** to your Applications folder.
3. Launch ChocolateBar.
4. Grant Accessibility permission when prompted — this is how the app reads and clicks your existing menu bar items.

## Uninstall

Open **ChocolateBar → Settings → General → Permissions** and click **Reset & quit**. That clears the Accessibility entry cleanly. Then drag ChocolateBar from Applications to the Trash.

If you skipped that step and the entry is stuck in System Settings, run:

```bash
tccutil reset Accessibility com.aloysius.chocolatebar
```

## Reporting issues

Found a bug, an app that doesn't render correctly in the strip, or have a feature idea? **Open an issue** using one of the templates:

- 🐛 [**Bug report**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=bug_report.yml) — something broken or misbehaving.
- 💡 [**Feature request**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=feature_request.yml) — something you wish ChocolateBar did.
- 🧩 [**App compatibility**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=app_compatibility.yml) — a specific app's icon doesn't render or click correctly.

The templates ask for your macOS version, chip, and the app(s) involved — please fill them in; it makes the bug fixable in one round instead of three.

## Privacy

ChocolateBar runs entirely on your Mac. No telemetry, no analytics, no network calls except to check for updates. The Accessibility API is used only to enumerate menu bar items and active windows on your own machine, and to click them when you ask.

## Refund policy

14 days, no forms. Email [support@chocolatebar.app](mailto:support@chocolatebar.app) and you'll get a refund the same day.

## License

ChocolateBar is commercial software. The source code is private. This repository exists solely for public issue tracking — it does not contain source or binaries.

Copyright © 2026 Aloysius Lim. All rights reserved.
