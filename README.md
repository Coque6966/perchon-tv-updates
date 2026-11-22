# Perchon TV — Update files

Update server for **Perchon TV** (movies, series and live TV) and **Coque Tube** (ad-free YouTube), served through GitHub Pages. The apps check the JSON manifests below for new versions and update themselves — no reinstall needed.

Live site: https://coque6966.github.io/perchon-tv-updates/

Developed by Jorge Arturo Rodríguez Araujo (Coque6966), Mexico.

## Current versions

| App | Platform | Version | Package |
|---|---|---|---|
| Perchon TV | Android TV | v1.9.12 | coque-tv-tv-v1.9.12.apk |
| Perchon TV | Fire TV | v1.9.12 | perchon-tv-firestick-v1.9.12.apk |
| Perchon TV | Phone (Android) | v1.5.6 | coque-tv-v1.5.6.apk |
| Perchon TV | Roku | v5.7 | perchon-tv-roku-v5.7.zip |
| Perchon TV | LG webOS | v1.0.3 | coque-tv-webos-v1.0.3.ipk |
| Perchon TV | Samsung Tizen | v1.0.3 | coque-tv-tizen-v1.0.3.wgt |
| Coque Tube | Android TV | v2439 (32.48) | coque-tube-v2439.apk |
| Coque Tube | Fire TV | v2439 (32.48) | coque-tube-firestick-v2439.apk |
| Coque Tube | Roku | v1.0.6 | coque-tube-roku-v1.0.6.zip |
| Coque Tube | LG webOS | v1.0.2 | coque-tube-webos-v1.0.2.ipk |
| Coque Tube | Samsung Tizen | v1.0.2 | coque-tube-tizen-v1.0.2.wgt |

Older Perchon TV builds (v1.9.6–v1.9.11) are kept in this repo as rollback versions.

## Update manifests

- `coque-tv-tv-update.json` — Perchon TV for Android TV / Fire TV
- `coque-tv-update.json` — Perchon TV for phone
- `coque-tube-update.json` — Coque Tube for Android TV / Fire TV

Each manifest points to its APK on this same site. To publish a new version: copy the new APK into this directory, update its `apkUrl` in the matching JSON, commit and push. GitHub Pages serves the new manifest immediately.

## DO NOT upload

**Never upload `remote-kit.json` here: it contains access to the update portal.** Only the manifests and the app packages listed above belong in this repo.

## Status

Perchon TV v1.9.12 is installed and verified on a real TCL Android TV (65", Android 11). Coque Tube v2439 is installed on the same TV. Roku, webOS and Tizen packages are built and published here; they have not yet been verified on a real TV of each platform.
