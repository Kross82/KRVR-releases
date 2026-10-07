# KRVR — PC VR streaming for Apple Vision Pro

KRVR streams your PC VR games to Apple Vision Pro over your home network. Eye-tracked foveated streaming, steady frame delivery, and head tracking that stays put.

**Get it:** [KRVR on the App Store](https://apps.apple.com/us/app/krvr/id6761065018) · [KRVR for Windows (free)](https://github.com/Kross82/KRVR-releases/releases/latest) · [Setup guide](https://krvr.app/setup.html) · [krvr.app](https://krvr.app)

## How it works

Native OpenXR games run through KRVR's own OpenXR runtime on the PC, with no SteamVR in the chain. Everything else runs through SteamVR with the KRVR driver. The headset side is the same either way.

1. **Install the server.** Download the latest `KRVR-Setup` installer from the [latest release](https://github.com/Kross82/KRVR-releases/releases/latest) and run it. Linux and SteamOS (testing): download the file for your system from the Linux and SteamOS section of the same page. It registers the OpenXR runtime, the SteamVR driver and the firewall rules for you.
2. **Press Connect.** Start the server on the PC, open KRVR on Vision Pro and tap Connect. The headset finds your PC on the local network by itself.
3. **Launch your game.** Start any VR game on the PC.

Upgrading from KRVR 1.x: the 2.0 installer replaces the old server. Close SteamVR and any VR game first, then run it over your existing install.

## Features

- **Eye-tracked foveated streaming** — the full-detail region follows your gaze. Built on Apple's Foveated Streaming framework; gaze data stays on your own network.
- **Steady frame delivery** — frame pacing keeps delivery locked to the display. Motion Smoothing gives a game that cannot keep up an even rate instead of a ragged one.
- **Mixed reality windows** — cut a passthrough window into the game to see your wheel, rig, keyboard or controllers.
- **Live tuning** — bitrate, fovea size, periphery compression and sharpening change while you play, no restarts.
- **Audio and microphone** — game audio to the headset or your PC speakers. For your headset mic in games, install the free [VB-CABLE](https://vb-audio.com/Cable/) on the PC ([setup](https://krvr.app/setup.html#audio)).
- **Hand and eye tracking** — Vision Pro tracks your hands and your eyes, and KRVR passes both to games that support them, as standard OpenXR and SteamVR input.
- **90 or 120 Hz** — on Vision Pro with M5, choose the rate in the headset and the game follows it. 120 Hz runs in Mixed immersion.
- **PlayStation VR2 Sense controllers** — tracking, buttons, finger touch and haptics through OpenXR and SteamVR.
- **Games panel and desktop mirror** — start and stop PC games from the headset, and see your PC screen in the headset on any monitor including ultrawides.

## Requirements

**Windows PC:** Windows 10 or 11 · NVIDIA or AMD GPU · latest GPU drivers · wired ethernet to your router · SteamVR installed for SteamVR games

**Linux or SteamOS PC (testing):** Ubuntu 24.04 or newer, Fedora 39 or newer, Arch, or SteamOS · NVIDIA or AMD GPU · SteamVR installed for SteamVR games

**Apple Vision Pro:** KRVR from the App Store · same local network as the PC · 5 GHz Wi-Fi, Wi-Fi 6 recommended · 120 Hz needs Vision Pro with M5

## Help and feedback

- [Setup guide and troubleshooting](https://krvr.app/setup.html)
- [Discord](https://discord.gg/zsYw3SJkHD)
- [Report an issue](https://github.com/Kross82/KRVR-releases/issues)

---

KRVR is a product of KRXR LTD, registered in England & Wales, company no. 17367119. Contact: karl@krvr.app
