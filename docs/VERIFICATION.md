# 本版验证说明 / Verification

适用于 **0.88 Public Beta 1**（应用内版本 0.88 / Build 12）。

## 已有证据

- 本版功能源码的最终完整 XCTest 回归：**391 项通过、0 失败**。发布准备核对了全部 221 项测试输入文件，与该轮测试保持一致。
- 本次公开安装包从相同的功能源码重新构建，目的是移除个人构建路径和不必要的归档属性；未修改功能、画质或元数据策略。重建本身不计作另一次 391 项测试。
- 公开包检查包括：运行资源一致性、Apple Silicon 架构、声明最低 macOS 15、签名完整性、ZIP 解压后文件一致性和可执行权限。最终文件校验值随 Release 提供。
- 原有文件级测试覆盖源文件不变、目标冲突、压缩结果回读、拍摄元数据、取消与重试等行为；不是对所有相机或系统组合的保证。

## 尚未证明的范围

- 较早的同轮全量测试出现过一次取消时临时目录残留，后续测试通过，但原因未定位，仍属于已知问题。
- 最新批次列表的完整真实窗口与键盘／VoiceOver验收、实体设备断连、长视频与大批真实素材、另一台 Mac 和最低系统版本测试仍待完成。
- 部分 Mac 照片合成小样有日期／GPS往返证据；iPhone 导入、iCloud 同步及带小数秒视频的 Photos 兼容性仍有待验事项。
- 安装包仅有 ad-hoc 签名，未获得 Developer ID 签名或 Apple 公证，Gatekeeper 评估未通过。签名完整性通过不代表 Apple 已审核或公证。

具体范围见[已知问题](KNOWN_ISSUES.md)。SHA-256 校验值用于核对下载完整性，不代表安全认证或格式兼容认证。

## English

The final full XCTest run for this functional source passed **391 tests with zero failures**. All 221 tested input files were rechecked unchanged for publication. The public package was rebuilt from that same source to remove personal build paths and archive attributes; no functional, quality or metadata policy changed, and this rebuild is not counted as another test run.

Packaging checks cover resource consistency, arm64 architecture, the declared macOS 15 minimum, signature integrity, extracted-file equality and executable permission. Release assets include checksums. An earlier full test run reproduced intermittent cancellation residue; later passes do not establish a fix. Real-device/large-batch behavior, the newest row UI and complete accessibility, another Mac/minimum OS, iPhone/iCloud and fractional-second Photos behavior remain unverified or unresolved.

This is an ad-hoc-signed, non-notarized beta. Passing signature integrity checks is not Apple approval, and Gatekeeper assessment was rejected. Checksums verify file integrity, not safety certification or universal compatibility.
