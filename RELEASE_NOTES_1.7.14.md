# QQ ChainScope 1.7.14

发布日期 / Release date: 2026-09-30

1.7.14 Stable 优化 C/D 在 ECO 模式、关闭界面后的处理开销。原有声音功能保持不变；A/B/C/D 请一起升级。

1.7.14 Stable reduces C/D processing in ECO mode with their windows closed. Existing audio behavior is preserved; update A/B/C/D together.

## 本次变化 / Changes

### 1.7.14 — Stable — 2026-09-30

- 中文：优化 C Mixboard、D Mixboard 在 ECO 模式、关闭界面后的处理开销。C 的 MIX 不再要求 B Return 持续计算不需要的频谱；D 减少重复控制更新和空闲处理。音频路由、EQ Match、延迟和切换行为保持原样。A/B/C/D 四件套请一起更新。
- English: Reduces processing in C Mixboard and D Mixboard in ECO mode with their windows closed. C MIX no longer keeps B Return computing an unneeded shared spectrum; D avoids repeated control updates and idle work. Audio routing, EQ Match, latency and switching behavior remain unchanged. Update all four A/B/C/D plug-ins together.

本地 48 kHz、256 帧测试中，“六个 A Send + D Mixboard”处理时间比 1.7.13 减少约 24.6%。这是本地处理回调测试，不等同于所有 DAW 的 ASIO Guard 数值。

In local 48 kHz, 256-frame callback tests, six A Sends plus D Mixboard used about 24.6% less processing time than 1.7.13. This is a local callback result, not a measured ASIO Guard reduction for every DAW.

## 安装 / Installation

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。保存工程并退出宿主后，四件套一起覆盖，再重新扫描。Windows 选 x64 VST3；macOS VST3 按宿主架构选 Apple Silicon 或 Intel 包，只安装一套；Universal 2 AU 包含两种架构。详细步骤见安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, replace all four, then rescan. Use x64 VST3 on Windows. Choose one macOS VST3 package matching the host architecture, Apple Silicon or Intel. Universal 2 AU contains both architectures. See the installation guides for details.

沿用已确认的 1.7.7 中英文手册及其原版本标识，内容未修改。Classic、SSL、Light、Dark 四种界面都可选。macOS 成品为 ad-hoc 签名，未进行 Apple Developer ID 公证。

The approved 1.7.7 Chinese and English manuals are included unchanged with their original labels. Classic, SSL, Light and Dark remain available. macOS builds are ad-hoc signed without Apple Developer ID notarization.

## 下载 / Downloads

八个文件：四个平台 ZIP、两份安装说明和两份手册。源码保持私有；本公开仓库自动生成的 Source code ZIP 只有公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ-ChainScope-1.7.14-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.14-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.14-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.14-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.14-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.14-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-1.7.14-macOS-Universal-2-AU.zip)
- [QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-User-Manual-Chinese-v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.14/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
