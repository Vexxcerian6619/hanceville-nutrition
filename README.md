# Hanceville Nutrition — app update feed

This repo is the public update channel for the Hanceville Nutrition app
(Android). The app reads `version.json` when it opens:

- `versionCode` / `versionName` — the latest release
- `apkUrl` — where the latest APK downloads from
- `notes` — one line shown in the in-app update banner

To ship an update: build the new APK with the same signing key, upload it
over the same Google Drive file (keeps the link), bump `version.json`
here. Every installed app offers the update on its next launch.
