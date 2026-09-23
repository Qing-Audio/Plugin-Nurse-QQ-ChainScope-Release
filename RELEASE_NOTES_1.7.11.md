# QQ ChainScope 1.7.11

发布日期 / Release date: 2026-09-23

1.7.11 已指定为 Stable。这次集中修复 EQ Match 在重新连接、切换 Group 或 Standalone 时丢失的问题，没有新增操作按钮。

1.7.11 is designated Stable. This update fixes loss of learned EQ Match on reconnection and Group/Standalone changes. No new controls are added.

## 修复与行为变化 / Fixes and behavior changes

### 1.7.11 — Stable

- 中文：B Return 在 Standalone、同轨 Group、跨轨 Group 之间切换或重新连接时保留 Wet/Main Out 的 EQ Match；C Mixboard 进入或离开 Standalone、C/D 切换 Group 时同样保留。保存并重新打开时不再因参考 Group 已改变而丢失匹配。调整 EQ 精度保留结果及开关状态。主动 Reset、整组同步重置和采样率变化仍清空。其他声音处理和界面保持原样。

- English: B Return retains Wet/Main Out EQ Match across Standalone, same-track and cross-track Group changes and reconnections. C retains EQ when entering/leaving Standalone; C/D retain it when changing Groups. Reloading a saved state no longer drops EQ because the reference Group changed. Changing EQ quality preserves the learned result and Match state. Explicit Reset, whole-set synchronise reset and sample-rate changes still clear EQ. Other audio behavior and the UI are unchanged.

### 1.7.10 — previous Candidate, superseded by 1.7.11 / 已由 1.7.11 替代的候选版

- 中文：修复 B Return 从跨轨模式切换到 Standalone 时丢失已计算的 Wet/Main Out EQ Match，并保留保存恢复后的效果。重新连接其他 Group 时仍会清空的问题由 1.7.11 补齐。

- English: Fixed loss of learned Wet/Main Out EQ when B Return detached from cross-track mode into Standalone, including saved-state restoration. The remaining loss on reconnection to another Group is addressed in 1.7.11.



## 安装与升级 / Installation and upgrading

每个平台 ZIP 都包含 A Send、B Return、C Mixboard、D Mixboard。先保存工程并关闭宿主，四件套一起覆盖，再重新扫描。Windows 使用 x64 VST3；macOS VST3 选择与宿主一致的 Apple Silicon 或 Intel 包，只安装其中一套；Universal 2 AU 包含两种架构。支持 Windows 10/11 x64、macOS 11 或更高版本。详细安装路径与排查步骤见随包安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, replace all four and rescan. Use x64 VST3 on Windows. Choose one macOS VST3 package matching the host architecture: Apple Silicon or Intel. Universal 2 AU contains both architectures. Windows 10/11 x64 and macOS 11 or later are supported; see the included guides for paths and troubleshooting.

## 手册与兼容性 / Manuals and compatibility

沿用已确认的 1.7.7 版中英文手册，各 48 页，保留原文件和版本标识。本次 EQ Match 保留/清空规则见上方；其他操作继续沿用原说明。采样率变化仍清空 EQ Match。切换 Linear Phase 会改变延迟，宿主更新补偿时可能短暂断音。多轨参与端 A/B/C 仍需放在轨道处理链最后；原始轨发送给其他轨时，使用推子后的 A Send 和推子前发送。QQ Host 跨进程 Multi Track 适配仍待处理。macOS 成品为 ad-hoc 签名，未做 Apple Developer ID 公证。

The approved 48-page 1.7.7 Chinese and English manuals are included unchanged with their original labels. Updated EQ persistence/reset behavior is described above; other instructions remain applicable. Sample-rate changes still clear EQ Match. Changing Linear Phase changes latency and may briefly interrupt audio while the host updates compensation. Keep participating A/B/C endpoints last in their tracks; when the original feeds other tracks, use post-fader A Send with pre-fader sends. QQ Host cross-process Multi Track remains pending. macOS builds are ad-hoc signed without Apple Developer ID notarization.

## 下载文件 / Assets

四个平台 ZIP、两份安装说明、两份手册，共八个文件。源码保持私有。本公开仓库的自动 Source code ZIP 只包含公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ-ChainScope-1.7.11-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.11-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.11-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.11-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.11-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.11-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-1.7.11-macOS-Universal-2-AU.zip)
- [QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.11/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
