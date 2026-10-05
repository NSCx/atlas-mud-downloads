# Atlas MUD Client

Atlas is a customizable Windows MUD client for Discworld and other MUD servers, with dark and light themes, layouts for Full HD/QHD/4K displays, saved server profiles, a live map, optional Mudlet scripting packages, and a local voice reader.

## Download and install

- [Latest Windows release](https://github.com/NSCx/atlas-mud-downloads/releases/latest)
- [Download Atlas 1.4.2 installer (Windows x64)](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.4.2/Atlas-MUD-Setup-1.4.2-x64.exe)
- [SHA-256 checksum](https://github.com/NSCx/atlas-mud-downloads/releases/download/v1.4.2/Atlas-MUD-Setup-1.4.2-x64.exe.sha256)

Download the `.exe`, run it, and follow the installer steps. Installing over an earlier Atlas version preserves your profile. In Atlas, select your MUD server or add a custom server, then connect.

The current installer is unsigned. Automatic updates are not enabled in version 1.4.2; download later versions from this release page. Mudlet package support covers core scripting features and does not include complete GUI or mapper compatibility.

Version 1.4.2 adds drag-to-pan in **World atlas**, arrow-key panning, and a button to center your current room. Zoom preserves your viewed position. Recent terminal output, chat, and session logs use size limits to reduce memory growth during long sessions; export logs during play to keep older output.

## Verify the download

In PowerShell, run this command in the folder containing the downloaded installer:

```powershell
Get-FileHash .\Atlas-MUD-Setup-1.4.2-x64.exe -Algorithm SHA256
```

Compare the result with the downloaded `.sha256` file. The expected SHA-256 for version 1.4.2 is:

```text
1d853bde9ed5754340f4bddd9bd6e5b66da660fe0c02423530e92cf813a3a8b2
```

## About this repository

This public repository contains download documentation and binary releases. Application source and development history are maintained privately. GitHub's automatically generated **Source code (zip)** and **Source code (tar.gz)** downloads contain this documentation only; use the `.exe` asset to install Atlas.
