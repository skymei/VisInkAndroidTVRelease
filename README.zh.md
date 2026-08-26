[English](README.md) | **中文**

# VisInk Android TV

面向 Android 电视的 Emby 客户端。免费侧载，不上 Google Play，也没有订阅或内购。

安装包不放在默认分支里。请到 [Releases](https://github.com/skymei/VisInkAndroidTVRelease/releases)（也就是各个 tag）下载对应版本的 APK。

## 选哪个包

| 文件 | 适用 |
|---|---|
| `VisInk-*-armeabi-v7a.apk` | 32 位 ARM。**电视优先选这个** |
| `VisInk-*-arm64-v8a.apk` | 64 位 ARM |
| `VisInk-*-universal.apk` | 含全部 ABI，体积最大；架构不确定时用 |

需要 Android TV（Leanback），Android 7.0 及以上。包名是 `com.skymei.visink`。

覆盖安装即可更新，不要卸载再装：卸载会清掉本机保存的服务器和登录态。各版本支持的功能写在对应 tag / Release 说明里。

## 能做什么

连自己的 Emby 服务器之后，可以用遥控器浏览首页、媒体库、搜索、影片/剧集/人物详情、继续观看与收藏，并播放（直连优先，必要时回退或转码）。设置里可改外观、播放、搜索和界面语言。
