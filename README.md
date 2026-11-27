## 🎬 real3DOF – Showcase

See real3DOF in action on the Bigscreen Beyond 2/2e.

- Lighthouse-free 3DoF tracking
- Integrated VR Dashboard
- Customizable Double-Tap detection
- Real-time IMU visualization
- Automatic drift compensation

[![Watch the real3DOF Showcase](https://img.youtube.com/vi/qmbPRzgM4Og/maxresdefault.jpg)](https://www.youtube.com/watch?v=qmbPRzgM4Og)

▶️ [Watch the showcase on YouTube](https://www.youtube.com/watch?v=qmbPRzgM4Og)


---

## ⚠️ Disclaimer & Safety Notice

### 📋 General Disclaimer

**real3DOF** is a free, non-commercial and experimental hobby project developed independently for the VR community.

The software is provided **"AS IS"**, without any express or implied warranty, including but not limited to functionality, stability, compatibility or fitness for a particular purpose, to the extent permitted by applicable law.

> [!WARNING]
> **Installation and use of real3DOF are at your own risk.**
>
> Experimental software may contain bugs, cause unexpected behaviour or interfere with existing SteamVR configurations.

### 🛡️ Safety Instructions

> [!CAUTION]
> **Virtual Beacon (3DoF) mode is intended exclusively for seated VR experiences.**
>
> It provides rotational head tracking only and does not provide positional tracking (6DoF).

- Do not use Virtual Beacon mode for standing, walking or room-scale VR.
- Do not rely on real3DOF as a safety or boundary protection system.
- Always ensure that your physical surroundings are safe and free of obstacles.
- Unexpected tracking behaviour, orientation drift or loss of tracking may occur.
- If you experience unexpected movement, disorientation, dizziness or discomfort, stop using the software immediately and safely remove your headset.
- Restore Lighthouse tracking before returning to standing or room-scale VR.

### 🔧 System Compatibility

real3DOF interacts directly with SteamVR, headset sensors and tracking configurations.

Compatibility with all hardware configurations, operating systems, SteamVR versions and third-party applications cannot be guaranteed.

> [!IMPORTANT]
> Back up your existing SteamVR configuration before installing or using real3DOF.

Future SteamVR or headset firmware updates may affect the functionality of this software.

### ⚖️ Limitation of Liability

To the maximum extent permitted by applicable law, the developer shall not be liable for damages, data loss, system interruptions or other consequences arising from the installation, use or inability to use this software.

Nothing in this disclaimer excludes or limits liability where such exclusion or limitation is prohibited by applicable law.

### 🤝 Independent Community Project

real3DOF is an independent third-party hobby project.

It is **not affiliated with, endorsed by, sponsored by or officially supported by Bigscreen or Valve Corporation.**

All third-party trademarks and product names belong to their respective owners.

---



# real3DOF

**Real stereoscopic 3DoF for Bigscreen Beyond 2 / 2e — without Lighthouse base stations.**

*Experimental SteamVR driver and Windows Control Center by SCI.*

> **Beta 0.2 · Test version**  
> This project is under active development. Use it for testing; it is not a replacement for full room-scale 6DoF tracking.

## What does real3DOF do?

real3DOF allows compatible Bigscreen Beyond 2 / 2e headsets to run **stereoscopic SteamVR content with rotational head tracking** — yaw, pitch and roll — using the headset's motion sensors, without requiring active Lighthouse base stations for 3DoF mode.

Unlike a flat monitor mirrored into a headset, the virtual viewpoint responds to the direction you look. **Positional head tracking is not provided in 3DoF mode.**

### Features in Beta 0.2

- **Virtual Beacon / 3DoF mode**: rotational tracking without Lighthouse base stations.
- **Lighthouse / 6DoF mode**: switch back to your regular SteamVR setup.
- **Native SteamVR integration** via dedicated drivers.
- **Windows Control Center** with live tracking readings and a wireframe headset preview.
- **Recalibrate, recenter and auto-bias** controls to help manage sensor drift.
- **Double Tap** headset-input feature with configurable sensitivity and diagnostic graph.
- **English and German** UI.

## Requirements

- Windows PC with SteamVR.
- Bigscreen Beyond 2 or Beyond 2e headset, connected and configured for SteamVR.
- Current beta installer (when a test release is made available).

**No Lighthouse base stations are required while using Virtual Beacon / 3DoF mode.** For conventional Lighthouse / 6DoF tracking you still need the appropriate Lighthouse hardware.

## Installation

See [Installation & setup](docs/INSTALLATION.md).

For troubleshooting, see [FAQ](docs/FAQ.md) and [Beta testing checklist](docs/TESTING.md).

## Downloads

The first installer is being prepared as a **test release**. Check [GitHub Releases](https://github.com/SciDev-2026/real3DOF/releases). A release draft is not public until it is explicitly published by the developer.

## Important limitations

- **3DoF is orientation-only:** leaning or walking around does not move your virtual head position.
- **Yaw drift is possible:** without an external absolute orientation reference, some heading drift can accumulate. Auto-bias reduces certain gyro-offset errors but cannot guarantee a fixed absolute heading.
- Some SteamVR apps assume full 6DoF or tracked controllers, so behavior varies by application.
- Beta software may require SteamVR restarts, recalibration, or troubleshooting.

## Feedback and bug reports

Please open a GitHub [Issue](https://github.com/SciDev-2026/real3DOF/issues) and include your Windows and SteamVR versions, headset model, steps to reproduce, and relevant **redacted** logs. Do not post account information, device serial numbers, or private paths.

## Support the project

If you find real3DOF useful, you can support development voluntarily on [Ko-fi](https://ko-fi.com/scidev). Support is optional.

## Development and distribution

This beta is distributed as compiled binaries. Source code is **not** published under an open-source license. Do not assume that public access to this documentation grants permission to redistribute or modify the binaries.

real3DOF is an independent community project by **SCI**, not affiliated with or endorsed by Bigscreen or Valve. Bigscreen Beyond, SteamVR, and other marks belong to their respective owners.

© 2026 SCI. All rights reserved.

<!-- SCI:BEGIN BETA_0_2_DOCS -->
## Beta 0.2: user manual, compatibility and known issues

**Please launch the real3DOF Control Center first, select and apply the tracking mode, and only then start SteamVR.**

- [English User Manual (PDF, including Double Tap and Expert Mode)](https://github.com/SciDev-2026/real3DOF/releases/download/v0.2.0-beta.1/real3DOF_Beta_0.2_User_Manual_EN.pdf)
- [Known Issues & Development Roadmap](docs/KNOWN_ISSUES_AND_ROADMAP.md)
- [HMD Dashboard Button hotfix (English, automatic backup)](https://github.com/SciDev-2026/real3DOF/releases/download/v0.2.0-beta.1/real3DOF_SCI_HMD_Bindings_MergeFix_v2_EN.zip)
- [Beta 0.2 download / release notes](https://github.com/SciDev-2026/real3DOF/releases/tag/v0.2.0-beta.1)

**Tested hardware:** Bigscreen Beyond **2e** only. Beyond 2 and original Beyond have **not** been tested; experimental use is at your own risk and compatibility is not guaranteed.

**Designed primarily for:** seated **simracing**, **UEVR** games, and VR titles operated with a **gamepad, keyboard or mouse** rather than tracked VR controllers. Virtual Beacon provides rotational 3DoF only, not positional 6DoF tracking.

**Known Beta 0.2 issues:** Double Tap **does not work in Lighthouse mode**; Dashboard/HMD Button may need the separate binding hotfix; the live acceleration trace may show `TRACE unavailable`; and the Virtual Beacon may remain visible when Lighthouse mode is selected. See the [full status and roadmap](docs/KNOWN_ISSUES_AND_ROADMAP.md).
<!-- SCI:END BETA_0_2_DOCS -->
