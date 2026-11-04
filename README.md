# WolfDock

<p align="center"><img src="assets/wolfdock.png" width="144" alt="WolfDock blue wolf logo"></p>

WolfDock is the new name for MacDock. One Mac utility for Dock previews, window snapping, audio, clipboard, cleanup, mouse profiles and live monitoring, with an interactive blue wolf in Dynamic Island. A separate Windows preview brings the same visual direction and an initial set of desktop tools.

This public repository contains downloads and release notes. Application source development remains private.

## Downloads

| Platform | Download | Requirements |
| --- | --- | --- |
| macOS | [WolfDock 1.6.8](https://github.com/sSegara/MacDock-Releases/releases/tag/v1.6.8) | Apple silicon, macOS 26 or later |
| Windows preview | [WolfDock 0.1.0 for Windows](https://github.com/sSegara/MacDock-Releases/releases/tag/windows-v0.1.0) | Windows 10 22H2 / Windows 11, x64 |

[Latest stable Mac release](https://github.com/sSegara/MacDock-Releases/releases/latest) · [All releases](https://github.com/sSegara/MacDock-Releases/releases)

## Mac

The 1.6.8 update introduces WolfDock branding, a dark blue main interface, grouped navigation, accessible blue switches, a responsive Cleanup page and a menu that fits its favorites. The compact wolf uses a lower animation rate and resumes pointer tracking when the Island opens.

For a new installation, download **WolfDock-1.6.8.dmg** and copy WolfDock into Applications. Existing MacDock/WolfDock installations can choose **Check for updates → Update** in the app. Feature choices, mouse profiles and automation profiles stay in the existing settings domain. Release checksums and the original MacDock signing identity are verified before replacement.

The **MacDock-1.6.8.dmg** asset provides compatibility with older app names and updaters. Both DMGs contain the same signed app bytes. For manual replacement, choose the package matching the name already installed in Applications. Users of 1.6.3/1.6.4 need this manual replacement once, because those versions have an older update helper; versions from 1.6.5 use the corrected helper.

Mac builds are locally signed and are not notarized. macOS may require **System Settings → Privacy & Security → Open Anyway** on the first launch. Later updates retain the original signing identity. Automatic update checks can be disabled in the Updates page; installation begins only after choosing Update.

## Windows preview

Extract **WolfDock-Windows-0.1.0-x64.zip** and run **WolfDock.exe**. The .NET runtime is included; administrator access is not requested. Closing the main window keeps WolfDock in the system tray. Use the wolf tray menu to reopen it or quit.

Included: live CPU/RAM and volume usage, Keep Awake, keyboard window snapping, music/video Dynamic Island, countdown, notes, local clipboard history, tray favorites, folder analysis and reviewed duplicate cleanup through Recycle Bin. Settings are stored separately at `%LOCALAPPDATA%\WolfDock\settings.json`.

![WolfDock Windows interface rendered in headless UI tests](assets/windows-preview.png)

This is an early preview: 174 source/headless checks pass, including 36 page/size combinations, but native Windows integrations still need testing on a Windows PC. The executable is not Authenticode signed. Windows automatic updates, per-device mouse profiles, temperature/SMART sensors, disk benchmarking, lyrics/weather and other Mac-only tools are still pending. The release notes list the current limits.

## Checksums

Each download includes a SHA-256 checksum file. Verify the downloaded ZIP or DMG against its matching checksum before manual installation.
