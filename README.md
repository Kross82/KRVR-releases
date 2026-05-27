# KRVR — Native PCVR Streaming for Apple Vision Pro

KRVR streams your PC VR games wirelessly to Apple Vision Pro with NVIDIA CloudXR foveated encoding. Low latency, high quality, native visionOS experience.

**Now live on the App Store.** Pair the visionOS app with the Windows desktop installer below to get streaming.

## Features

- **Foveated Streaming** — Eye-tracked rendering sends full resolution where you're looking, compressed periphery. Powered by Apple FoveatedStreaming + NVIDIA CloudXR.
- **90Hz Streaming** — Smooth VR at full refresh rate with adaptive pose prediction.
- **Game Profiles** — Per-game resolution and quality settings. Auto-applied on launch.
- **Live Stats HUD** — In-headset pill overlay showing FPS, encode time, GPU time, network latency, resolution.
- **Desktop Mirror** — View your PC screen from inside the headset.
- **Passthrough Support** — Mixed reality mode with alpha blending for cockpit sims.
- **Controller Support** — PSVR2 Sense controllers with haptic feedback.
- **Auto Immersion** — Starts in passthrough, switches to full immersion when a game launches, returns to passthrough when you quit.

## Requirements

### PC (Windows)
- Windows 10 (October 2018 update) or Windows 11
- NVIDIA GeForce RTX 40 series or newer (RTX 50 recommended)
- 5GHz WiFi network, 50Mbps+ sustained recommended
- Latest NVIDIA drivers

### Headset
- Apple Vision Pro
- visionOS 26.4 or later
- KRVR app installed (from the App Store or TestFlight)

## Download

> ⚠️ **Don't use the green "Code → Download ZIP" button.** That only downloads this README. The Windows installer is below ↓

### Windows Desktop App
Download **KRVR-Setup-v1.3.6.exe** from the [latest release](https://github.com/Kross82/KRVR-releases/releases/latest) (under the **Assets** section).

Run the installer — it handles everything: CloudXR runtime, firewall rules, OpenXR configuration, SteamVR driver registration.

### Vision Pro App
Install from the **[App Store](https://apps.apple.com/us/app/krvr/id6761065018)** (recommended), or join the beta via **[TestFlight](https://testflight.apple.com/join/gNNdfEzx)** to get earlier builds with new features as they ship.

## Quick Start

1. **Install** KRVR on your Windows PC (run the installer)
2. **Install** KRVR on your Vision Pro (from the App Store)
3. **Launch** KRVR on your PC — click **Start**
4. **Open** KRVR on your Vision Pro — tap **Connect**
5. **Scan** the QR code displayed on your PC
6. **Launch** a VR game from your PC
7. **Play** — the game streams to your Vision Pro

## Supported Games

Any OpenXR game works natively. SteamVR/OpenVR games work natively too — KRVR ships with a built-in SteamVR driver based on [mbucchia's OpenVR-CloudXR](https://github.com/mbucchia/OpenVR-CloudXR). No OpenComposite, no manual setup.

### Tested
**OpenXR-direct**
- iRacing
- Microsoft Flight Simulator 2024
- Le Mans Ultimate
- Kayak VR: Mirage
- Assetto Corsa EVO

**SteamVR / OpenVR**
- Half-Life: Alyx
- Skyrim VR
- Assetto Corsa
- Pavlov VR
- Boneworks

## Network Tips

For best quality, use a dedicated 5GHz WiFi network between your PC and Vision Pro. A WiFi 6 access point connected directly to your PC via Ethernet gives the lowest latency.

## Community

Join the KRVR Discord: **[discord.gg/7RxKBNTbdh](https://discord.gg/7RxKBNTbdh)**

## Help Us Improve

Your feedback drives the roadmap. We need help dialling in resolution, quality, and compatibility across different hardware setups. Please share:

- Your GPU model and driver version
- Games you've tested (working or not)
- Network setup (router, connection type)
- Screenshots or clips of any issues
- Quality/latency impressions

Post feedback in **#bug-reports** or **#feature-requests** on Discord.

## FAQ

**Q: Do AMD/Intel GPUs work?**
A: No. KRVR requires NVIDIA RTX 40 series or newer for CloudXR hardware encoding.

**Q: Can I use SteamVR games?**
A: Yes. KRVR v1.3.6 ships with a built-in SteamVR driver based on mbucchia's OpenVR-CloudXR. Just launch SteamVR games from Steam — no OpenComposite, no DLL swaps.

**Q: What resolution does it stream at?**
A: Configurable. Defaults are 4400 render / 2400 stream with foveated encoding. Adjust in the KRVR desktop app.

**Q: Does it work over the internet?**
A: KRVR is designed for local network streaming. Internet streaming is not supported.

---

*KRVR uses NVIDIA CloudXR technology. NVIDIA and CloudXR are trademarks of NVIDIA Corporation.*
