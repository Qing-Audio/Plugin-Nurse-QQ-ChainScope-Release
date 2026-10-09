# QQ ChainScope 1.7.22

发布日期 / Release date: 2026-10-09

## 本次变化 / Changes

### 1.7.17
- 中文：修复 macOS 多个插件实例之间的 Group 与多轨控制信息共享；AU 缺少轨道标识时允许手动选择全部 Group。
- English: Fixes shared Group and remote-control discovery across macOS instances. AU permits manual selection of all Groups when track identity is unavailable.

### 1.7.18
- 中文：补齐 AU 的工程采样位置，让跨轨 Before 测量、波形和 EQ Match 取得参考信号。
- English: Supplies the AU project-sample clock for cross-track Before analysis, waveform and EQ Match reference capture.

### 1.7.19
- 中文：修复 AU 停止播放后 Before 电平的更新状态，保留峰值保持与分析历史。
- English: Fixes AU Before meter freshness after playback stops while retaining peak holds and analysis history.

### 1.7.20
- 中文：修复重新打开工程后已开启的 Multi Track 没有重新注册的问题，无需手动关闭再打开按钮。
- English: Restores saved Multi Track endpoint registration when reopening a project, without requiring a manual toggle.

### 1.7.21
- 中文：修复 AU 起播时短暂漏出 Send 原声的问题，并及时同步停止播放时修改的 QQ Bypass 状态；起播淡入的进一步修复见 1.7.22。
- English: Addresses the brief AU Send burst at playback start and promptly publishes stopped QQ Bypass changes. Further startup fade handling follows in 1.7.22.

### 1.7.22 — Stable
- 中文：修复 AU 与 Windows VST3 起播时的短暂淡入。宿主暂停处理、重新播放时立即使用当前音量比例；播放中的 Bypass crossfade 保留，不增加音频延迟。
- English: Fixes playback-start fades in AU and Windows VST3. Current remote gains apply immediately after processing suspension or playback restart. Existing live Bypass crossfades remain intact, with no added audio latency.

## 安装与升级 / Installation and upgrade

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。保存工程并关闭宿主后，四件套一起更新，再重新扫描。Windows 选 x64 VST3；Mac 根据宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套。Universal 2 AU 包含两种架构。详细步骤见安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, update all four and rescan. Use x64 VST3 on Windows. Choose one Mac VST3 package matching the host architecture: Apple Silicon or Intel. Universal 2 AU contains both architectures. See the installation guides for detailed steps.

沿用原版 1.7.7 中英文手册和 Classic、SSL、Light、Dark 四种界面。macOS 成品为 ad-hoc 签名，未进行 Apple Developer ID 公证。各平台完成版本、架构和签名检查；Windows 实际 VST3 与 Mac 实际 AU 接口的起播回归测试通过。此次结果不代表覆盖所有 DAW 与系统组合。QQ Host 跨进程多轨兼容仍待处理。

The original 1.7.7 Chinese and English manuals and Classic, SSL, Light and Dark styles are retained. macOS builds are ad-hoc signed without Apple Developer ID notarization. Platform versions, architectures and signatures were checked. Startup regression tests passed against actual Windows VST3 and Mac AU interfaces. These results do not cover every DAW and operating system combination. QQ Host cross-process Multi Track compatibility remains pending.

## 下载 / Downloads

八个文件：四个平台 ZIP、两份安装说明、两份手册。源码保持私有。本公开仓库自动生成的 Source code ZIP 只包含公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ ChainScope 1.7.22 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ.ChainScope.1.7.22.txt)
- [QQ-ChainScope-1.7.22-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-1.7.22-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.22-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-1.7.22-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.22-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-1.7.22-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.22-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-1.7.22-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.22-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-1.7.22-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ.ChainScope.v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.22/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
