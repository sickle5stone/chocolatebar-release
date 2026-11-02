# ChocolateBar: menu bar manager for Mac with a second row

> Let your notch eat no more!

**ChocolateBar** is a native menu bar manager for Mac. It can hide menu bar icons, and it can show them full size in a second row below the menu bar, including the icons a MacBook Pro notch hides. Press ⇧⌘B, or click the ChocolateBar menu bar icon, to open the row. Click an icon and that app's real menu opens. Works with or without a notch.

- **macOS 12 Monterey, 13 Ventura, 14 Sonoma and 15 Sequoia.** macOS 26 Tahoe support coming soon.
- **Apple Silicon and Intel.** Universal binary, so an Intel Mac does not need Rosetta.
- **Accessibility only.** ChocolateBar never asks for Screen Recording permission.
- **$15 USD one-time.** 48-hour free trial, full features, no card.

🌐 **Get ChocolateBar**: [chocolatebar.app](https://chocolatebar.app). This is the only place to download.
💬 **Report a bug or request a feature**: [open an issue](https://github.com/sickle5stone/chocolatebar-release/issues/new/choose)
📧 **Private support / licensing**: [support@chocolatebar.app](mailto:support@chocolatebar.app)

> **About this repository**
> This repo is the **public issue tracker** for ChocolateBar. It contains no source code and no downloadable binaries. ChocolateBar is closed-source commercial software; the codebase is private. The app itself is distributed exclusively from [chocolatebar.app](https://chocolatebar.app).

---

## Who it's for

- **14-inch and 16-inch MacBook Pro owners** whose menu bar icons disappear behind the camera notch. macOS 12 to 15 has no built-in second row; ChocolateBar adds one.
- **iMac, Mac mini, MacBook Air and external-display users** whose menu bar has too many icons, with or without a notch.
- **Work Macs** where the VPN, security and chat icons IT installed cannot be removed. Hide them, or move them to the row.

## What ChocolateBar does

- **Hide menu bar icons.** **Enable Hide Menubar Items** (Settings → General, off by default) hides the icons left of the | divider, so the menu bar stays clean. Apple's own system icons are optional and off by default.
- **Show them in a second row.** The row opens when you press ⇧⌘B or click the ChocolateBar menu bar icon. Every menu bar app shows at full size, including the ones behind the notch. Auto-hide is optional and off by default.
- **Real menus.** Click an icon and you get that app's real menu, via the macOS Accessibility API. No fake menus.
- **Mirror by default.** Without hiding, icons stay in the menu bar and also show in the row.
- **Where it sits.** Pin the row to the top or bottom, on the left, middle, or right, and nudge it with the offset sliders.
- **Profiles.** Save a settings snapshot (layout, density, theme, hidden icons, order, position, auto-hide, custom icons) and switch in one click. Profiles don't launch apps.
- **Running apps, optional.** ChocolateBar can show running apps, one chip per app. This is off by default: Settings → General → **Show running apps**, or press ⌃⌘S.

## System requirements

| | |
|---|---|
| **macOS** | macOS 12 Monterey to 15 Sequoia · macOS 26 Tahoe support coming soon |
| **Architecture** | Universal binary: Apple Silicon and Intel |
| **Download size** | ~5 MB (native Swift, no Electron) |
| **Memory** | About 30 MB at launch |
| **Permissions** | Accessibility only (required to read and click other apps' menu bar items). Never Screen Recording. |

## Pricing

**$15 USD, one-time.** No subscription. Includes 1 year of updates; the app keeps working after that. Use it on every Mac you own. 7-day refund, no forms.

48-hour free trial, full features, no card needed.

Licenses bought before 0.6.0 (16 Oct 2026) keep lifetime updates. Licenses from 0.6.0 include one year of updates.

## Install

Download ChocolateBar from [chocolatebar.app](https://chocolatebar.app). After the DMG downloads:

1. Double-click the DMG to mount it.
2. Drag **ChocolateBar.app** to your Applications folder.
3. Launch ChocolateBar.
4. Grant Accessibility permission when prompted. This is how the app reads and clicks your existing menu bar items.

If macOS says the app can't be checked for malicious software, right-click ChocolateBar in Applications, choose **Open**, then click **Open** again.

## Uninstall

Open **ChocolateBar → Settings → General → Permissions** and click **Reset & quit**. That clears the Accessibility entry cleanly. Then drag ChocolateBar from Applications to the Trash.

If you skipped that step and the entry is stuck in System Settings, run:

```bash
tccutil reset Accessibility app.chocolatebar.chocolatebar
```

## Reporting issues

Found a bug, an app that doesn't render correctly in the strip, or have a feature idea? **Open an issue** using one of the templates:

- 🐛 [**Bug report**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=bug_report.yml): something broken or misbehaving.
- 💡 [**Feature request**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=feature_request.yml): something you wish ChocolateBar did.
- 🧩 [**App compatibility**](https://github.com/sickle5stone/chocolatebar-release/issues/new?template=app_compatibility.yml): a specific app's icon doesn't render or click correctly.

The templates ask for your macOS version, chip, and the app(s) involved. Please fill them in; it makes the bug fixable in one round instead of three.

## Privacy

ChocolateBar runs on your Mac. No telemetry. It never requests Screen Recording permission. Licensed users check `version.json` when they click to check for updates, or once a day if **Notify me** is on (off by default). Clicking Download requests `/update-check`. The Accessibility API is used only to list menu bar items on your own machine, and to click them when you ask.

## License

ChocolateBar is commercial software. The source code is private. This repository exists solely for public issue tracking. It does not contain source or binaries.

Copyright © 2026 Aloysius Lim. All rights reserved.
