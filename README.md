# Atlas MUD Client

Atlas is a customizable Windows MUD client for Discworld and other MUD servers, with dark and light themes, layouts for Full HD/QHD/4K displays, saved server profiles, a live map, optional Mudlet scripting packages, a local voice reader, and Windows voice input.

## Download and install

- [Latest Windows release](https://github.com/NSCx/atlas-mud-downloads/releases/latest)
- [Download Atlas 1.5.3 installer (Windows x64)](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.3/Atlas-MUD-Setup-1.5.3-x64.exe)
- [SHA-256 checksum](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.3/Atlas-MUD-Setup-1.5.3-x64.exe.sha256)

Download the `.exe`, run it, and follow the installer steps. Installing over an earlier Atlas version preserves your profile. In Atlas, select your MUD server or add a custom server, then connect.

The current installer is unsigned. Automatic updates are not enabled in version 1.5.3; download later versions from this release page. Mudlet package support covers core scripting features and does not include complete GUI or mapper compatibility.

Version 1.5.3 shows cleaned commands immediately. Windows dictates into a separate speech draft while the game command box above shows the full command: “S” or “type south” becomes “south”. Standalone N/S/E/W and diagonal abbreviations become full directions, with U/D and in/out also supported. Common commands such as L, I, “look around”, and “who is online” are cleaned into game commands. “Type” is removed only before recognized directions or built-in command verbs. Speech never sends commands automatically; review the command above, then press Enter.

For Windows Voice Access, click **Voice draft** and dictate into its focused field. The full command appears above, and Enter sends it; the draft stays available for the next command. **Close voice draft**, Stop, and Escape close Atlas's draft only. Use Voice Access's own microphone control to stop its listening.

Click the microphone or press **Ctrl+Shift+M** to dictate; click again or use **Stop dictation** to close its session. If Atlas cannot confirm closure of the Windows popup, it keeps the active indicator and asks you to close the popup with its X button. Windows voice typing may use Microsoft’s online speech service; Atlas does not save recordings or send audio to its own service.

Open **Settings → Voice input** for recognition detection, refresh, and Windows language, microphone, and voice-access settings. Atlas-managed dictation cancels on Escape, leaving Play, private input, sending a command, or losing focus. Confirm the Windows voice typing panel has closed before entering passwords or leaving Play. Losing focus keeps the Windows dictation session marked active, so Stop dictation remains available. **Clean dictation** tidies complete direction phrases and line breaks without sending commands.

Targets and player-name casing are preserved, along with chat punctuation: “tell Bob N.” stays a message. Unknown commands pass through to normal aliases and Lua processing without guesses. Atlas's /clear, /help, /stop, /walk, and /demo retain their existing local behavior. Ordinary keyboard commands and private input bypass speech cleanup. Manual command edits are preserved, and oversized dictation is rejected rather than truncated. Recognition quality depends on Windows and your microphone; each MUD defines its own vocabulary.

World atlas still supports drag-to-pan, arrow-key panning, and centering your current room. Recent terminal output, chat, and session logs use size limits to reduce memory growth during long sessions; export logs during play to keep older output.

## Verify the download

In PowerShell, run this command in the folder containing the downloaded installer:

```powershell
Get-FileHash .\Atlas-MUD-Setup-1.5.3-x64.exe -Algorithm SHA256
```

Compare the result with the downloaded `.sha256` file. The expected SHA-256 for version 1.5.3 is:

```text
a72d0261652aec1b5cc6b1d205fbe23dc35fff181bcada6af63a286fb96422dc
```

## About this repository

This public repository contains download documentation and binary releases. Application source and development history are maintained privately. GitHub's automatically generated **Source code (zip)** and **Source code (tar.gz)** downloads contain this documentation only; use the `.exe` asset to install Atlas.
