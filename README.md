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

媒体资源在你的 Emby 服务器端。本项目只提供 Emby 客户端登录、播放能力。

安装包在 [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases) 里，也就是各个 tag 下面，请务必安装最新的 Release 版本，Pre-Release 版本是测试版，可能会有各种问题，更新时直接覆盖安装，不要先卸载，否则要重新登录你应用内已经登录过的服务器。

## 安装

| 文件 | 说明 |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32 位 ARM，**电视一般下这个** |
| `VisInk-*-arm64-v8a.apk` | 64 位 ARM |
| `VisInk-*-universal.apk` | 通用包，体积最大。不确定芯片再下这个 |

## 运行环境

| | 最低配置 | 推荐配置 |
|---|---|---|
| 系统 | Android **7.0**（API 24） | Android **12** 或更新 |
| 设备 | 带电视桌面、能用方向键遥控器的电视或盒子（Android TV、Google TV 等）。不支持手机和平板 | 客厅常用的 1080p 或 4K 电视 / 盒子 |
| 芯片 | ARM 32 位或 64 位 | 和电视一致：32 位下 v7a，64 位下 arm64 |
| 解码 | 能硬解 H.264 | 能硬解 H.264、HEVC |
| 网络 | 电视能访问 Emby | 同一局域网，或远程网络稳定 |
| 空间 | 约 100 MB（单架构包） | 再留一点给封面缓存即可 |

界面按 1080p 电视做的，4K 也能用。

## 当前版本能力

- 登录 Emby，保存会话
- 多服务器、多账号
- 首页、媒体库、搜索
- 影片 / 剧集详情
- 人物页
- 继续观看、收藏
- 直连播放；本机解不了再转码
- 字幕、音轨、倍速、下一集
- 外观、播放、搜索设置
- 简体中文、繁体中文、英语、日语、韩语等界面语言

## 反馈

项目还在起步，用着不顺还请担待。

安卓 TV 系统繁杂，开发者没有足够的真机 TV 去做完整的测试，在部分真机和模拟器的联合测试下仍然可能有很多的不兼容问题，请下载正式 release 版本使用，如果有问题可以提 [Issue](https://github.com/skymei/VisInkAndroidTVRelease/issues)，或者发邮件到 [support@visink.cc](mailto:support@visink.cc)。

报问题，请尽量写细一点：用的哪一版、什么电视或盒子、媒体资源格式是什么，怎么操作的、预期怎样、实际怎样。有截图或录屏更好，方便我们排查修复。
