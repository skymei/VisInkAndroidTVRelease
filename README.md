<h1 align="center">
  <img src="docs/logo-ink.png#gh-light-mode-only" height="28" width="28" alt="VisInk" />
  <img src="docs/logo.png#gh-dark-mode-only" height="28" width="28" alt="VisInk" />
  VisInk
</h1>

<p align="center">
  <strong>中文</strong> · <a href="README.en.md">English</a>
</p>

<p align="center">
  面向 Android TV 的 Emby 客户端，免费使用。
</p>


<p align="center">
  <img src="https://img.shields.io/badge/Kotlin-2.2.10-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin 2.2.10" />
  &nbsp;
  <img src="https://img.shields.io/badge/Android-7.0%2B-3DDC84?logo=android&logoColor=white" alt="Android 7.0+" />
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><img src="https://img.shields.io/github/v/release/skymei/VisInkAndroidTVRelease?label=%E6%9C%80%E6%96%B0%E7%89%88" alt="最新版本" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases"><img src="https://img.shields.io/github/downloads/skymei/VisInkAndroidTVRelease/total?label=%E4%B8%8B%E8%BD%BD%E6%AC%A1%E6%95%B0" alt="下载次数" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><img src="https://img.shields.io/github/downloads/skymei/VisInkAndroidTVRelease/latest/total?label=%E6%9C%AC%E7%89%88%E4%B8%8B%E8%BD%BD" alt="本版下载" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/stargazers"><img src="https://img.shields.io/github/stars/skymei/VisInkAndroidTVRelease?style=flat" alt="Star" /></a>
  &nbsp;
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/issues"><img src="https://img.shields.io/github/issues/skymei/VisInkAndroidTVRelease?label=Issues" alt="Issues" /></a>
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases"><strong>下载安装包</strong></a>
</p>

<p align="center">
  <img src="docs/screens/immersive.jpg" alt="沉浸轮播" width="960" />
</p>
<p align="center"><sub>空闲后进入沉浸轮播</sub></p>

<p align="center">
  <img src="docs/screens/home.jpg" alt="首页" width="48%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="剧集详情" width="48%" />
</p>
<p align="center"><sub>首页 · 剧集详情</sub></p>

<p align="center">
  <img src="docs/screens/player.jpg" alt="播放与弹幕" width="48%" />
  &nbsp;
  <img src="docs/screens/player-paused.jpg" alt="暂停" width="48%" />
</p>
<p align="center"><sub>播放与弹幕 · 暂停</sub></p>

<p align="center">
  <img src="docs/screens/library.jpg" alt="媒体库" width="48%" />
  &nbsp;
  <img src="docs/screens/search.jpg" alt="搜索" width="48%" />
</p>
<p align="center"><sub>媒体库 · 跨服务器搜索</sub></p>

<p align="center">
  <img src="docs/screens/settings.jpg" alt="播放设置" width="960" />
</p>
<p align="center"><sub>播放设置：码率、字幕、弹幕与解码</sub></p>

---

## 能力

媒体资源在你的 Emby 服务器上。本项目只提供电视端的登录、浏览和播放。

### 浏览

- 登录 Emby 并保持会话，支持多台服务器、多个账号
- 可为服务器线路单独配置代理
- 首页、空闲沉浸轮播、继续观看、收藏和收藏人物
- 媒体库浏览，可按观看状态筛选和排序
- 搜索当前服务器，或一次搜索已保存的全部服务器；支持手机扫码输入
- 电影 / 剧集详情、分季选集、人物页

### 播放

- 优先直连播放；电视解不了时，再由服务器转码
- 可设置播放码率上限
- 视频硬件解码；音频可在自动、软件解码、系统解码之间切换，覆盖 AAC、AC3、EAC3、DTS、TrueHD 等常见格式
- 音轨、倍速、多级快进和快退
- 记住同一部电影或剧集的倍速、音轨、字幕和版本
- 片头、片尾和下一集
- 播放中可以切换线路

#### 媒体格式支持

应用会优先让电视或盒子直接播放原始片源。只要电视或盒子支持对应格式，大多数常见资源都可以直接播放；设备不支持时，Emby 服务器可能会先转换成兼容格式。电视支持杜比视界，是播放杜比视界片源的前提，但不同片源的 Profile、封装方式和音轨仍可能影响最终效果。

