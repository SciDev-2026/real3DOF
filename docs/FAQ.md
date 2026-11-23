# Frequently asked questions

### Is this the same as the headset's flat-screen / virtual-monitor 3DoF mode?

No. real3DOF is designed for **stereoscopic SteamVR content** with rotational head tracking, rather than simply mirroring a conventional desktop image.

### Do I need Lighthouse base stations?

Not for **Virtual Beacon / 3DoF** mode. For conventional **Lighthouse / 6DoF** mode, use your normal base stations and tracking hardware.

### Can I lean, crouch or move sideways in VR?

Not in 3DoF mode. real3DOF provides **yaw, pitch and roll**, but no physical X/Y/Z position tracking.

### Does it work in every VR game?

No universal guarantee. Apps vary in their assumptions about positional tracking and controller input. Please report the exact title and symptoms when something does not work.

### Is occasional yaw drift normal?

Some drift can occur because an IMU alone does not supply a stable absolute heading. Recenter and recalibration may help. Auto-bias cannot eliminate every source of yaw drift.

### What is Double Tap?

A configurable gesture feature that detects two physical taps on the headset, with threshold and timing diagnostics in the Control Center. Check the currently configured action before use.

### What if SteamVR does not recognize a driver?

Close SteamVR completely, restart the Control Center and review its status. For troubleshooting, include your SteamVR log with personal details removed. Avoid manually deleting unrelated third-party drivers.

### Is real3DOF open source?

Not at this time. The initial beta is distributed as compiled software, with documentation and feedback on GitHub.

### Where can I support development?

Voluntary support: https://ko-fi.com/scidev
