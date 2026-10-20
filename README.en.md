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

<p align="center">
  <img src="docs/screens/immersive.jpg" alt="Immersive carousel" width="960" />
</p>
<p align="center"><sub>Immersive carousel after idle</sub></p>

<p align="center">
  <img src="docs/screens/home.jpg" alt="Home" width="48%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="Series details" width="48%" />
</p>
<p align="center"><sub>Home · Series details</sub></p>

<p align="center">
  <img src="docs/screens/player.jpg" alt="Playback with danmaku" width="48%" />
  &nbsp;
  <img src="docs/screens/player-paused.jpg" alt="Paused" width="48%" />
</p>
<p align="center"><sub>Playback with danmaku · Paused</sub></p>

<p align="center">
  <img src="docs/screens/library.jpg" alt="Library" width="48%" />
  &nbsp;
  <img src="docs/screens/search.jpg" alt="Search" width="48%" />
</p>
<p align="center"><sub>Library · Search across servers</sub></p>

<p align="center">
  <img src="docs/screens/settings.jpg" alt="Playback settings" width="960" />
</p>
<p align="center"><sub>Playback settings: bitrate, subtitles, danmaku, and decoding</sub></p>

---

## Capabilities

Your media stays on your Emby server. This project is the TV client for signing in, browsing, and playback.

### Library

- Sign in to Emby and keep the session. Multiple servers and accounts.
- A proxy can be set on each server line.
- Home, an idle immersive carousel, continue watching, favorites, and favorite people.
- Library browsing with watched-state filters and sort.
- Search the current server, or every saved server at once. A phone can submit the query by scanning a code.
- Movie and series details, seasons and episodes, and person pages.

### Playback

- Direct play first. The server transcodes only when the TV cannot decode the file.
- A manual bitrate ceiling.
- Hardware video decode. Audio can use automatic, software, or system decode, including AAC, AC3, EAC3, DTS, and TrueHD.
- Audio tracks, playback speed, and several seek step sizes.
- The app can remember speed, audio, subtitles, and version for the same movie or series.
- Intros, credits, and the next episode.
- The active server line can be changed during playback.

#### Supported media formats

The app first tries to let the TV or box play the original media directly. Most common files play this way when the device supports their formats; otherwise, Emby may convert the media into a compatible format first. A TV that supports Dolby Vision is required for Dolby Vision playback, but the file's profile, container, and audio tracks can still affect the final result.

| Type | Playable range | Notes |
|---|---|---|
| Video | H.264 / AVC | MP4, M4V, MOV, MKV, and TS; also the format most often used when the server converts video |
| Video | HEVC / H.265 | MP4, MKV, and TS; common 4K, Main10, and HDR files usually work, depending on the TV or box |
| Video | AV1 | MP4, MKV, and WebM; requires AV1 decoding on the TV or box |
| Video | VP8 / VP9 | MKV and WebM; requires the corresponding decoder on the TV or box |
| Picture | SDR, HDR10, HDR10+, HLG | Requires the TV or box to support the corresponding HDR display mode |
| Dolby Vision | Common Profile 5 and Profile 8 / 8.1 | When the TV or box supports the profile, the app can pass the Dolby Vision picture to it and may trigger the TV's Dolby Vision mode; verify actual files on devices such as the Sony X90L |
| Dolby Vision | Profile 7 | Some files play as HDR10; keeping full Dolby Vision depends on the file and device |
| Dolby Vision | Profile 8.4 and Profile 4 | Some TVs and files work; compatibility depends on the actual device |
| Audio | AAC, AC-3, E-AC-3, MP3, FLAC, Opus, Vorbis, DTS, DTS-HD, TrueHD, ALAC, WMA, PCM | Common tracks can play; Atmos and DTS:X output depends on the TV, receiver or soundbar, and the HDMI/eARC connection |
| Files and streaming | MP4, M4V, MOV, MKV, WebM, TS, HLS | The extension is only the outer container; the video, audio, and subtitle tracks inside it still affect direct playback |

The following sources are more likely to need server conversion: VC-1, WMV3, ProRes, HEVC in 12-bit or 4:2:2 / 4:4:4, and ISO, BDMV, RM, or RMVB. A file can also be converted when its resolution, bitrate, frame rate, audio, or subtitles exceed the device's capabilities.

After server conversion, Dolby Vision or HDR10+ dynamic effects may not be preserved. Open “Media Info” during playback to see whether the current route is Direct Play, Direct Stream, or server conversion.

### Subtitles and danmaku

- Text subtitles: SRT, VTT, and ASS / SSA, with size, position, and color.
- Image subtitles: PGS, DVB, and VobSub.
- The current subtitle can be nudged earlier or later while playing.
- ASSRT can be connected as an online subtitle source.
- Danmaku follows the film clock, with automatic matching, manual search, style, and a timing offset.
- A compatible danmaku service can be added, including setup from a phone.

### App

- Appearance themes, and three text sizes.
- Interface languages: system, Simplified Chinese, Traditional Chinese, English, Japanese, Korean, Spanish, French, and German.
- Clear video, image, subtitle, danmaku, and update caches by category. Sign-in and settings stay.
- Check GitHub for a stable release and install it over the current app.

## Which APK

APKs are on [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases). Install the latest stable Release. Pre-Release builds are for testing and are not meant for daily use. To update, install over the existing app. Do not uninstall first — that removes the servers you have already signed in to.

| File | Use |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32-bit ARM. **Most TVs should use this.** |
| `VisInk-*-arm64-v8a.apk` | 64-bit ARM |
| `VisInk-*-universal.apk` | All ABIs. Largest file. Use it only when the chip is unknown. |

## Android version and hardware

| | Minimum | Recommended |
|---|---|---|
| System | Android **7.0** (API 24) | Android **12** or later |
| Device | A TV or box with a TV launcher and a D-pad remote. Phones and tablets are not supported. | A 1080p or 4K set you actually use with a remote |
| CPU | 32-bit or 64-bit ARM | Match the device: 32-bit uses v7a, 64-bit uses arm64 |
| Video playback | H.264 support | H.264 and HEVC support; other formats depend on the TV or box. |
| Network | The TV can reach Emby | Same LAN, or a stable remote link |
| Storage | About 100 MB for an ABI build | Leave room for artwork and the playback cache |

The interface is designed for 1080p. 4K sets work.

## Feedback

Android TV builds vary widely, and physical-device coverage is limited, so a stable release can still hit a compatibility issue. Please install the latest Release.

Open an [issue](https://github.com/skymei/VisInkAndroidTVRelease/issues), or email [support@visink.cc](mailto:support@visink.cc).

Include the Android version, the VisInk version, the TV or box model, the media format, the steps, what you expected, and what happened. A screenshot or screen recording helps.
