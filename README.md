# Atlas MUD Client

Atlas is a customizable Windows MUD client for Discworld and other MUD servers, with dark and light themes, layouts for Full HD/QHD/4K displays, saved server profiles, a live map, optional Mudlet scripting packages, a local voice reader, and Windows voice input.

## Download and install

- [Latest Windows release](https://github.com/NSCx/atlas-mud-downloads/releases/latest)
- [Download Atlas 1.5.0 installer (Windows x64)](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.0/Atlas-MUD-Setup-1.5.0-x64.exe)
- [SHA-256 checksum](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.5.0/Atlas-MUD-Setup-1.5.0-x64.exe.sha256)

Download the `.exe`, run it, and follow the installer steps. Installing over an earlier Atlas version preserves your profile. In Atlas, select your MUD server or add a custom server, then connect.

The current installer is unsigned. Automatic updates are not enabled in version 1.5.0; download later versions from this release page. Mudlet package support covers core scripting features and does not include complete GUI or mapper compatibility.

Version 1.5.0 adds a microphone button beside the command box and **Ctrl+Shift+M** for Windows voice input. Review the dictated command and press Enter to send it. Compatible installed Windows recognition engines provide one-phrase dictation; otherwise Atlas opens Windows voice typing with **Win+H**. The Windows panel controls its own microphone and privacy settings. Windows voice typing may use Microsoft's online speech service. Atlas does not record audio or send it to its own service, and no third-party recognition model is bundled.

Open **Settings → Voice input** for recognition detection, refresh, and Windows language, microphone, and voice-access settings. Atlas-managed dictation cancels on Escape, leaving Play, private input, sending a command, or losing focus. Close the Windows voice typing panel before entering passwords or leaving Play. **Clean dictation** tidies complete direction phrases and line breaks without sending commands.

World atlas still supports drag-to-pan, arrow-key panning, and centering your current room. Recent terminal output, chat, and session logs use size limits to reduce memory growth during long sessions; export logs during play to keep older output.

## Verify the download

In PowerShell, run this command in the folder containing the downloaded installer:

```powershell
Get-FileHash .\Atlas-MUD-Setup-1.5.0-x64.exe -Algorithm SHA256
```

Compare the result with the downloaded `.sha256` file. The expected SHA-256 for version 1.5.0 is:

```text
108bc6886c140997cb6363f30403f4036047a326789c2ae5fbf15103d2bd7b78
```

## About this repository

This public repository contains download documentation and binary releases. Application source and development history are maintained privately. GitHub's automatically generated **Source code (zip)** and **Source code (tar.gz)** downloads contain this documentation only; use the `.exe` asset to install Atlas.
