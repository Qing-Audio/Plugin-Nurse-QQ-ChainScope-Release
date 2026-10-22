# QQ ChainScope 1.8.1 Stable

发布日期 / Release date: 2026-10-22

## 本次变化 / Changes since 1.8.0

### 1.8.1
- 中文：配合 QQ Host 1.3.6 的多段处理，使用音频块标记和采样位置配对 Original、Return 与混合音频，保留插件延迟对齐。完整且位于同一 QQ Host 的 A/B/C 组可以参与分段；旧版、不完整、跨 Host 及 D 组继续保留分段保护。现有界面、DSP、测量、预置和说明书保持不变。A/B/C/D 四个模块必须一起升级。
- English: Adds audio-block and sample-position matching for Original, Returns and mixed audio under QQ Host 1.3.6 multistage processing, retaining declared-latency alignment. Complete A/B/C groups contained within one QQ Host can use multiple stages. Older, incomplete, cross-Host and D groups keep pipeline protection. Existing UI, DSP, metering, presets and manuals are retained. Upgrade all four A/B/C/D modules together.


## 安装与升级 / Installation and upgrade

保存工程并完全退出宿主，再一起更新 A Send、B Return、C Mixboard、D Mixboard 四个模块，并重新扫描插件。Windows 使用 x64 VST3。Mac 的 VST3 选择与宿主架构一致的一套；Universal 2 AU 同时包含 Apple Silicon 与 Intel。不要混用本版与旧版模块，也不要在系统目录与用户目录保留重复副本。

Save the session and quit the host completely before updating all four A/B/C/D modules and rescanning. Use x64 VST3 on Windows. On Mac, choose one VST3 package matching the host architecture; Universal 2 AU includes Apple Silicon and Intel. Keep every module on the same version and avoid duplicate system/user installations.

## 使用与兼容性 / Usage and compatibility

QQ Host 多段处理需要配套支持本次接口的版本；本次 Windows 配套版本为 QQ Host 1.3.6。普通 DAW 和既有处理路径保留。未对 Mac 版 QQ Host 的配套组合作实际宿主验证。

QQ Host multistage processing requires a matching host version supporting the new interface; the paired Windows version is QQ Host 1.3.6. Native DAW and existing processing paths are retained. This release does not claim a real-host test of the paired macOS QQ Host combination.

Windows 10/11 x64；macOS 11.0 或更新系统。Mac 为 ad-hoc 签名，未经过 Apple Developer ID 公证。安装位置、重扫及必要的解除隔离步骤见安装说明。

Windows 10/11 x64; macOS 11.0 or later. Mac builds use ad-hoc signatures and are not Apple Developer ID notarized. See the installation guides for paths, rescanning and quarantine steps.

## 验证范围 / Validation scope

复用已完成的 Windows 构建、回归测试和安装验证。Windows 实际 VST3 机架按 1/2/3/4 段处理时输出逐样本一致，包括循环和停止后恢复。Mac 发布检查包含版本、架构、签名、原生音频块配对及处理器回归、实际 AU 接口与文件完整性；不把这些自动检查写成新的 DAW 听感验证。

Existing Windows builds, regressions and installation checks are reused. Actual Windows VST3 rack output is sample-identical at 1/2/3/4 stages, including loops and stop/resume. Mac release checks cover version, architecture, signatures, native block matching and processor regressions, actual AU interfaces and file integrity. These automated checks do not imply a new DAW listening test.

## 说明书 / Manuals

本 Release 附带原有中英文用户手册，各 54 页。手册内容和文件名保留真实的 v1.8.0 标识，未重新编写或改名冒充 1.8.1。

Both existing 54-page Chinese and English user manuals are attached. Their content and filenames retain the genuine v1.8.0 version; they have not been rewritten or relabeled as 1.8.1.

## 下载 / Downloads

八个附件：四个平台 ZIP、两份安装说明和两本手册。产品源码保持私有；GitHub 自动生成的 Source code 压缩包只包含公开仓库文档。

Eight assets: four platform ZIPs, two installation guides and both manuals. Product source remains private; GitHub's automatic Source code archives contain public repository documentation only.

- [QQ ChainScope 1.8.1 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ.ChainScope.1.8.1.txt)
- [QQ-ChainScope-1.8.1-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-1.8.1-Installation-Guide-English.txt)
- [QQ-ChainScope-1.8.1-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-1.8.1-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.8.1-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-1.8.1-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.8.1-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-1.8.1-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.8.1-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-1.8.1-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.8.0.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ.ChainScope.v1.8.0.pdf)
- [QQ-ChainScope-User-Manual-English-v1.8.0.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.1/QQ-ChainScope-User-Manual-English-v1.8.0.pdf)
