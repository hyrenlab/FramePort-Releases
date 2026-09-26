# FramePort / 影像港口

把拍过的素材，安心带回 Mac。

FramePort 是面向个人摄影用户的轻量 macOS 工具：从存储卡和文件夹导入照片、视频与录音，校验文件，并按需生成更便于携带的照片和视频副本。

**0.88 Public Beta 1 · Apple Silicon · 简体中文 / English**

[下载安装包](https://github.com/j1374483500-dot/FramePort-Releases/releases/download/v0.88.0-beta.1/FramePort-0.88-beta.1-macOS-arm64.zip) · [版本说明与校验信息](https://github.com/j1374483500-dot/FramePort-Releases/releases/tag/v0.88.0-beta.1) · [报告问题](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) · [分享使用感受](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=feedback.yml)

这是首次公开测试版，欢迎用一小批已有备份的素材试用，并告诉我们哪里不顺手。测试期间请保留原件。这个仓库只提供安装包、使用说明和反馈入口，源码保持私有。

## 可以做什么

- **拷卡和整理**：选择拍摄日期，预览保存位置与文件名，再确认导入；支持照片、视频和独立录音。
- **校验和备份**：复制后进行 SHA-256 校验，可另选一个备份位置，分别查看保存与备份结果。
- **独立压缩**：拖入照片或视频，选择保存位置，生成 HEIC / MP4 轻量副本。保留原件，不需要建立相册，也没有复杂的画质选项。
- **看清处理结果**：逐文件显示进度与结果，取消后保留已完成的副本，继续处理未完成项。

处理在本机完成。FramePort 负责素材输入与整理，当前不提供 AI 分析、手机连接或照片库云同步。

## 下载与安装

| 项目 | 当前范围 |
| --- | --- |
| 芯片 | Apple Silicon（M 系列）；暂不提供 Intel 版本 |
| 系统 | 声明最低 macOS 15；当前实际验收环境为 macOS 27，其他版本待验证 |
| 语言 | 简体中文、英文，跟随系统首选语言 |
| 来源 | 挂载为磁盘的存储卡、读卡器、设备和本地文件夹；不支持 PTP / MTP 直连 |
| 发布标识 | `v0.88.0-beta.1`；应用内版本为 0.88，Build 12 |

1. 从上方下载 ZIP；可在同一版本页面查看 SHA-256 校验信息。
2. 解压，将 **FramePort.app** 拖入“应用程序”，再打开。
3. 先选择少量有备份的素材完成一次导入或压缩，检查结果后再扩大批量。

**本版使用 ad-hoc 签名，尚未获得 Apple 公证，Gatekeeper 检查未通过。** 下载后可能被 macOS 拦截。如果你已核实下载来源与文件完整性，并决定继续试用，可在尝试打开后，查看“系统设置 → 隐私与安全性”是否提供针对 FramePort 的“仍要打开”。这不是所有环境下都可用的安装保证；具体说明见 [Apple 官方指南](https://support.apple.com/en-us/102445)。若无法打开，请报告系统版本与提示文字。

## 试用前需要知道

- 压缩会改变图像或视频编码，不承诺无损或固定压缩比例。仅尽量保留**原件中已有且可读取**的拍摄时间、时区、地点和设备信息；不会推测原件缺少的 GPS。
- **iPhone / iCloud 路径尚未验收**，部分含小数秒拍摄时间的视频在 Apple 照片中仍有时间偏移问题。
- 取消视频压缩时，偶尔可能留下临时工作目录；此问题尚未修复。
- 能原样导入某种格式，不等于 macOS 一定能预览或压缩它；当前也不适合作为保留完整卡目录结构的专业拷卡工具。

更多范围和状态见 [已知问题](docs/KNOWN_ISSUES.md) 与 [本版验证说明](docs/VERIFICATION.md)。

## 帮我们把它做得更顺手

最想听到的反馈是：**你想完成什么，在哪一步犹豫、出错，或者不知道接下来该做什么。** 安装失败、常见设备与格式的表现、长批次进度，以及时间和地点显示，都很有帮助。

提交 [问题报告](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) 或 [体验反馈](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=feedback.yml) 即可，不需要提供个人照片、视频或日志。GitHub Issues 是公开的；请去掉人名、完整路径、文件名中的身份信息、精确地点和其他隐私。截图和可分享的小样均为可选。

## English

**FramePort is a lightweight media import and compression app for individual photographers on macOS.** Import photos, videos and audio from mounted cards or folders, verify copies with SHA-256, optionally save a second backup, and create smaller HEIC / MP4 copies without changing the originals. Standalone compression also accepts individual photo and video files directly.

**[Download Public Beta 1](https://github.com/j1374483500-dot/FramePort-Releases/releases/download/v0.88.0-beta.1/FramePort-0.88-beta.1-macOS-arm64.zip)** · [Release notes and checksums](https://github.com/j1374483500-dot/FramePort-Releases/releases/tag/v0.88.0-beta.1) · [Report a bug](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) · [Share feedback](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=feedback.yml)

- Apple Silicon only. Declared minimum: macOS 15; current acceptance testing used macOS 27. Other macOS versions and Intel Macs are unverified or unsupported respectively.
- English and Simplified Chinese, following your preferred system language. The app reports version 0.88, Build 12; the public release tag is `v0.88.0-beta.1`.
- Unzip, drag **FramePort.app** into Applications, and open it. This beta is **ad-hoc signed, not notarized, and did not pass Gatekeeper assessment**. After verifying the source and file integrity, you may choose the app-specific **Open Anyway** option in System Settings → Privacy & Security, if available. Follow [Apple’s instructions](https://support.apple.com/en-us/102445); opening is not guaranteed on every Mac.
- Start with a small batch of backed-up files and keep your originals. Compression is not lossless. Capture metadata can only be carried over when it exists and can be read; missing locations are not invented.
- iPhone / iCloud behavior is not yet validated. Some fractional-second video timestamps are interpreted incorrectly by Apple Photos. Cancelling video compression can occasionally leave a temporary working folder. See [known issues](docs/KNOWN_ISSUES.md) and [verification](docs/VERIFICATION.md).
- Media processing is local. There is no AI analysis, phone connection, cloud photo sync, or PTP / MTP camera connection in this release.

This repository contains public downloads, documentation and feedback only. Source code remains private. Issues are public: redact personal data, paths, identifying file names and precise locations. Personal footage and logs are never required to report a problem.
