# Hanceville Nutrition — app update feed

This public repo is the update channel for the Hanceville Nutrition app
(Android). The app reads `version.json` every time it opens:

- `versionCode` / `versionName` — the latest release
- `apkUrl` — direct download of the latest APK (the file in this repo)
- `notes` — one line shown in the in-app update banner

To ship an update:
1. Build the new APK with the same signing key (hanceville.keystore).
2. Replace `hanceville-nutrition.apk` in this repo with the new build.
3. Bump `versionCode` / `versionName` in `version.json`.

Every installed app (v1.3+) then offers the update on its next launch.
