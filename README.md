# ChocolateBar — Issue Tracker

> A second row for your Mac menu bar. See every icon, switch windows, or hide the clutter.

**ChocolateBar** is a native macOS menu bar manager. It shows the menu bar icons your Mac hides (behind the notch or off a crowded bar), full size, in a second row below the menu bar, alongside your open app windows. Click one and the real thing opens. Prefer a clean bar? Hide mode tucks the clutter away instead.

🌐 **Get ChocolateBar**: [chocolatebar.app](https://chocolatebar.app) — this is the only place to download.
💬 **Report a bug or request a feature**: [open an issue](https://github.com/sickle5stone/chocolatebar-release/issues/new/choose)
📧 **Private support / licensing**: [support@chocolatebar.app](mailto:support@chocolatebar.app)

> **About this repository**
> This repo is the **public issue tracker** for ChocolateBar. It contains no source code and no downloadable binaries. ChocolateBar is closed-source commercial software; the codebase is private. The app itself is distributed exclusively from [chocolatebar.app](https://chocolatebar.app).

---

## What ChocolateBar does

- **A second row of full-size icons.** Everything macOS hid behind the notch or pushed off the bar, visible and clickable in a strip below the menu bar. Lay it out wide, or as a column down one side. Works with or without a notch.
- **Open windows, one click.** Your open app windows sit in the same strip. No Cmd-Tab roulette, no Dock detour.
- **Hide mode.** Rather keep the bar clean? Tuck third-party icons away and peek at them when you need them.
- **Real clicks, real menus.** Clicking an icon triggers the real menu bar item via the macOS Accessibility API.
- **Profiles.** Save different setups (for example work and home) and switch with a hotkey.
- **Zero configuration.** Auto-detects new menu bar items and windows the moment apps add them. Install, grant, done.
- **Private by design.** Accessibility permission only, never Screen Recording. No telemetry, no accounts.

## System requirements

| | |
|---|---|
| **macOS** | macOS 12 Monterey to 15 Sequoia · macOS 26 Tahoe support coming soon |
| **Architecture** | Universal binary: Apple Silicon and Intel |
| **Download size** | ~5 MB (native Swift, no Electron) |
| **Memory** | < 30 MB at idle |
| **Permissions** | Accessibility (required to read and click other apps' menu bar items) |

## Pricing

**$15 USD, one-time.** Includes 1 year of updates; the app keeps working after that. Use it on every Mac you own. 7-day refund, no forms.
<!-- {LAUNCH10} --> First 10 buyers pay $10 with code `LAUNCH10`.
<!-- {TRIAL} --> 48-hour free trial, full features, no card needed.

Licenses bought before one-year terms were introduced keep lifetime updates.

## Install

Download ChocolateBar from [chocolatebar.app](https://chocolatebar.app). After the DMG downloads:

1. Double-click the DMG to mount it.
2. Drag **ChocolateBar.app** to your Applications folder.
3. Launch ChocolateBar.
4. Grant Accessibility permission when prompted — this is how the app reads and clicks your existing menu bar items.

If macOS says the app can't be checked for malicious software, right-click ChocolateBar in Applications, choose **Open**, then click **Open** again.

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

ChocolateBar runs entirely on your Mac. No telemetry, no analytics, no accounts. It contacts chocolatebar.app only when you check for updates. The Accessibility API is used only to list menu bar items and open windows on your own machine, and to click them when you ask. ChocolateBar never requests Screen Recording permission.

## License

ChocolateBar is commercial software. The source code is private. This repository exists solely for public issue tracking — it does not contain source or binaries.

Copyright © 2026 Aloysius Lim. All rights reserved.
