# WolfDock

<p align="center"><img src="assets/wolfdock.png" width="144" alt="WolfDock blue wolf logo"></p>

WolfDock is the new name for MacDock. One Mac utility for Dock previews, window snapping, audio, clipboard, cleanup, mouse profiles and live monitoring, with an interactive blue wolf in Dynamic Island. A separate Windows preview brings the same visual direction and an initial set of desktop tools.

This public repository contains downloads and release notes. Application source development remains private.

## Downloads

| Platform | Download | Requirements |
| --- | --- | --- |
| macOS | [WolfDock 1.6.13](https://github.com/sSegara/WOLFDOCK-RELEASE/releases/tag/v1.6.13) | Apple silicon, macOS 26 or later |
| Windows preview | [WolfDock 0.1.1 for Windows](https://github.com/sSegara/WOLFDOCK-RELEASE/releases/tag/windows-v0.1.1) | Windows 10 22H2 / Windows 11, x64 |

[Latest stable Mac release](https://github.com/sSegara/WOLFDOCK-RELEASE/releases/latest) · [All releases](https://github.com/sSegara/WOLFDOCK-RELEASE/releases)

## Mac

The 1.6.13 update stabilizes compact wolf blinking and Dynamic Island dismissal, adds audio-reactive bars for the selected local player, keeps Focus/countdown clocks visible alongside music, and schedules completion notifications with sound. Finished indicators remain until acknowledged. Basic Spotify controls work without a Developer account; successful/pending command notices are removed and failures do not automatically open Spotify.

For a new installation, download **WolfDock-1.6.13.dmg** and copy WolfDock into Applications. The release channel is now **WOLFDOCK-RELEASE**. Versions through 1.6.12 require one manual replacement from this DMG because they validate the former channel name. From 1.6.13 onward, use **Check for updates → Update** in the app. Feature choices, mouse profiles and automation profiles retain the existing settings domain and original signing identity.

The **MacDock-1.6.13.dmg** asset supports older installed app names. Both DMGs contain the same signed app bytes. Choose the package matching the app name already present in Applications, then replace that application.

Spotify repeat confirmation can remain stale while its window is hidden; set repeat in the Spotify window in that case. The optional Spotify account connection is deferred. System notification appearance/sound depends on macOS settings and has not been directly observed in this release's testing; timer scheduling and persistent completion indicators were checked. Physical 120 Hz and MacBook-notch checks also remain pending.

Mac builds are locally signed and are not notarized. macOS may require **System Settings → Privacy & Security → Open Anyway** on the first launch. Later updates retain the original signing identity. Automatic update checks can be disabled in the Updates page; installation begins only after choosing Update.

## Windows preview

Extract **WolfDock-Windows-0.1.1-x64.zip** and run **WolfDock.exe**. The .NET runtime is included; administrator access is not requested. Closing the main window keeps WolfDock in the system tray. Click the wolf for the blue quick panel with CPU/RAM and favorites; choose **Buka WolfDock** to restore the main window. Right-click retains the native menu. To update an older preview, exit it through its tray menu before launching the new version; the saved profile is retained.

Included: live CPU/RAM and volume usage, Keep Awake, keyboard window snapping, music/video Dynamic Island, countdown, notes, local clipboard history, tray favorites, folder analysis and reviewed duplicate cleanup through Recycle Bin. Settings are stored separately at `%LOCALAPPDATA%\WolfDock\settings.json`.

The 0.1.1 update also removes repeated interface text, restores minimized windows and saves pending note edits before searching.

![WolfDock Windows interface rendered in headless UI tests](assets/windows-preview.png)

![WolfDock Windows quick panel rendered in headless UI tests](assets/windows-quick-panel.png)

This is an early preview: 314 source/headless checks pass, including 36 page/size combinations, but native Windows integrations still need testing on a Windows PC. The executable is not Authenticode signed. Windows automatic updates, per-device mouse profiles, temperature/SMART sensors, disk benchmarking, lyrics/weather and other Mac-only tools are still pending. The release notes list the current limits.

## Checksums

Each download includes a SHA-256 checksum file. Verify the downloaded ZIP or DMG against its matching checksum before manual installation.
