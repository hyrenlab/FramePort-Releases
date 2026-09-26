# 已知问题 / Known issues

适用于 **FramePort 0.88 Public Beta 1**（`v0.88.0-beta.1`，应用内 0.88 / Build 12）。这是公开测试版，尚非 1.0 稳定版。

| 范围 | 当前状态与建议 |
| --- | --- |
| 安装 | Apple Silicon 包使用 ad-hoc 签名，未公证，Gatekeeper 检查未通过。可信来源与文件完整性确认后，可按 [Apple 官方指南](https://support.apple.com/en-us/102445) 检查系统提供的单应用“仍要打开”入口；部分系统环境可能仍无法打开。 |
| 系统与设备 | 声明最低 macOS 15，当前验收使用 macOS 27。尚未完成其他 macOS 版本、另一台 Mac 及广泛真实设备验收；不提供 Intel 包。来源须为可挂载磁盘或文件夹，PTP / MTP 直连未实现。 |
| Apple 照片时间与地点 | 部分 Mac 照片样本已验证，不能代表全部文件。带小数秒拍摄时间的视频仍可能出现时间偏移；iPhone 导入及 iCloud 同步尚未验收。需要正确归档时，请检查照片信息页的拍摄日期和地图。“最近添加”按导入顺序显示，不能单独用来判断拍摄时间是否丢失。 |
| 视频取消清理 | 取消视频压缩时偶尔留下 `.work` 临时目录，原因仍在调查，尚未修复。已复现测试中的原件保持不变，未发布未完成的最终副本；这不代表所有中断场景都已验收。遇到时请报告取消时的阶段和大致等待时间，不要随意删除无法确认用途的目录。 |
| 批次界面与长任务 | 逐文件结果、继续未完成和处理阶段已有自动化覆盖；最新列表行的完整真实窗口验收仍待完成。千级真实素材、长视频、设备断连及其他 Mac 上的表现仍需要反馈。 |

## 格式与压缩边界

- 原件按原始字节复制、校验；压缩副本独立保存。照片压缩输出 HEIC，视频输出 MP4，压缩比例因素材而异，不等同于画质损失比例。
- RAW 渲染和媒体解码能力取决于 macOS。识别并原样导入一个文件，不保证能够预览或压缩它。
- 副本只保留原件中可读取、可移植的信息。缺失的拍摄时间、时区或 GPS 不会靠猜测补齐；厂商私有字段可能无法移入副本。
- 不承诺完整卡镜像或完整剪辑素材包：部分代理、专有容器和配套结构不在导入范围。需要完整卡结构时，请另外保留原卡备份。
- 独立压缩接受单独照片和视频，不递归处理文件夹，也不压缩独立音频；当前批次可继续未完成项，但不提供跨重启的独立压缩作业恢复。
- 旧压缩副本不会自动改写。需要应用本版元数据处理时，应从原件重新生成一份，并核对目标照片应用中的结果。

## 反馈时提供什么

[报告问题](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) 时，写明 macOS 版本、Mac 芯片、相关设备或文件格式、操作步骤、期望结果及实际结果即可。对于相册时间问题，请同时说明导入路径，以及差异来自照片信息页还是“最近添加”列表。

不需要上传私人素材或完整日志。GitHub Issues 公开可见；截图、文件名、路径、设备序列号、GPS 坐标和其他个人信息请先脱敏。只有在你愿意且有权分享时，才附上最小化、无隐私的样本。

## English

This applies to **FramePort 0.88 Public Beta 1** (`v0.88.0-beta.1`; in-app version 0.88 / Build 12), not a stable 1.0 release.

- **Installation:** Apple Silicon only; ad-hoc signed, not notarized, and rejected by Gatekeeper assessment. If you trust the source and have checked file integrity, follow [Apple’s app-specific opening guidance](https://support.apple.com/en-us/102445). The exception may be unavailable in some environments.
- **Compatibility:** The declared minimum is macOS 15. Current acceptance testing used macOS 27; other releases, another Mac and broad real-device coverage remain unverified. PTP / MTP connections are not supported; use mounted storage or folders.
- **Photos metadata:** Some Mac Photos samples passed, but fractional-second video dates can still be interpreted with a time offset. iPhone import and iCloud sync have not been validated. Inspect the capture date and map in the photo’s information; Recently Added alone does not establish metadata loss.
- **Cancellation:** Video cancellation can occasionally leave a `.work` temporary folder. The cause is unresolved. Reproduced tests preserved originals and did not publish an unfinished final output; this does not validate every interruption scenario.
- **Batch experience:** Automated tests cover incremental results, retries and progress stages. Full real-window acceptance of the newest list rows, long videos, large real batches and device disconnection remains outstanding.
- **Format boundaries:** Import support does not guarantee decoding or compression support. Compression is not lossless, and metadata can only be retained when readable and portable. Missing GPS is not inferred. Complete camera-card structures and editing packages are not guaranteed. Standalone compression accepts individual photos/videos, not recursive folders or audio, and its jobs do not resume across app restarts. Existing copies are not rewritten automatically.

A useful report describes your macOS version, Mac chip, relevant device or format, steps, expected result and actual result. Personal footage and full logs are not required. Issues are public; redact identifying names, paths, serial numbers, precise locations and other personal data before sharing anything.
