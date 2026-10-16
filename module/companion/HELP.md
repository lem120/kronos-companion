# Kronos Companion 1.1.0

Stable integration for controlling **Kronos 2017 countdown timers** from Bitfocus Companion.

## Features

- Dynamic timer list read from Kronos.
- Timer presets show the Kronos displayed name and remaining time in `MM:SS`.
- Stable timer identity while the Kronos list changes.
- Timer preset press = select + Play/Resume.
- Generic **PLAY**, **PAUSE** and **RESET** controls for the selected timer.
- Live/Broadcast feedback: dark stopped, blue selected, green running, amber paused, red overtime.
- Overtime formatting without decimal milliseconds.
- Automatic Kronos database discovery on macOS and Windows.
- **Follow Kronos Order** presets for position-based Companion layouts.
- Legacy **Fixed ID** presets remain available when a fixed timer identity is preferred.

## Requirements

- Kronos 2017 v1.49 with the Kronos Companion Bridge installed.
- Bitfocus Companion 5.1 or newer, compatible with runtime `node26` and API `2.2.0`.
- Kronos and Companion on the same computer when using automatic database discovery.

## Connection

- **Host:** `127.0.0.1`
- **HTTP port:** `18749`
- **Kronos database:** leave empty for auto-discovery.

The module searches the supported Kronos application-data locations on both macOS and Windows, including legacy bridge locations when present.

## Recommended mode — Follow Kronos Order

Use the presets under **Timers · Follow Kronos Order**.

Each placed Companion button represents a position in the Kronos timer list rather than a permanently fixed timer ID. If the list is reordered in Kronos, the same Companion cell automatically updates its timer name, remaining time, state and controlled timer.

Buttons created with older releases remain Fixed ID buttons. Replace them with the Follow Kronos Order presets if you want position-following behaviour.

## Bridge API

- `GET /health`
- `GET /status`
- `POST /timer/<position>/play`
- `POST /timer/<position>/pause`
- `POST /timer/<position>/stop`
- `POST /timer/<position>/reset`

POST requests use the header `X-Kronos-Bridge: 1`.

## Project status

Version **1.1.0** is the stable release baseline for timer control, dynamic names, database auto-discovery and Follow Kronos Order.
