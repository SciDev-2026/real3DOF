# Installation and setup — real3DOF Beta 0.2

> **Experimental test release.** Keep a copy of your existing SteamVR driver configuration and test carefully before relying on it.

## Before installing

1. Install and launch SteamVR at least once with your normal Bigscreen Beyond 2 / 2e setup.
2. Close SteamVR completely before running the real3DOF installer.
3. Download the test installer **only** from the project's GitHub Releases page.
4. Keep any existing real3DOF development driver directories until you have verified the new installation.

## Install

1. Run the installer and follow its prompts.
2. Launch **real3DOF Control Center**.
3. Select **Virtual Beacon / 3DoF**, apply the tracking mode, and follow any SteamVR restart prompt.
4. Verify that tracking shows **LIVE** and that yaw, pitch and roll respond to gentle head movements.
5. If needed, use **Recenter** and **Recalibrate**.

For regular room-scale tracking, select **Lighthouse / 6DoF** and apply the mode.

## Double Tap

Open the **Double Tap** tab. Enable it only if desired, configure its thresholds, and verify its behavior in the diagnostics before using it in SteamVR.

## Uninstall / rollback

1. Return to **Lighthouse / 6DoF** when possible.
2. Close SteamVR and the Control Center.
3. Uninstall via Windows Installed Apps.
4. Confirm SteamVR starts normally with your original headset setup.

Do not delete existing prototype folders until you have confirmed that the installer and uninstaller behave as expected on your system. If SteamVR driver registration remains abnormal, consult the project issue tracker instead of removing unrelated drivers.

## Troubleshooting

See [FAQ](FAQ.md).
