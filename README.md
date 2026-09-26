<p align="center">
  <img src="assets/frameport-icon.png" width="104" height="104" alt="FramePort 应用图标">
</p>
<h1 align="center">FramePort</h1>
<p align="center">影像港口 · 把拍过的素材，安心带回 Mac。</p>
<p align="center"><strong>简体中文</strong> · <a href="README.en.md">English</a></p>
<p align="center">
  <img src="https://img.shields.io/badge/release-0.88%20Beta%201-B85C1A?labelColor=4B4B4B" alt="0.88 Public Beta 1">
  <img src="https://img.shields.io/badge/Mac-Apple%20Silicon-686868?labelColor=4B4B4B" alt="Apple Silicon">
  <img src="https://img.shields.io/badge/macOS-15%2B%20declared-686868?labelColor=4B4B4B" alt="声明最低 macOS 15">
</p>
<h3 align="center"><a href="https://github.com/j1374483500-dot/FramePort-Releases/releases/download/v0.88.0-beta.1/FramePort-0.88-beta.1-macOS-arm64.zip">下载 Mac 版 · Public Beta 1</a></h3>
<p align="center">
  <a href="https://github.com/j1374483500-dot/FramePort-Releases/releases/tag/v0.88.0-beta.1">版本说明与校验信息</a> ·
  <a href="https://github.com/j1374483500-dot/FramePort-Releases/issues/new/choose">提交反馈</a>
</p>

---

FramePort 是面向个人摄影用户的轻量 macOS 素材工具。从存储卡和文件夹导入照片、视频与录音，完成校验，再按需生成便于携带的照片和视频副本。**核心做深，选项做少。**

## 从存储卡，到整理好的素材

| 功能 | 你可以做什么 |
| :--- | :--- |
| **导入与整理** | 按拍摄日期选择素材，预览文件名与保存位置，再确认导入。 |
| **校验与备份** | 复制后进行 SHA-256 校验，可另选一个备份位置，分别查看结果。 |
| **独立压缩** | 拖入照片或视频，生成 HEIC / MP4 轻量副本。保留原件，无需建立相册。 |
| **清楚的处理结果** | 逐文件更新结果，取消后保留已完成的副本，继续处理未完成项。 |

媒体处理在本机完成。当前专注素材输入与整理，不提供 AI 分析、手机连接或照片库云同步。

## 三步开始

1. **下载**上方 ZIP，在同一版本页面查看 SHA-256 校验信息。
2. **安装**：解压，将 **FramePort.app** 拖入“应用程序”，再打开。
3. **试用**：先用少量已有备份的素材，完成一次导入或压缩并检查结果。请保留原件。

> **首次打开：** 本版使用 ad-hoc 签名，尚未获得 Apple 公证，Gatekeeper 检查未通过。核实下载来源与文件完整性后，如决定继续，可在尝试打开后查看“系统设置 → 隐私与安全性”是否提供针对 FramePort 的“仍要打开”。入口可能不可用；请参阅 [Apple 官方指南](https://support.apple.com/en-us/102445)。

**适用环境：** Apple Silicon（M 系列），暂不支持 Intel。声明最低 macOS 15，当前实际验收使用 macOS 27，其他版本待验证。界面支持简体中文与英文，跟随系统首选语言。来源须为可挂载的磁盘或文件夹，暂不支持 PTP / MTP 直连。

## 关于这次公开测试

这是 **0.88 Public Beta 1**，尚非 1.0 稳定版。应用内显示 **0.88 / Build 12**，发布标签为 `v0.88.0-beta.1`。

- **压缩与元数据：** 不承诺无损或固定压缩比例；仅尽量保留原件中已有且可读取的拍摄时间、时区、地点和设备信息，不推测缺失的 GPS。
- **Apple 照片：** iPhone / iCloud 路径尚未验收，部分带小数秒拍摄时间的视频仍可能出现时间偏移。
- **取消与兼容性：** 取消视频压缩偶尔会留下临时目录。能导入某种格式，不代表一定能预览或压缩；不保证保留完整卡结构；真实大批次与最新列表界面的完整实机验收仍待完成。

查看 [已知问题](docs/KNOWN_ISSUES.md) · [本版验证说明](docs/VERIFICATION.md)，了解具体范围与未完成的验收。

## 一起把它做得更顺手

我们尤其想听到这三类反馈：

- **哪里不直觉：** 哪一步让你犹豫，或者不知道接下来该做什么？
- **设备与素材表现：** 安装、读卡、常见格式或长批次哪里遇到问题？
- **输出是否符合预期：** 文件大小、观看效果，以及照片中的时间和地点是否正确？

[报告问题](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) · [分享使用感受](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=feedback.yml)

GitHub Issues 公开可见。无需提供个人素材或完整日志；截图与样本均为可选，请先去除人名、身份信息、完整路径、序列号和精确地点。

---

本仓库仅提供安装包、文档与反馈入口，源码保持私有。GitHub 自动生成的 **Source code** 压缩包仅包含这个公开仓库的文档与素材，**不是应用安装包或应用源码**。使用条款见 [LICENSE](LICENSE)，第三方数据说明见 [THIRD_PARTY_NOTICES](THIRD_PARTY_NOTICES.md)。