| 类型 | 可播放范围 | 说明 |
|---|---|---|
| 视频 | H.264 / AVC | MP4、M4V、MOV、MKV、TS；兼容性最好，也是服务器转换时最常用的格式 |
| 视频 | HEVC / H.265 | MP4、MKV、TS；常见的 4K、Main10 和 HDR 片源通常可以播放，具体取决于电视或盒子的能力 |
| 视频 | AV1 | MP4、MKV、WebM；需要电视或盒子支持 AV1 解码 |
| 视频 | VP8 / VP9 | MKV、WebM；需要电视或盒子支持对应解码 |
| 画面 | SDR、HDR10、HDR10+、HLG | 需要电视或盒子支持对应的 HDR 显示效果 |
| 杜比视界 | 常见 Profile 5、Profile 8 / 8.1 | 电视或盒子支持对应 Profile 时，可以把杜比视界画面交给设备输出，并可能触发电视的杜比视界效果；Sony X90L 等设备请以实际片源验证 |
| 杜比视界 | Profile 7 | 部分片源会以 HDR10 播放，是否能保持完整杜比视界效果取决于片源和设备 |
| 杜比视界 | Profile 8.4、Profile 4 | 部分电视和片源可以播放，兼容性需要以实际设备为准 |
| 音频 | AAC、AC-3、E-AC-3、MP3、FLAC、Opus、Vorbis、DTS、DTS-HD、TrueHD、ALAC、WMA、PCM | 常见音轨可以播放；Atmos、DTS:X 是否能由电视、功放或回音壁输出，取决于设备和 HDMI/eARC 连接方式 |
| 文件和在线播放 | MP4、M4V、MOV、MKV、WebM、TS、HLS | 文件后缀只代表外包装，里面的视频、音频和字幕格式仍会影响能否直接播放 |

以下资源更容易需要服务器转换：VC-1、WMV3、ProRes，12-bit 或 4:2:2 / 4:4:4 的 HEVC，以及 ISO、BDMV、RM、RMVB 等格式。片源的分辨率、码率、帧率、音轨或字幕超出设备能力时，也可能触发转换。

服务器转换后，画面可能不再保留杜比视界或 HDR10+ 的动态效果。播放时打开“媒体信息”，可以看到当前是直接播放、直接串流还是服务器转换。

### 字幕与弹幕

- 文本字幕：SRT、VTT、ASS / SSA。可调整大小、位置和颜色
- 图形字幕：PGS、DVB、VobSub
- 播放中可对当前字幕微调提前或延后
- 可接入 ASSRT 在线字幕
- 弹幕跟随影片时间，支持自动匹配、手动搜索、样式和偏移
- 可添加兼容的弹幕服务，并用手机扫码填写地址

### 应用

- 外观皮肤，以及小、中、大三档文字
- 界面语言：跟随系统、简体中文、繁体中文、英语、日语、韩语、西班牙语、法语、德语
- 按类别清理音视频、图片、字幕、弹幕和更新包缓存，不影响登录和设置
- 从 GitHub 检查正式版，覆盖安装并保留已登录的服务器

## 安装

安装包在 [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases)。请安装最新的正式版。Pre-Release 是测试版，不建议日常使用。更新时直接覆盖安装，不要先卸载，否则需要重新登录已经保存的服务器。

| 文件 | 说明 |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32 位 ARM。**多数电视安装这个。** |
| `VisInk-*-arm64-v8a.apk` | 64 位 ARM |
| `VisInk-*-universal.apk` | 通用包，体积最大。不确定芯片时再用 |

## 运行环境

| | 最低 | 推荐 |
|---|---|---|
| 系统 | Android **7.0**（API 24） | Android **12** 或更新 |
| 设备 | 带电视桌面、能用方向键的电视或盒子。不支持手机和平板 | 日常使用的 1080p 或 4K 电视 / 盒子 |
| 芯片 | ARM 32 位或 64 位 | 与设备一致：32 位用 v7a，64 位用 arm64 |
| 视频播放 | 支持 H.264 | 支持 H.264、HEVC；其他格式以电视或盒子的实际能力为准 |
| 网络 | 电视能访问 Emby | 同一局域网，或稳定的远程连接 |
| 空间 | 约 100 MB（单架构包） | 再留一些给封面和播放缓存 |

界面按 1080p 电视设计，4K 电视可以使用。

## 反馈

Android TV 的系统差异很大，真机覆盖有限，正式版仍可能遇到兼容问题。请安装最新的 Release。

遇到问题可以提 [Issue](https://github.com/skymei/VisInkAndroidTVRelease/issues)，或发邮件到 [support@visink.cc](mailto:support@visink.cc)。

请尽量写上这些信息：Android 版本、VisInk 版本、电视或盒子型号、片源格式、操作步骤、预期结果和实际结果。截图或录屏能帮助定位。
