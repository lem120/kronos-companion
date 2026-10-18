# Kronos Companion 1.1.0

Community integration for **Kronos 2017 v1.49** and **Bitfocus Companion 5.1+**.

Kronos Companion brings the Kronos countdown timer list into Companion through a local bridge designed for live-production workflows.

> **Kronos Companion is free and community-built.**  
> If it saves you time on show day, you can support its continued development on [Buy Me a Coffee](https://buymeacoffee.com/wario_bruno).

## Features

- Dynamic Kronos timer list
- Timer names and live `MM:SS` countdown values
- Play / Pause / Reset controls
- Live/Broadcast button feedback
- Overtime display without milliseconds
- **Follow Kronos Order**
- Legacy Fixed ID mode
- Automatic Kronos database discovery on macOS and Windows
- Installer backup and rollback

## Requirements

- A working, legally obtained installation of **Kronos 2017 v1.49**
- **Bitfocus Companion 5.1+**
- macOS or Windows

Kronos itself is **not included** in this distribution.

## Installation

1. Download `Kronos_Companion_1.1.0_Windows.zip` or `Kronos_Companion_1.1.0_macOS.zip` from the v1.1.0 release.
2. Extract the complete archive.
3. Run `INSTALL_KRONOS_COMPANION`.
4. The installer verifies the supported Kronos build, creates a backup and applies the bridge patch locally.
5. Import `Kronos_Companion_Module_1.1.0.tgz` in Companion.
6. Configure the connection with host `127.0.0.1`, port `18749`, and leave the database field empty for auto-discovery.

## Recommended timer mode

Use **Timers · Follow Kronos Order**. Each Companion cell represents a position in the Kronos list. Reordering timers in Kronos automatically updates the name, time, state and timer controlled by that Companion cell.

## Rollback

Both platform packages include a rollback script. The installer creates a backup before modifying the local Kronos installation.

## Public distribution model

The installer does **not** ship the Kronos application or a complete modified `Kronos2017.swf`. It verifies a supported existing installation and applies the Kronos Companion bridge patch locally.

## Support the project

Kronos Companion is free to use and developed as an independent community project.

If it helps your live-production workflow, you can support continued development and maintenance on **[Buy Me a Coffee](https://buymeacoffee.com/wario_bruno)**.

Support is entirely optional and does not unlock additional features or downloads.

## Disclaimer

Kronos Companion is an independent community project. It is not affiliated with, endorsed by, or sponsored by Manythink or Bitfocus. Kronos and other third-party product names are the property of their respective owners.
