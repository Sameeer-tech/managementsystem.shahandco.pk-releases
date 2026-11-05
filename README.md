# Shah & Co — Android releases

Public release channel for the Shah & Co Flutter app.

The app reads this file on launch:

`https://raw.githubusercontent.com/Sameeer-tech/managementsystem.shahandco.pk-releases/main/latest.json`

## Files

- `latest.json` — current version the app should offer (update this after every APK release)

## Publish a new version

1. In the **app** repo, bump `pubspec.yaml` (example: `1.0.1+2`).
2. Build: `flutter build apk --release`
3. Create a GitHub **Release** in **this** repo (tag `v1.0.1`) and upload `shahandco-1.0.1.apk`.
4. Update `latest.json` with the new `version`, `version_code`, and `apk_url`, then commit to `main`.

`version_code` must match the `+N` number in `pubspec.yaml`.
