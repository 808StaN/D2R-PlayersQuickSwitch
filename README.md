# D2R QuickSwitch

A [D2RMM](https://www.nexusmods.com/diablo2resurrected/mods/169) mod that lets you send `/players 1–8` commands in Diablo II: Resurrected with a single key press — **no AutoHotkey or any additional software required**.

## How it works

After installing the mod via D2RMM, two files are generated in your D2R directory:

- `QuickSwitch.ps1` — a PowerShell script that registers global hotkeys and sends the appropriate `/players X` command whenever D2R is in the foreground.
- `QuickSwitch.bat` — a launcher that starts the script in a hidden window.

The script automatically waits for D2R to launch and exits when the game is closed.

## Setup

1. Install the mod via **D2RMM** and configure your key bindings.
2. Run **`QuickSwitch.bat`** once before starting a D2R session.
3. Press your configured key in-game to switch `/players` count instantly.

## Configuration (D2RMM)

| Option | Default | Description |
|---|---|---|
| Key for /players 1 | F1 | Key that sends `/players 1` |
| Key for /players 2 | F2 | Key that sends `/players 2` |
| Key for /players 3 | F3 | Key that sends `/players 3` |
| Key for /players 4 | F4 | Key that sends `/players 4` |
| Key for /players 5 | F5 | Key that sends `/players 5` |
| Key for /players 6 | F6 | Key that sends `/players 6` |
| Key for /players 7 | F7 | Key that sends `/players 7` |
| Key for /players 8 | F8 | Key that sends `/players 8` |
| Tooltip duration (ms) | 1500 | How long the notification is shown. 0 = disabled. |
| Chat open delay (ms) | 100 | Delay between opening chat and typing. Increase if commands are missed. |

Each key can be set to **Disabled** or any **F1–F12** key. Duplicate key assignments are detected and reported as an error in D2RMM.

## Requirements

- Windows 10/11 (PowerShell 5+ built-in)
- [D2RMM](https://www.nexusmods.com/diablo2resurrected/mods/169)

## Author

808StaN
