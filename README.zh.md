<p align="center">
  <img src="docs/logo.png" width="92" alt="VisInk" />
</p>

<p align="center">
  <a href="README.md">English</a> · <strong>中文</strong>
</p>

<h1 align="center">VisInk</h1>

<p align="center">
  多媒体客户端，连你自己的片库。<br/>
  这里是 <strong>Android 电视版的免费安装包</strong>，侧载即可，不上架商店，不收费。
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><strong>下载最新版</strong></a>
</p>

---

<p align="center">
  <img src="docs/screens/home.jpg" alt="首页" width="920" />
</p>
<p align="center"><sub>首页</sub></p>

<p align="center">
  <img src="docs/screens/welcome.jpg" alt="欢迎页" width="48%" />
  &nbsp;
  <img src="docs/screens/login.jpg" alt="登录" width="48%" />
</p>
<p align="center"><sub>欢迎页 · 登录</sub></p>

<p align="center">
  <img src="docs/screens/search.jpg" alt="搜索" width="48%" />
  &nbsp;
  <img src="docs/screens/detail.jpg" alt="详情" width="48%" />
</p>
<p align="center"><sub>搜索 · 详情</sub></p>

<p align="center">
  <img src="docs/screens/mine.jpg" alt="我的" width="48%" />
  &nbsp;
  <img src="docs/screens/settings.jpg" alt="设置" width="48%" />
</p>
<p align="center"><sub>我的 · 设置</sub></p>

---

VisInk 不提供片源。片在你的 Emby 上，电视上装这个客户端，用遥控器看。安装包在 [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases)（也就是各个 tag）里，默认分支没有 APK。更新请直接覆盖安装，**别先卸载**：卸了本机登录和服务器记录就没了。

## 下哪个包

| 文件 | 什么时候用 |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32 位 ARM。**电视优先下这个。** |
| `VisInk-*-arm64-v8a.apk` | 64 位 ARM |
| `VisInk-*-universal.apk` | 三种架构都打进去，体积最大。搞不清再选这个。 |

包名：`com.skymei.visink`。

## 系统版本和硬件

| | 最低 | 推荐 |
|---|---|---|
| 系统 | Android TV / Google TV **7.0**（API 24） | Android TV / Google TV **12** 及以上 |
| 设备 | 带电视桌面、能用方向键遥控器的电视或盒子。手机和平板装不了。 | 客厅里日常在用的电视或盒子，1080p 或 4K |
| CPU | 32 位 ARM（`armeabi-v7a`）或 64 位 ARM（`arm64-v8a`） | 电视是 32 位就装 v7a 包，64 位就装 arm64 包 |
| 解码 | 至少能硬解常见片源（H.264） | 能硬解 H.264 和 HEVC，片库大多能直连，少转码 |
| 网络 | 电视能访问到你的 Emby | 有线或稳定 Wi-Fi，别跟服务器隔着很差的链路 |
| 存储 | ABI 包大约 100 MB；全量包大约 250 MB | 同样够用，再留一点给封面缓存 |

界面按 1080p 电视来的，4K 电视也能用。这不是手机 APK。

## 这个版本能做什么

- 登 Emby、下次自动进、切最近用过的服务器和账号
- 欢迎页、首页、媒体库、搜索、全部搜索
- 电影 / 剧集详情、人物页；单集卡片直接播，没有单独的单集页
- 继续看、收藏
- 播放：能直连就直连，不行再走本机解码或 libVLC，再不行让服务器转码；暂停、进度、字幕、音轨、倍速、下一集、媒体信息都有
- 设置：外观、播放、搜索、界面语言、关于
- 语言：跟随系统，或简体中文 / 繁体中文 / English / 日本語 / 한국어 / Español / Français / Deutsch
