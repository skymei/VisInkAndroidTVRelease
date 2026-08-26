**English** | [中文](README.zh.md)

# VisInk Android TV

An Emby client for Android TV. Free sideload builds. Not on Google Play, and there is no subscription or in-app purchase.

Packages are not on the default branch. Download APKs from [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases) (the version tags).

## Which package

| File | Use |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32-bit ARM. **Prefer this on TVs** |
| `VisInk-*-arm64-v8a.apk` | 64-bit ARM |
| `VisInk-*-universal.apk` | All ABIs, largest file; use if you are unsure |

Requires Android TV (Leanback) on Android 7.0 or later. Application ID is `com.skymei.visink`.

Update by overlay-installing a newer build with the same signature. Do not uninstall first: uninstalling wipes the saved servers and login on the device. Feature notes for each version are on that version’s tag / Release.

## What it does

After you connect your Emby server, the remote can browse Home, Library, Search, movie/series/person details, continue watching, and favorites, then play (direct first, with fallback or server transcode when needed). Settings cover appearance, playback, search, and UI language.
