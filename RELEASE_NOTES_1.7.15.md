# QQ ChainScope 1.7.15

发布日期 / Release date: 2026-10-05

## 本次变化 / Changes

### 1.7.15 — Stable — 2026-10-05

- 中文：修复拖动旋钮、推子、百分比、混合比例和频率数值时按下或松开 Shift 导致的参数回跳。切换 Shift 时从当前值继续调整，普通拖动和精细调整的速度保持原样。A/B/C/D 四件套请一起更新。
- English: Fixes parameter jumps when pressing or releasing Shift during knob, fader, percentage, mix-weight and frequency drags. Adjustment continues from the current value when Shift changes; normal and fine sensitivities are retained. Update all four A/B/C/D plug-ins together.

音频处理、路由、EQ Match、延迟和已保存工程的参数含义保持原样。

Audio processing, routing, EQ Match, latency and saved parameter meanings are unchanged.

## 安装与升级 / Installation and upgrade

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。保存工程并关闭宿主后，四件套一起更新，再重新扫描。Windows 选 x64 VST3；Mac 根据宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套。Universal 2 AU 包含两种架构。详细步骤见安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, update all four and rescan. Use x64 VST3 on Windows. Choose one Mac VST3 package matching the host architecture: Apple Silicon or Intel. Universal 2 AU contains both architectures. See the installation guides for detailed steps.

沿用原版 1.7.7 中英文手册和 Classic、SSL、Light、Dark 四种界面。macOS 成品为 ad-hoc 签名，未进行 Apple Developer ID 公证。各平台完成版本和架构检查，AU 通过自动校验；未增加 DAW 听感实测。QQ Host 跨进程多轨兼容仍待处理。

The original 1.7.7 Chinese and English manuals and Classic, SSL, Light and Dark styles are retained. macOS builds are ad-hoc signed without Apple Developer ID notarization. Platform versions and architectures were checked, and AU passed automated validation; no new DAW listening test is claimed. QQ Host cross-process Multi Track compatibility remains pending.

## 下载 / Downloads

八个文件：四个平台 ZIP、两份安装说明、两份手册。源码保持私有。本公开仓库自动生成的 Source code ZIP 只包含公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ-ChainScope-1.7.15-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.15-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.15-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.15-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.15-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.15-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-1.7.15-macOS-Universal-2-AU.zip)
- [QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.15/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
