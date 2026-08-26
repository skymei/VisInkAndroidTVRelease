<p align="center">
  <img src="docs/logo.png" width="92" alt="VisInk" />
</p>

<p align="center">
  <a href="README.md">English</a> · <strong>中文</strong>
</p>

<h1 align="center">VisInk</h1>

<p align="center">
  <em>为自己的片库准备的多媒体客户端。</em>
</p>

<p align="center">
  VisInk 做的是多媒体客户端：装在你的电视上，连<strong>你自己的</strong>媒体服务器，把注意力留给画面。<br/>
  当前仓库是 <strong>Android TV 版本的免费派发仓</strong> —— 签名 APK 放在 GitHub Releases 上，不上 Play 商店，没有订阅，也没有内购。
</p>

<p align="center">
  <a href="https://github.com/skymei/VisInkAndroidTVRelease/releases/latest"><strong>下载最新版本</strong></a>
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

## VisInk 是什么

VisInk 是一个**多媒体客户端品牌**。产品是客厅里的遥控器体验：浏览自己的片库、打开一部作品、在已有的电视上播放。它不是流媒体平台，也不托管你的文件。你提供 Emby 服务器，VisInk 提供电视端应用。

Android TV 客户端面向 Leanback 电视和方向键，通过本仓库免费发放。

## 本仓库是什么

安装包**不放在默认分支**。每个版本对应一个 GitHub Release / tag，下面挂三份已签名 APK。该版本支持的功能写在 tag 说明里。

| 文件 | 适用 |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32 位 ARM。**大多数电视优先选这个。** |
| `VisInk-*-arm64-v8a.apk` | 64 位 ARM |
| `VisInk-*-universal.apk` | 含全部 ABI，体积最大；架构不确定时用 |

包名是 `com.skymei.visink`。需要 **Android TV（Leanback）**，**Android 7.0** 及以上。

覆盖安装即可更新，请用同一签名的新包。**不要先卸载再装** —— 卸载会清掉本机保存的服务器和登录态。

## Android TV 里有什么

- 连接 Emby 服务器、恢复会话、切换最近账号
- 首页、媒体库、搜索、影片 / 剧集 / 人物详情
- 继续观看与收藏
- 播放：直连优先，必要时走设备解码或 libVLC，再必要时由服务器转码
- 设置里可改外观、播放、搜索和界面语言
- 语言：跟随系统，或简体中文 / 繁体中文 / English / 日本語 / 한국어 / Español / Français / Deutsch

不上 Google Play，没有 Play 内购，也没有 Android TV Top Shelf / 系统推荐。
