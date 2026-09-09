<h1 align="center">
  <img src="docs/logo-ink.png#gh-light-mode-only" height="28" width="28" alt="VisInk" />
  <img src="docs/logo.png#gh-dark-mode-only" height="28" width="28" alt="VisInk" />
  VisInk
</h1>

<p align="center">
  <strong>English</strong> · <a href="README.md">中文</a>
</p>

<p align="center">
  A free Emby client for Android TV.
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><img src="https://img.shields.io/github/v/release/skymei/VisInkAndroidTVRelease?label=release" alt="Latest release" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases"><img src="https://img.shields.io/github/downloads/skymei/VisInkAndroidTVRelease/total?label=downloads" alt="Downloads" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><img src="https://img.shields.io/github/downloads/skymei/VisInkAndroidTVRelease/latest/total?label=latest%20downloads" alt="Latest release downloads" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/stargazers"><img src="https://img.shields.io/github/stars/skymei/VisInkAndroidTVRelease?style=flat" alt="Stars" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/issues"><img src="https://img.shields.io/github/issues/skymei/VisInkAndroidTVRelease" alt="Issues" /></a>
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases"><strong>Download</strong></a>
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

Your media lives on your own Emby server. This project only provides the Emby client for browsing and playback.

APKs are on [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases), under each tag. Always install the latest stable Release — Pre-Release builds are test versions and may have issues. To update, overlay-install on top of the existing app. **Do not uninstall first** — that wipes the servers and accounts you have already signed in to.

## Which APK

| File | Use |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32-bit ARM. **Most TVs should use this.** |
| `VisInk-*-arm64-v8a.apk` | 64-bit ARM |
| `VisInk-*-universal.apk` | All ABIs, largest file. Use only if you are unsure. |

## Android version and hardware

| | Minimum | Recommended |
|---|---|---|
| System | Android **7.0** (API 24) | Android **12** or later |
| Device | A TV or box with a TV launcher and a D-pad remote (Android TV, Google TV, and similar). Phones and tablets are not supported. | A living-room set or box you actually use with a remote, 1080p or 4K |
| CPU | 32-bit ARM (`armeabi-v7a`) or 64-bit ARM (`arm64-v8a`) | Same as the TV: 32-bit box → v7a package; 64-bit box → arm64 package |
| Video | A hardware decoder for common files (at least H.264) | Hardware decode for H.264 and HEVC so most libraries direct-play |
| Network | Reach your Emby server from the TV | Wired or stable Wi-Fi to the server |
| Storage | ~100 MB for an ABI build; ~250 MB for universal | Same; leave headroom for artwork cache |

The UI is designed around 1080p Android TV. 4K sets work. This is not a phone APK.

## Current capabilities

- Emby login and saved session
- Multiple servers and accounts
- Home, library, search
- Movie / series details
- Person pages
- Continue watching and favorites
- Direct play; transcode when the TV cannot decode
- Subtitles, audio tracks, playback speed, next episode
- Appearance, playback, and search settings
- UI in Simplified Chinese, Traditional Chinese, English, Japanese, Korean, and more

## Feedback

This project is still early. Please bear with us if something is rough.

Android TV runs on a wide variety of system builds, and we don't have enough physical TVs to test every one. Despite testing on a mix of real devices and emulators, compatibility issues may still arise. Please download an official release build. If you run into a problem, open an [issue](https://github.com/skymei/VisInkAndroidTVRelease/issues) or email [support@visink.cc](mailto:support@visink.cc).

When reporting a bug, please be as specific as you can: which build, which TV or box, what media format you were playing, what you did, what you expected, and what actually happened. Screenshots or a short screen recording make it much easier for us to investigate and fix.
