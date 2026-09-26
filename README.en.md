<p align="center">
  <img src="assets/frameport-icon.png" width="104" height="104" alt="FramePort app icon">
</p>
<h1 align="center">FramePort</h1>
<p align="center">Bring what you captured home to your Mac.</p>
<p align="center"><a href="README.md">简体中文</a> · <strong>English</strong></p>
<p align="center">
  <img src="https://img.shields.io/badge/release-0.88%20Beta%201-B85C1A?labelColor=4B4B4B" alt="0.88 Public Beta 1">
  <img src="https://img.shields.io/badge/Mac-Apple%20Silicon-686868?labelColor=4B4B4B" alt="Apple Silicon">
  <img src="https://img.shields.io/badge/macOS-15%2B%20declared-686868?labelColor=4B4B4B" alt="Declared minimum macOS 15">
</p>
<h3 align="center"><a href="https://github.com/j1374483500-dot/FramePort-Releases/releases/download/v0.88.0-beta.1/FramePort-0.88-beta.1-macOS-arm64.zip">Download for Mac · Public Beta 1</a></h3>
<p align="center">
  <a href="https://github.com/j1374483500-dot/FramePort-Releases/releases/tag/v0.88.0-beta.1">Release notes &amp; checksums</a> ·
  <a href="https://github.com/j1374483500-dot/FramePort-Releases/issues/new/choose">Share feedback</a>
</p>

---

FramePort is a lightweight macOS media tool for individual photographers. Import photos, videos and audio from cards or folders, verify your copies, and optionally create smaller photo and video files to take with you. **A focused workflow, with fewer choices to make.**

## From memory card to organized media

| Feature | What it does |
| :--- | :--- |
| **Import and organize** | Select capture dates, preview file names and destinations, then confirm the import. |
| **Verify and back up** | Check copies with SHA-256, optionally choose a second backup location, and see each result. |
| **Compress directly** | Drop in photos or videos to create smaller HEIC / MP4 copies. Keep your originals; no album setup needed. |
| **See each result** | Results appear as files finish. Cancel without losing completed copies, then continue unfinished items. |

Media processing runs locally. This release focuses on importing and organizing; it does not include AI analysis, phone connections or cloud photo sync.

## Get started in three steps

1. **Download** the ZIP above. SHA-256 verification information is on the same release page.
2. **Install:** unzip, drag **FramePort.app** into Applications, and open it.
3. **Try it:** start with a few backed-up files, complete an import or compression, and check the results. Keep your originals.

> **First launch:** This beta is ad-hoc signed, not notarized by Apple, and did not pass Gatekeeper assessment. After verifying the download source and file integrity, you may choose to try the app-specific **Open Anyway** option in System Settings → Privacy & Security after attempting to open FramePort. That option may be unavailable; see [Apple’s instructions](https://support.apple.com/en-us/102445).

**Requirements:** Apple Silicon (M series); no Intel build. The declared minimum is macOS 15; current acceptance testing used macOS 27, and other versions remain unverified. English and Simplified Chinese follow your preferred system language. Sources must be mounted storage or folders; PTP / MTP connections are not supported.

## About this public beta

This is **0.88 Public Beta 1**, not a stable 1.0 release. The app reports **0.88 / Build 12**; the release tag is `v0.88.0-beta.1`.

- **Compression and metadata:** Compression is not guaranteed to be lossless or achieve a fixed reduction. Capture time, time zone, location and device information can only be retained when present and readable. Missing GPS is not inferred.
- **Apple Photos:** iPhone / iCloud paths have not been validated. Some video dates with fractional seconds can still be interpreted with a time offset.
- **Cancellation and compatibility:** Cancelling video compression can occasionally leave a temporary folder. Import support does not guarantee preview or compression support. Complete card structures are not guaranteed. Large real-world batches and full native-window acceptance of the newest list UI remain outstanding.

Read the [known issues](docs/KNOWN_ISSUES.md#english) and [verification notes](docs/VERIFICATION.md) for the scope and outstanding acceptance checks.

## Help make it feel effortless

Three kinds of feedback are especially useful:

- **Where you hesitated:** Which step felt confusing, or left you unsure what to do next?
- **Your devices and files:** Did installation, card import, common formats or a long batch cause trouble?
- **The finished copies:** Were file size, viewing quality, capture time and location what you expected?

[Report a bug](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=bug_report.yml) · [Share your experience](https://github.com/j1374483500-dot/FramePort-Releases/issues/new?template=feedback.yml)

GitHub Issues are public. Personal footage and full logs are not required; screenshots and samples are optional. Redact names, identifying information, full paths, serial numbers and precise locations before sharing.

---

This repository provides downloads, documentation and feedback only; the app’s source code remains private. GitHub’s automatic **Source code** archives contain only this public repository’s documentation and assets, **not the app installer or app source**. See [LICENSE](LICENSE) for usage terms and [THIRD_PARTY_NOTICES](THIRD_PARTY_NOTICES.md) for third-party data attribution.
