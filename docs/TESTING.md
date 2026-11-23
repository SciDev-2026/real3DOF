# Beta testing checklist

Please record results for each item instead of assuming a successful installer build means the installed software is correct.

- [ ] Installer starts and completes on a PC without previous real3DOF development drivers.
- [ ] Both native SteamVR drivers register under the intended installation directory.
- [ ] SteamVR starts without unexpected errors.
- [ ] Virtual Beacon / 3DoF provides stereo rendering and responsive yaw/pitch/roll.
- [ ] Live tracking status and preview update normally.
- [ ] Recenter and recalibrate operate as expected.
- [ ] Double Tap only triggers according to configured thresholds/timing.
- [ ] Switching to Lighthouse / 6DoF restores the normal hardware setup.
- [ ] Installer upgrade preserves intended settings.
- [ ] Uninstall removes only real3DOF registrations/files and does not disturb third-party drivers.

**Please keep a backup of your setup until these checks pass.**

When filing an issue, include the build label, headset model, Windows/SteamVR versions and reproduction steps. Redact usernames, filesystem paths, device serials and login information before attaching logs or screenshots.
