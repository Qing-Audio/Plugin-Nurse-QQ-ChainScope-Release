# QQ ChainScope 1.7.13

发布日期 / Release date: 2026-09-27

1.7.13 已指定为 Stable。这次修复 TP 低估和 Peak 漏掉短促峰值的问题，并包含 1.7.12 的 Multi Track 按钮缩放修复。

1.7.13 is designated Stable. It fixes underestimated True Peaks and missed short sample peaks, and includes the 1.7.12 Multi Track button scaling fix.

## 修复与行为变化 / Fixes and behavior changes

### 1.7.13 — Stable — 2026-09-27

- 中文：修复 TP 对部分采样点间峰值的低估，采用 ITU-R BS.1770-5 附录 2 的过采样滤波测量；修复 Peak 在两次界面刷新之间漏掉短促峰值的问题。音频处理、路由、EQ Match、延迟和原有 TP 保持／复位规则不变。A/B/C/D 四件套请一起更新。
- English: Fixes underestimated inter-sample True Peaks using the oversampling measurement filter from ITU-R BS.1770-5 Annex 2, and prevents short sample peaks from being missed between display refreshes. Audio processing, routing, EQ Match, latency and the existing TP hold/reset behavior are unchanged. Update all four A/B/C/D plug-ins together.

### 1.7.12 — Stable; public release withdrawn / 已撤回公开发布 — 2026-09-27

- 中文：修复 A Send、B Return、C Mixboard 顶部 Multi Track 按钮缩放不一致、压住相邻按钮的问题。声音处理不变。该版本的发布构建已取消，本次 1.7.13 包含此修复。
- English: Fixes inconsistent scaling of the Multi Track header button in A Send, B Return and C Mixboard, preventing overlap with nearby buttons. Audio processing is unchanged. Its release builds were cancelled; 1.7.13 includes this fix.

## 安装与升级 / Installation and upgrading

每个平台 ZIP 都包含 A Send、B Return、C Mixboard、D Mixboard。先保存工程并关闭宿主，四件套一起覆盖，再重新扫描。Windows 使用 x64 VST3；macOS VST3 选择与宿主一致的 Apple Silicon 或 Intel 包，只安装其中一套；Universal 2 AU 包含两种架构。支持 Windows 10/11 x64、macOS 11 或更高版本。详细安装路径与排查步骤见随包安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, replace all four and rescan. Use x64 VST3 on Windows. Choose one macOS VST3 package matching the host architecture: Apple Silicon or Intel. Universal 2 AU contains both architectures. Windows 10/11 x64 and macOS 11 or later are supported; see the included guides for paths and troubleshooting.

## 手册与兼容性 / Manuals and compatibility

沿用已确认的 1.7.7 版中英文手册，各 48 页，保留原文件和版本标识。其他操作继续沿用原说明。采样率变化仍清空 EQ Match。切换 Linear Phase 会改变延迟，宿主更新补偿时可能短暂断音。多轨参与端 A/B/C 仍需放在轨道处理链最后；原始轨发送给其他轨时，使用推子后的 A Send 和推子前发送。QQ Host 跨进程 Multi Track 适配仍待处理。macOS 成品为 ad-hoc 签名，未做 Apple Developer ID 公证。

The approved 48-page 1.7.7 Chinese and English manuals are included unchanged with their original labels. Other instructions remain applicable. Sample-rate changes still clear EQ Match. Changing Linear Phase changes latency and may briefly interrupt audio while the host updates compensation. Keep participating A/B/C endpoints last in their tracks; when the original feeds other tracks, use post-fader A Send with pre-fader sends. QQ Host cross-process Multi Track remains pending. macOS builds are ad-hoc signed without Apple Developer ID notarization.

## 下载文件 / Assets

四个平台 ZIP、两份安装说明、两份手册，共八个文件。源码保持私有。本公开仓库的自动 Source code ZIP 只包含公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ-ChainScope-1.7.13-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.13-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.13-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.13-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.13-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.13-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-1.7.13-macOS-Universal-2-AU.zip)
- [QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.13/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
