# QQ ChainScope 1.7.24

发布日期 / Release date: 2026-10-11 · Stable

## 本次变化 / Changes

### 1.7.23
- 中文：允许播放中点击响度 Match、L/R Cal、PHASE CALC、EQ CAL 和 Latency Rescue。响度 Match、L/R Cal 与 EQ CAL 每次都使用从本次播放起点到点击时的累计数据，重复点击保留记录；停止后重新播放开始新一轮。ECO 下需在播放前打开相应分析界面。
- English: Allows loudness Match, L/R Cal, PHASE CALC, EQ CAL and Latency Rescue during playback. Loudness Match, L/R Cal and EQ CAL use accumulated data from the current playback pass's start to each click, retaining the capture across repeated calculations. Stop and restart for a new pass. In ECO, open the required analysis view before playback.

### 1.7.24 — Stable
- 中文：B Return 在底部 Monitor 行右侧加入 SIP，控制 L/R/S 监听是否保留空间位置。新建实例默认关闭，旧工程保留原来的原位监听方式；Stereo 与 M 不变。中英文手册更新为 50 页，独立介绍 Graph、频谱、波形及放大操作，并补充播放中计算、SIP、发送和名称来源说明。
- English: Adds SIP at the right of B Return's Monitor row to control spatial placement in L/R/S monitoring. New instances default to SIP off; older projects retain their previous in-place monitoring. Stereo and M are unchanged. Both manuals now have 50 pages, with a dedicated Graph chapter and updated live-calculation, SIP, sending and source-name guidance.

## 安装与升级 / Installation and upgrade

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。保存工程并关闭宿主，四件套一起更新，再重新扫描。Windows 使用 x64 VST3；Mac 根据宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套。Universal 2 AU 同时包含两种架构。详细步骤见安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, update all four and rescan. Use x64 VST3 on Windows. Choose one Mac VST3 package matching the host: Apple Silicon or Intel. Universal 2 AU contains both architectures. See the installation guides for the full steps.

随包提供新版 50 页中英文手册。Classic、SSL、Light、Dark 四种界面继续保留。播放中首次启用会增加延迟的 Phase 或线性相位 EQ 时，DAW 更新延迟补偿可能带来短暂停顿。SIP 默认行为的变化只用于新建 B Return，旧工程沿用原来的原位监听方式。

The updated Chinese and English manuals each have 50 pages. Classic, SSL, Light and Dark styles remain available. Enabling Phase or linear-phase EQ for the first time during playback may briefly interrupt audio while the DAW adjusts delay compensation. The new SIP default applies to new B Return instances; older sessions retain their previous in-place monitoring.

## 平台、验证与已知限制 / Platforms, checks and known limits

Windows 10/11 x64；macOS 11.0 或更新系统。macOS 成品采用 ad-hoc 签名，未经 Apple Developer ID 公证。各平台的版本、架构与文件完整性已核对，Mac 签名与实际 AU 接口测试通过；Windows 复用已通过的实际 VST3 测试。本次没有新增 DAW 听感实测，验证不覆盖所有宿主与系统组合。QQ Host 跨进程多轨兼容仍待处理。

Windows 10/11 x64; macOS 11.0 or later. Mac builds are ad-hoc signed and are not Apple Developer ID notarized. Versions, architectures and file integrity have been checked; Mac signature checks and actual AU interface tests passed. The existing Windows VST3 test results are reused. No new DAW listening test is claimed, and these checks do not cover every host and OS combination. QQ Host cross-process Multi Track compatibility remains pending.

## 下载 / Downloads

八个文件：四个平台 ZIP、两份安装说明、两份手册。源码保持私有。GitHub 自动生成的 Source code ZIP 只包含这个公开仓库中的文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source stays private. GitHub's automatic Source code ZIP contains only the documentation in this public repository.

- [QQ ChainScope 1.7.24 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ.ChainScope.1.7.24.txt)
- [QQ-ChainScope-1.7.24-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-1.7.24-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.24-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-1.7.24-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.24-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-1.7.24-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.24-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-1.7.24-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.24-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-1.7.24-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.7.24.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ.ChainScope.v1.7.24.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.24.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.24/QQ-ChainScope-User-Manual-English-v1.7.24.pdf)
