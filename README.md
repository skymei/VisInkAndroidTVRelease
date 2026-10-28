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
  <img src="docs/screens/immersive.jpg" alt="沉浸轮播" width="44%" />
</p>
<p align="center"><sub>空闲后进入沉浸轮播</sub></p>

<p align="center">
  <img src="docs/screens/home.jpg" alt="首页" width="30%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="剧集详情" width="30%" />
  &nbsp;
  <img src="docs/screens/library.jpg" alt="媒体库" width="30%" />
</p>
<p align="center"><sub>首页 · 剧集详情 · 媒体库</sub></p>

<p align="center">
  <img src="docs/screens/player.jpg" alt="播放与弹幕" width="30%" />
  &nbsp;
  <img src="docs/screens/player-paused.jpg" alt="暂停" width="30%" />
  &nbsp;
  <img src="docs/screens/search.jpg" alt="搜索" width="30%" />
</p>
<p align="center"><sub>播放与弹幕 · 暂停 · 跨服务器搜索</sub></p>

---

## 能力

媒体资源在你的 Emby 服务器上。本应用只负责电视端的登录、浏览和播放。

### 浏览

- 多服务器、多账号，会话持久保存
- 登录页管理线路：名称、协议、账号密码和延迟显示
- 服务器头像：内置图标按名称搜索，也可导入图标库
- 首页与「我的」：继续观看、收藏、收藏人物和观看统计
- 空闲自动进入沉浸轮播，超时与轮播时保持亮屏可设
- 媒体库单页滚动，按观看状态筛选和排序
- 搜索当前服务器或全部服务器，聚合搜索可在设置关闭
- 电影 / 剧集详情、分季选集、人物页

### 播放

- 优先直连，设备不支持时由服务器转码；可设码率上限
- 视频硬解；音频可选自动、软件或系统解码，覆盖 AAC、AC3、EAC3、DTS、TrueHD
- 多声道按输出设备降混；音轨、字幕、线路和解码都能在播放中切换
- 面板里有章节和选集，倍速与快进步长（5–60 秒）可调
- 记住每部影片的倍速、音轨、字幕和版本，可在设置关闭
- 片头片尾可分别设为自动跳过，片尾能返回并定位刚播完的一集
- 控件隐藏时按确认键暂停，返回需两秒内连按两次才退出
- 播放背景取图：默认开启，详情页和首页 Hero 用屏上已显示的封面作开场图

### 字幕与弹幕

- 文本字幕 SRT、VTT、ASS / SSA，大小、位置、颜色可调，双语分别配色
- 图形字幕 PGS、DVB、VobSub
- 播放中可临时提前或延后字幕，也可在线搜索 ASSRT 字幕并自填密钥
- 弹幕跟随影片时间，支持弹弹play 官方来源和自定义来源
- 弹幕可自动匹配或手动搜索，样式、密度、时间偏移可调，匹配跨集记住

### 网络与代理

- 全局代理统一转发 Emby、弹幕和应用请求，也可按线路或弹幕单独覆盖
- 每条线路可设 HTTP / SOCKS 代理和自定义名称
- 代理、弹幕服务、图标库地址都能用手机扫码填写

### 应用

- 界面文字小 / 中 / 大三档；语言可跟随系统，另支持简繁中文、英、日、韩、西、法、德
- 节能模式：降低图片尺寸与并发加载，缓解低配设备卡顿
- 按类别清理音视频、图片、字幕、弹幕和更新包缓存，不影响登录和设置
- 启动时检查更新（可关），覆盖安装保留已登录的服务器
- 关于页可查看开源许可

## 媒体格式

默认让电视或盒子直接播放原片，设备不支持时再由 Emby 转成兼容格式。电视支持杜比视界，是播放杜比视界片源的前提。

| 类型 | 支持 | 说明 |
|---|---|---|
| 视频 | H.264 / AVC | MP4、M4V、MOV、MKV、TS，兼容性最好 |
| 视频 | HEVC / H.265 | MP4、MKV、TS，常见 4K、Main10 和 HDR 片源通常可播 |
| 视频 | AV1、VP8 / VP9 | MP4、MKV、WebM，需设备支持对应解码 |
| 画面 | SDR、HDR10、HDR10+、HLG | 需设备支持对应的 HDR 显示 |
| 杜比视界 | Profile 5、8 / 8.1 | 画面交给设备输出，可能触发电视的杜比视界效果 |
| 杜比视界 | Profile 7、8.4、4 | 视片源和设备而定，Profile 7 部分会以 HDR10 播放 |
| 音频 | AAC、AC-3、E-AC-3、MP3、FLAC、Opus、Vorbis、DTS、DTS-HD、TrueHD、ALAC、WMA、PCM | Atmos、DTS:X 能否输出取决于设备与 HDMI / eARC |
| 封装 | MP4、M4V、MOV、MKV、WebM、TS、HLS | 后缀只是外包装，内部格式仍影响能否直连 |

VC-1、WMV3、ProRes、12-bit 或 4:2:2 / 4:4:4 的 HEVC，以及 ISO、BDMV、RM、RMVB 更容易触发转码；分辨率、码率、帧率、音轨或字幕超出设备能力时也会转码。

转码后画面可能不再保留杜比视界或 HDR10+ 的动态效果。播放时打开「媒体信息」，可查看当前是直接播放、直接串流还是服务器转码。

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
