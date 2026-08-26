<p align="center">
  <img src="docs/logo.png" width="92" alt="VisInk" />
</p>

<p align="center">
  <strong>English</strong> · <a href="README.zh.md">中文</a>
</p>

<h1 align="center">VisInk</h1>

<p align="center">
  <em>Multimedia clients for your own library.</em>
</p>

<p align="center">
  VisInk builds clients that sit on your television, talk to <strong>your</strong> media server, and stay out of the way of the film.<br/>
  This repository is the <strong>free Android TV distribution</strong> — signed APKs on GitHub Releases, not the Play Store, with no subscription and no in-app purchase.
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><strong>Download the latest release</strong></a>
</p>

---

<p align="center">
  <img src="docs/screens/home.jpg" alt="Home" width="920" />
</p>
<p align="center"><sub>Home</sub></p>

<p align="center">
  <img src="docs/screens/welcome.jpg" alt="Welcome" width="48%" />
  &nbsp;
  <img src="docs/screens/login.jpg" alt="Sign in" width="48%" />
</p>
<p align="center"><sub>Welcome · Sign in</sub></p>

<p align="center">
  <img src="docs/screens/search.jpg" alt="Search" width="48%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="Title details" width="48%" />
</p>
<p align="center"><sub>Search · Details</sub></p>

<p align="center">
  <img src="docs/screens/mine.jpg" alt="Mine" width="48%" />
  &nbsp;
  <img src="docs/screens/settings.jpg" alt="Settings" width="48%" />
</p>
<p align="center"><sub>Mine · Settings</sub></p>

---

## What VisInk is

VisInk is a **multimedia client brand**. The product is the living-room remote experience: browse a private catalog, open a title, and play it on a television you already own. It is not a streaming service and it does not host your files. You bring an Emby server; VisInk brings the TV app.

The Android TV client is built for Leanback televisions and a D-pad. It is given away from this repository.

## What this repository is

Packages do **not** live on the default branch. Each version is a GitHub Release / tag with three signed APKs. Feature notes for that version are on the tag.

| File | Use |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32-bit ARM. **Prefer this on most TVs.** |
| `VisInk-*-arm64-v8a.apk` | 64-bit ARM |
| `VisInk-*-universal.apk` | All ABIs, largest download — use if you are unsure |

Application ID is `com.skymei.visink`. Requires **Android TV (Leanback)** on **Android 7.0** or later.

Update by overlay-installing a newer build signed with the same key. **Do not uninstall first** — uninstalling wipes saved servers and the login on the device.

## In the Android TV app

- Connect your Emby server, restore a session, and switch recent accounts
- Home, library, search, movie / series / person details
- Continue watching and favorites
- Playback: direct first, device decode or libVLC when needed, server transcode last
- Appearance, playback, search, and UI language in Settings
- Languages: system, Simplified Chinese, Traditional Chinese, English, Japanese, Korean, Spanish, French, German

There is no Google Play listing, no Play billing, and no Android TV Top Shelf / system recommendations.
