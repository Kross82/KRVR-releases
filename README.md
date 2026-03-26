# KRVR — Native PCVR Streaming for Apple Vision Pro

> **ALPHA BUILD — This is an early testing release, not a finished product.** Expect bugs, rough edges, and things that need tuning. We need your feedback to make it great. Please report issues and share your experience on our [Discord](#community).

KRVR streams your PC VR games wirelessly to Apple Vision Pro with NVIDIA CloudXR foveated encoding. Low latency, high quality, native visionOS experience.

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
- TestFlight app installed

## Download

### Windows Desktop App
Download **KRVR-Setup.exe** from the [latest release](https://github.com/Kross82/KRVR-releases/releases/latest).

Run the installer — it handles everything: CloudXR runtime, firewall rules, OpenXR configuration.

### Vision Pro App
Install via TestFlight: **[Join the KRVR Beta](https://testflight.apple.com/join/gNNdfEzx)**

## Quick Start

1. **Install** KRVR on your Windows PC (run the installer)
2. **Install** KRVR on your Vision Pro (via TestFlight)
3. **Launch** KRVR on your PC — click **Start**
4. **Open** KRVR on your Vision Pro — tap **Connect**
5. **Scan** the QR code displayed on your PC
6. **Launch** a VR game from your PC
7. **Play** — the game streams to your Vision Pro

## Supported Games

Any OpenXR game works natively. SteamVR/OpenVR games work with [OpenComposite](https://gitlab.com/znixian/OpenOVR).

### Tested
- iRacing
- Microsoft Flight Simulator 2024
- Le Mans Ultimate (with OpenComposite)
- Kayak VR: Mirage
- Assetto Corsa EVO

## Network Tips

For best quality, use a dedicated 5GHz WiFi network between your PC and Vision Pro. A WiFi 6 access point connected directly to your PC via Ethernet gives the lowest latency.

## Community

Join the KRVR Discord: **[discord.gg/7RxKBNTbdh](https://discord.gg/7RxKBNTbdh)**

## Help Us Improve

This is an alpha release — your feedback is critical. We need help dialling in resolution, quality, and compatibility across different setups. Please share:

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
A: Yes, with OpenComposite. Replace `openvr_api.dll` in the game folder with the OpenComposite version.

**Q: What resolution does it stream at?**
A: Configurable. Default is 5200 render / 2080 stream with foveated encoding. Adjust in the KRVR desktop app.

**Q: Does it work over the internet?**
A: KRVR is designed for local network streaming. Internet streaming is not supported.

---

*KRVR uses NVIDIA CloudXR technology. NVIDIA and CloudXR are trademarks of NVIDIA Corporation.*
