# Atlas MUD Client

Atlas is a customizable Windows MUD client for Discworld and other MUD servers, with dark and light themes, layouts for Full HD/QHD/4K displays, saved server profiles, a live map, optional Mudlet scripting packages, a local voice reader, and Windows voice input.

## Download and install

- [Latest Windows release](https://github.com/NSCx/atlas-mud-downloads/releases/latest)
- [Download Atlas 1.5.2 installer (Windows x64)](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.2/Atlas-MUD-Setup-1.5.2-x64.exe)
- [SHA-256 checksum](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.2/Atlas-MUD-Setup-1.5.2-x64.exe.sha256)

Download the `.exe`, run it, and follow the installer steps. Installing over an earlier Atlas version preserves your profile. In Atlas, select your MUD server or add a custom server, then connect.

The current installer is unsigned. Automatic updates are not enabled in version 1.5.2; download later versions from this release page. Mudlet package support covers core scripting features and does not include complete GUI or mapper compatibility.

Version 1.5.2 improves spoken command handling. Standalone N/S/E/W and diagonal abbreviations become full directions, with U/D and in/out also supported. Common commands such as L, I, “look around”, and “who is online” are cleaned into game commands. Windows voice typing shows a preview and applies cleanup when dictation stops or you press Enter; compatible native recognition cleans the command draft immediately. Speech never sends commands automatically.

Click the microphone or press **Ctrl+Shift+M** to dictate; click again or use **Stop dictation** to close its session. If Atlas cannot confirm closure of the Windows popup, it keeps the active indicator and asks you to close the popup with its X button. Windows voice typing may use Microsoft’s online speech service; Atlas does not save recordings or send audio to its own service.

Open **Settings → Voice input** for recognition detection, refresh, and Windows language, microphone, and voice-access settings. Atlas-managed dictation cancels on Escape, leaving Play, private input, sending a command, or losing focus. Confirm the Windows voice typing panel has closed before entering passwords or leaving Play. Losing focus keeps the Windows dictation session marked active, so Stop dictation remains available. **Clean dictation** tidies complete direction phrases and line breaks without sending commands.

Targets and player-name casing are preserved, along with chat punctuation: “tell Bob N.” stays a message. Unknown commands pass through to normal aliases and Lua processing without guesses. Ordinary keyboard commands and private input bypass speech cleanup. Oversized dictation is rejected rather than truncated. Review the draft before Enter; each MUD defines its own vocabulary.

World atlas still supports drag-to-pan, arrow-key panning, and centering your current room. Recent terminal output, chat, and session logs use size limits to reduce memory growth during long sessions; export logs during play to keep older output.

## Verify the download

In PowerShell, run this command in the folder containing the downloaded installer:

```powershell
Get-FileHash .\Atlas-MUD-Setup-1.5.2-x64.exe -Algorithm SHA256
```

Compare the result with the downloaded `.sha256` file. The expected SHA-256 for version 1.5.2 is:

```text
1702745134b7bcc50599581ef59819b7c7eba13e25c6e629fdbbb6fbde2f325c
```

## About this repository

This public repository contains download documentation and binary releases. Application source and development history are maintained privately. GitHub's automatically generated **Source code (zip)** and **Source code (tar.gz)** downloads contain this documentation only; use the `.exe` asset to install Atlas.
