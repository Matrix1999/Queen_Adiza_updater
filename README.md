<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:050505,45:25060a,100:dc0018&height=210&section=header&text=QUEEN%20ADIZA%20BOT&fontSize=42&fontColor=ffffff&fontAlignY=36&desc=ANDROID%20UPDATE%20CONTROL&descAlignY=59&descSize=16&animation=twinkling" width="100%"/>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=950&color=FF3347&center=true&vCenter=true&width=700&lines=Queen+Adiza+Bot+Update+Panel;Signed+APK+Release+Control;Version+Checks+%26+Change+Logs;Fast+GitHub-Hosted+Updates)](https://git.io/typing-svg)

<br/>

![App](https://img.shields.io/badge/APP-QUEEN_ADIZA_BOT-111111?style=for-the-badge&logo=android&logoColor=white)
![Channel](https://img.shields.io/badge/CHANNEL-ANDROID_UPDATES-8B0011?style=for-the-badge&logo=github&logoColor=white)
![Update mode](https://img.shields.io/badge/UPDATE_MODE-USER_CONFIRMED-202020?style=for-the-badge&logo=shield&logoColor=white)
![Signing](https://img.shields.io/badge/APK-SIGNED_RELEASE-DC0018?style=for-the-badge&logo=files&logoColor=white)

</div>

---

<div align="center">

## Queen Adiza release panel

</div>

This repository hosts the live update manifest for **Queen Adiza Bot**. The Android app checks `queen-adiza.json`, compares its `version_code` with the installed build, and presents a polished red, black, and white update dialog when a newer release is available.

```
App launch → read manifest → compare versions → show update dialog → Android installer
```

The APK is delivered through Android Download Manager. Android displays download progress and asks the user to confirm installation.

---

<div align="center">

## Current channel

</div>

| Setting | Value |
| --- | --- |
| App | Queen Adiza Bot |
| Version | 2.4.2 |
| Version code | 1 |
| Update state | Inactive until a signed release is published |
| Force update | Off |

The manifest starts with an empty `apk_url`. This keeps the update prompt quiet until the first signed APK is attached to a release.

---

<div align="center">

## Manifest

</div>

```json
{
  "version_code": 1,
  "version_name": "2.4.2",
  "apk_url": "",
  "changelog": "Queen Adiza Bot update channel initialized.",
  "update_size": "—",
  "force_update": false,
  "release_date": "2026-11-25"
}
```

| Field | Type | Purpose |
| --- | --- | --- |
| `version_code` | Integer | Increase for every app release. |
| `version_name` | Text | Version shown in the update dialog. |
| `apk_url` | HTTPS URL | Signed APK download URL from a GitHub Release. |
| `changelog` | Text | Release notes displayed before download. Use `\n` for line breaks. |
| `update_size` | Text | APK size shown in the dialog. |
| `force_update` | Boolean | `true` blocks dismissal; `false` offers “Later.” |
| `release_date` | Date | Release date in ISO `YYYY-MM-DD` format. |

---

<div align="center">

## Publish a release

</div>

1. Build the APK and sign it with the same key used for the installed app.
2. Create a GitHub Release and attach the signed file as `Queen_Adiza_Bot.apk`.
3. Increase `version_code` and update the manifest's version, release URL, notes, size, and date.
4. Leave `force_update` off for an optional update. Enable it only when older versions must stop running.

Example:

```json
{
  "version_code": 2,
  "version_name": "2.4.3",
  "apk_url": "https://github.com/Matrix1999/<repository>/releases/download/queen-adiza-v2/Queen_Adiza_Bot.apk",
  "changelog": "Improved pairing stability\nFaster session recovery",
  "update_size": "28 MB",
  "force_update": false,
  "release_date": "2026-11-25"
}
```

The app package ID and signing certificate must stay the same for Android to install an update over the existing app.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:dc0018,55:25060a,100:050505&height=110&section=footer&animation=twinkling" width="100%"/>

*Queen Adiza Bot · Update Control*

</div>
