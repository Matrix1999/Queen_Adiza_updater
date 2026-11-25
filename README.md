# Queen Adiza Bot · Update Panel

This repository hosts the update manifest used by the Queen Adiza Android app.

On launch, Queen Adiza reads `queen-adiza.json`, compares `version_code` with the installed app, and shows the in-app update dialog when a newer version is available. The APK is downloaded with Android Download Manager and installed through Android's package installer.

## Manifest fields

| Field | Purpose |
| --- | --- |
| `version_code` | Increase for every app release. |
| `version_name` | Version shown in the update dialog. |
| `apk_url` | HTTPS URL of the APK attached to a GitHub Release. |
| `changelog` | Release notes shown before downloading. Use `\n` for line breaks. |
| `update_size` | APK size label shown in the dialog. |
| `force_update` | `true` blocks dismissal; `false` offers “Later.” |
| `release_date` | Release date in ISO `YYYY-MM-DD` format. |

## Publish a Queen Adiza update

1. Build and sign the APK with the same signing key used for the installed app.
2. Create a GitHub Release and attach the signed APK.
3. Increase `version_code` and update the version, release download URL, changelog, size, and date in `queen-adiza.json`.
4. Keep `force_update` false for an optional update. Set it true only when older builds must stop being used.

Example release manifest:

```json
{
  "version_code": 2,
  "version_name": "2.4.3",
  "apk_url": "https://github.com/Matrix1999/munowatch-updater-panel/releases/download/queen-adiza-v2/Queen_Adiza_Bot.apk",
  "changelog": "Improved pairing stability\nFaster session recovery",
  "update_size": "28 MB",
  "force_update": false,
  "release_date": "2026-11-25"
}
```

Android always asks the user to confirm installation. An update must keep the app's package ID and use the same signing certificate as the installed build. The first manifest intentionally has an empty `apk_url`, so it remains inactive until a signed release is published.
