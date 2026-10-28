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
  <img src="https://img.shields.io/badge/Kotlin-2.2.10-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin 2.2.10" />
  &nbsp;
  <img src="https://img.shields.io/badge/Android-7.0%2B-3DDC84?logo=android&logoColor=white" alt="Android 7.0+" />
  &nbsp;
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
  <img src="docs/screens/home.jpg" alt="Home" width="30%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="Series details" width="30%" />
  &nbsp;
  <img src="docs/screens/library.jpg" alt="Library" width="30%" />
</p>
<p align="center"><sub>Home · Series details · Library</sub></p>

<p align="center">
  <img src="docs/screens/player.jpg" alt="Playback with danmaku" width="30%" />
  &nbsp;
  <img src="docs/screens/player-paused.jpg" alt="Paused" width="30%" />
  &nbsp;
  <img src="docs/screens/search.jpg" alt="Search" width="30%" />
</p>
<p align="center"><sub>Playback with danmaku · Paused · Cross-server search</sub></p>

---

## Capabilities

Your media stays on your Emby server. The app only handles sign-in, browsing, and playback on the TV.

### Browsing

- Multiple servers and accounts with persistent sessions
- Manage lines on the sign-in page: name, protocol, credentials, and latency
- Server avatars from a built-in searchable set, or an imported icon library
- Home and "Mine": continue watching, favorites, favorite people, and watch statistics
- An immersive carousel starts when idle, with configurable timeout and keep-awake
- Library on a single scrolling page, filtered and sorted by watch state
- Search the current server or all saved servers; aggregated search can be turned off
- Movie and series details, seasons and episodes, and person pages

### Playback

- Direct play first; the server transcodes only when the device cannot handle the file. A bitrate ceiling is available.
- Hardware video decode; audio can use automatic, software, or system decode, covering AAC, AC3, EAC3, DTS, and TrueHD
- Multichannel audio is downmixed for the output device; audio tracks, subtitles, lines, and decode mode can be switched during playback
- Chapters and episodes in the player panel; playback speed and seek step (5-60s) are adjustable
- Remembers speed, audio, subtitles, and version per title, and can be turned off in Settings
- Intro and credits can each be skipped automatically; credits can return to the episode that just ended
- Press OK to pause while the controls are hidden; leaving playback takes two Back presses within two seconds
- Playback background artwork, on by default: the detail page and the Home hero reuse the cover already on screen as the opening frame

### Subtitles and danmaku

- Text subtitles SRT, VTT, and ASS / SSA with size, position, and color; dual-language subtitles can use separate colors
- Image subtitles PGS, DVB, and VobSub
- Nudge the current subtitle earlier or later while playing, or search ASSRT online subtitles with your own key
- Danmaku follows the film clock, using the official Dandanplay source or a custom one
- Automatic matching or manual search, with style, density, and timing offset; matches are remembered across episodes

### Network and proxy

- A global proxy forwards Emby, danmaku, and app requests, with per-line or per-danmaku overrides
- An HTTP / SOCKS proxy and a custom name on each line
- Proxy, danmaku service, and icon library addresses can all be filled by scanning a code

### App

- Three interface text sizes; the language can follow the system, with Simplified and Traditional Chinese, English, Japanese, Korean, Spanish, French, and German
- Power-saving mode: smaller artwork and fewer parallel loads for low-end devices
- Clear video, image, subtitle, danmaku, and update caches by category without touching sign-in or settings
- Check for updates at launch (can be turned off); installing over the app keeps your signed-in servers
- Open-source licenses on the About page

## Media formats

The app lets the TV or box play the original file directly and leaves conversion to Emby when the device cannot handle it. Dolby Vision playback requires a TV that supports it.

| Type | Supported | Notes |
|---|---|---|
| Video | H.264 / AVC | MP4, M4V, MOV, MKV, TS; the most compatible option |
| Video | HEVC / H.265 | MP4, MKV, TS; common 4K, Main10, and HDR files usually work |
| Video | AV1, VP8 / VP9 | MP4, MKV, WebM; requires the matching decoder on the device |
| Picture | SDR, HDR10, HDR10+, HLG | Requires the matching HDR display mode |
| Dolby Vision | Profile 5, 8 / 8.1 | The picture is passed to the device and may trigger the TV's Dolby Vision mode |
| Dolby Vision | Profile 7, 8.4, 4 | Depends on the file and device; some Profile 7 files play as HDR10 |
| Audio | AAC, AC-3, E-AC-3, MP3, FLAC, Opus, Vorbis, DTS, DTS-HD, TrueHD, ALAC, WMA, PCM | Atmos and DTS:X output depends on the device and the HDMI / eARC link |
| Container | MP4, M4V, MOV, MKV, WebM, TS, HLS | The extension is only the wrapper; the tracks inside still affect direct play |

VC-1, WMV3, ProRes, 12-bit or 4:2:2 / 4:4:4 HEVC, and ISO, BDMV, RM, or RMVB are more likely to be transcoded. Conversion also kicks in when resolution, bitrate, frame rate, audio, or subtitles exceed what the device can handle.

After conversion, Dolby Vision or HDR10+ dynamic effects may not be preserved. Open "Media Info" during playback to see whether the current route is direct play, direct stream, or server conversion.

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
