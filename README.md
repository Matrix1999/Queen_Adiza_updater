<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:050505,45:25060a,100:dc0018&height=220&section=header&text=QUEEN%20ADIZA%20BOT&fontSize=42&fontColor=ffffff&fontAlignY=36&desc=WHATSAPP%20AUTOMATION%20%7C%20ANDROID%20CONTROL&descAlignY=59&descSize=15&animation=twinkling" width="100%"/>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=19&pause=900&color=FF3347&center=true&vCenter=true&width=750&lines=Manage+multiple+WhatsApp+sessions;Pair+numbers+inside+the+Android+app;AI%2C+media+and+group+tools;Queen+Adiza+Bot+2.4.2)](https://git.io/typing-svg)

<br/>

![App](https://img.shields.io/badge/APP-QUEEN_ADIZA_BOT-111111?style=for-the-badge&logo=android&logoColor=white)
![Runtime](https://img.shields.io/badge/RUNTIME-NODE_20-202020?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Sessions](https://img.shields.io/badge/SESSIONS-MULTI_NUMBER-8B0011?style=for-the-badge&logo=whatsapp&logoColor=white)
![Theme](https://img.shields.io/badge/THEME-RED_BLACK_WHITE-DC0018?style=for-the-badge&logo=android&logoColor=white)

</div>

---

## What Queen Adiza Bot does

Queen Adiza Bot is a WhatsApp automation bot managed from an Android dashboard. Link one or more WhatsApp numbers in the app, then control their bot sessions from one place. Each linked number receives its own session.

### Bot features

- **Multi-number sessions:** pair numbers in the app, view each session, and manage the bot from the dashboard.
- **AI chat:** switch between supported chat models and enable or disable AI replies.
- **Image creation:** generate images with supported creative models.
- **Media tools:** access commands for media downloads, audio, search, stickers, and conversions.
- **Group tools:** use the bot's group and admin command sets in WhatsApp chats.
- **Owner controls:** manage bot settings and session behavior through its command plugins.

The available commands depend on the bot configuration and on whether their required services are reachable.

## Run it on Android

1. Install **Queen Adiza Bot**.
2. Tap **Install or update engine** to prepare the Android Node 20 runtime and the bot's npm packages.
3. Open the dashboard and start the engine.
4. Choose **Sessions → Add session**, enter a WhatsApp number with its country code, and complete pairing in WhatsApp under **Linked devices**.
5. Repeat to add another number.

The app keeps the engine running with an Android foreground notification and a Stop action. Android 7 or later is required for bot hosting.

## Update channel

The app checks [`queen-adiza.json`](https://raw.githubusercontent.com/Matrix1999/Queen_Adiza_updater/main/queen-adiza.json) for a newer version. It shows a branded update dialog, downloads the signed APK, and opens Android's installer for the user's confirmation.

For each release, increase `version_code`, publish a signed APK in a GitHub Release, and update the manifest's version, APK URL, changelog, and file size. Keep the same package ID and signing key so Android can install the update over the existing app.

The current manifest remains inactive until a signed APK is published.

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:dc0018,55:25060a,100:050505&height=110&section=footer&animation=twinkling" width="100%"/>

*Queen Adiza Bot · WhatsApp automation from Android*

</div>
