<!-- SCI-MANAGED: REAL3DOF_BETA_0_2_STATUS -->
# real3DOF Beta 0.2 - Known Issues & Development Roadmap

real3DOF is an experimental SteamVR tool in active beta development. This document describes the current Beta 0.2 behavior and planned improvements. These plans may change.

## Important startup order

1. Start **real3DOF Control Center** while SteamVR is closed.
2. Select either **Virtual Beacon (3DoF)** or **Lighthouse (6DoF)** on the Overview tab.
3. **Apply** the selected mode and wait for confirmation.
4. Start **SteamVR**, and then launch the intended game or application.

See the [English User Manual (PDF)](https://github.com/SciDev-2026/real3DOF/releases/download/v0.2.0-beta.1/real3DOF_Beta_0.2_User_Manual_EN.pdf) for Control Center, Double Tap, advanced parameters and Expert Mode.

## Intended use / application compatibility

- **Simracing** and seated racing simulators where rotational head tracking is enough.
- **UEVR** games and other seated stereoscopic VR experiences which can be used without tracked VR controllers.
- Titles operated using a **gamepad, keyboard or mouse** instead of motion controllers.
- Virtual Beacon mode supplies **Yaw, Pitch and Roll (3DoF)** only. Head translation, leaning and room-scale movement are not tracked.
- Games requiring 6DoF positional head tracking or tracked VR controllers may not work as intended. Application compatibility has not been comprehensively tested.

## Headset compatibility

| Headset | Beta 0.2 status |
| --- | --- |
| Bigscreen Beyond 2e | Tested on this hardware. |
| Bigscreen Beyond 2 | Not tested; expected to be potentially compatible, but unverified. |
| Original Bigscreen Beyond | Not tested; compatibility unknown. |

**Use on untested headsets is experimental and at your own risk.** No guarantee of compatibility or safe operation is made.

## Known issues - Beta 0.2

| Area | Current limitation | Workaround / status |
| --- | --- | --- |
| Double Tap / Lighthouse | **Double Tap does not work in Lighthouse mode.** | Use the supported Double Tap functionality in Virtual Beacon (3DoF) mode. A driver fix is planned. |
| HMD Button / SteamVR Dashboard | On some computers the Double Tap HMD Button action is ignored even though the tap is detected. | Use the [English HMD Binding Hotfix v2](https://github.com/SciDev-2026/real3DOF/releases/download/v0.2.0-beta.1/real3DOF_SCI_HMD_Bindings_MergeFix_v2_EN.zip). It backs up the original SteamVR bindings and adds only missing entries. |
| Live acceleration graph | The Double Tap oscilloscope can display **`TRACE unavailable: update driver`**. | The missing/unsupported TRACE data path is under investigation. |
| Virtual Beacon after mode switch | The virtual Beacon may remain visible in SteamVR after switching to Lighthouse mode. | Cosmetic issue; proper hiding is planned. |
| Yaw drift | Extended 3DoF sessions can accumulate some yaw drift with IMU-only orientation tracking. | Recenter and calibrate as needed; tuning is ongoing. |
| App compatibility | Not all SteamVR/UEVR titles have been tested. | Prefer seated applications that do not require tracked VR controllers. |

## Planned improvements

### Double Tap and SteamVR

- Make Double Tap work in **Lighthouse (6DoF) mode**.
- Integrate the HMD Button binding fix into the installer, with backups and a non-destructive merge.
- Restore live accelerometer graph / TRACE data and improve diagnostic feedback.
- Hide the **Virtual Beacon** automatically when Lighthouse mode is selected.
- Improve mode-switching and driver initialization reliability.

### Control Center UI

- General GUI cleanup and usability improvements.
- Add an optional **system tray mode** when minimized / running in the background.
- Display clearer real-time HMD, IMU and driver state indicators.

### Tracking

- Improve stability and responsiveness in Virtual Beacon mode.
- Refine IMU calibration, auto-bias behavior and yaw drift mitigation.

### Future VR dashboard integration

- Create an **in-VR SteamVR dashboard tool** for real3DOF.
- View and modify Double Tap settings in the headset, including sensitivity and timing.
- Enable/disable Double Tap without leaving VR.

## Feedback

Report bugs through [GitHub Issues](https://github.com/SciDev-2026/real3DOF/issues) and provide the headset model, SteamVR version, real3DOF version, active tracking mode, steps to reproduce and relevant error messages. Do not post personal data or private system logs publicly without reviewing them.