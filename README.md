# ChocolateBar — Issue Tracker

> Every menu bar app in one row, one shortcut away.

**ChocolateBar** is a native macOS menu bar manager. Press ⇧⌘B, or click the ChocolateBar menu bar icon, and every menu bar app shows at full size in a row below the menu bar, including the ones behind the notch. Click one and that app's real menu opens. Works with or without a notch. Apple's system icons are optional.

🌐 **Get ChocolateBar**: [chocolatebar.app](https://chocolatebar.app) — this is the only place to download.
💬 **Report a bug or request a feature**: [open an issue](https://github.com/sickle5stone/chocolatebar-release/issues/new/choose)
📧 **Private support / licensing**: [support@chocolatebar.app](mailto:support@chocolatebar.app)

> **About this repository**
> This repo is the **public issue tracker** for ChocolateBar. It contains no source code and no downloadable binaries. ChocolateBar is closed-source commercial software; the codebase is private. The app itself is distributed exclusively from [chocolatebar.app](https://chocolatebar.app).

---

## What ChocolateBar does

- **Every menu bar app, one shortcut away.** The row opens when you press ⇧⌘B or click the ChocolateBar menu bar icon. Every menu bar app shows at full size, including the ones behind the notch. Apple's system icons are optional. Works with or without a notch. Auto-hide is optional and off by default.
- **Real menus.** Click an icon and you get that app's real menu, via the macOS Accessibility API.
- **Mirror by default.** Icons stay in the menu bar and also show in the row. **Enable Hide Menubar Items** (Settings → General, off by default) hides icons left of the | divider.
- **Where it sits.** Pin the row to the top or bottom, on the left, middle, or right, and nudge it with the offset sliders.
- **Profiles.** Save a settings snapshot (layout, density, theme, hidden icons, order, position, auto-hide, custom icons) and switch in one click. Profiles don't launch apps.
- **Running apps, optional.** ChocolateBar can show running apps, one chip per app. This is off by default: Settings → General → **Show running apps**, or press ⌃⌘S.

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

48-hour free trial, full features, no card needed.

Licenses bought before 0.6.0 (16 Oct 2026) keep lifetime updates. Licenses from 0.6.0 include one year of updates.

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

ChocolateBar runs on your Mac. No telemetry. It never requests Screen Recording permission. Licensed users check `version.json` when they click to check for updates, or once a day if **Notify me** is on (off by default). Clicking Download requests `/update-check`. The Accessibility API is used only to list menu bar items on your own machine, and to click them when you ask.

## License

ChocolateBar is commercial software. The source code is private. This repository exists solely for public issue tracking — it does not contain source or binaries.

Copyright © 2026 Aloysius Lim. All rights reserved.
