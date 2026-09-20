# QQ ChainScope 1.7.9

发布日期 / Release date: 2026-09-21

1.7.9 已由用户指定为 Stable。本次更新修复 EQ Match 对齐与 Side/Mid 波形显示，操作方式保持不变，已有 EQ 设置继续保留。

1.7.9 is user-designated Stable. This update fixes EQ Match alignment and Side/Mid waveform display while retaining the existing workflow and EQ settings.

## 本次修复 / Fixes since 1.7.7

### 1.7.9 — EQ Match alignment / EQ Match 对齐

- 中文：修复最小相位下 Before/Dry 与 Match 旁通路径多出约 80 ms 延迟的问题，涉及 B Return、C Mixboard 和 D 控制的发送端。保留线性相位补偿与现有 EQ 设置。
- English: Fixes approximately 80 ms of unintended delay in minimum-phase Before/Dry and Match bypass paths, affecting B Return, C Mixboard and D-controlled endpoints. Linear-phase compensation and existing EQ settings are retained.

### 1.7.8 — Side/Mid waveforms / Side、Mid 波形

- 中文：修复 Side 已无声却仍显示波形的问题，并修正反相声道的 Mid 波形；覆盖 B/C/D、停止后的监听切换及 WaveScope。
- English: Fixes false Side waveforms for identical channels and false Mid waveforms for opposite-polarity channels across B/C/D, including stopped monitoring changes and WaveScope.



## 安装与升级 / Installation and upgrading

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。先关闭宿主，四件套一起覆盖并重新扫描。Windows 使用 x64 VST3；macOS VST3 选择与宿主一致的 Apple Silicon 或 Intel 包，两套只安装一套。AU 包同时支持两种架构。Windows 10/11 x64，macOS 11 或更高版本；详细路径、重新扫描和安全设置见安装说明。

Each platform ZIP includes A Send, B Return, C Mixboard, and D Mixboard. Quit the host, replace the complete set, and rescan. Use x64 VST3 on Windows. On macOS, choose one VST3 package matching the host's Apple Silicon or Intel architecture. AU supports both architectures. Windows 10/11 x64 and macOS 11 or later; the installation guides include paths, rescan steps, and security settings.

## 说明书与兼容性 / Manuals and compatibility

本包沿用已确认的 1.7.7 版中英文手册，各 48 页；操作步骤同样适用于 1.7.9。本次修复见下方版本记录。

The approved 48-page 1.7.7 manuals are included unchanged. Their operating instructions also apply to 1.7.9; the fixes are listed below.


本次没有新增操作。切换 Linear Phase 仍会改变延迟，宿主更新补偿时可能短暂断音。macOS 为 ad-hoc 签名，未做 Apple Developer ID 公证。QQ Host 跨进程 Multi Track 适配仍待处理。多轨参与端 A/B/C 需放在轨道处理链最后；原始轨给其他轨发送时，继续使用推子后的 A Send 和推子前发送。升级前保存重要工程副本，避免混用新旧插件。

No new controls are added. Changing Linear Phase still changes latency and may briefly interrupt audio while the host updates compensation. macOS builds are ad-hoc signed, without Apple Developer ID notarization. QQ Host cross-process Multi Track remains pending. Keep participating A/B/C endpoints last in their tracks; when the original feeds other tracks, keep A Send post-fader and sends pre-fader. Save important sessions before upgrading and avoid mixing component versions.

## 下载文件 / Assets

四个平台 ZIP、两份安装说明、两份手册，共八个文件。源码保持私有。本公开仓库的自动 Source code ZIP 仅包含公开文档。

Eight files: four platform ZIPs, two installation guides, and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains this public documentation repository only.

- [QQ-ChainScope-1.7.9-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.9-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.9-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.9-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.9-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.9-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-1.7.9-macOS-Universal-2-AU.zip)
- [QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.9/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
