# QQ ChainScope 1.7.25

发布日期 / Release date: 2026-10-12 · Stable

## 本次变化 / Changes

### 1.7.25 — Stable
- 中文：设置中的 FULL / ECO 一起调整同一宿主进程里已经插入的 B Return、C Mixboard 和 D Mixboard，关闭窗口的插件也会跟随；后来新插入的插件仍默认 FULL，保存的工程保留各插件自己的模式。B/C/D 齿轮左侧新增单个插件的 ECO/FULL 按钮，并跟随全局调整。按钮、旋钮、菜单和数值框增加中文悬停说明。中英文手册各 51 页，新增配图说明。
- English: Settings FULL / ECO now updates existing B Return, C Mixboard and D Mixboard instances in the same host process, including closed editors. New inserts still start in FULL; saved projects retain each instance's mode. A local ECO/FULL button sits immediately left of the gear in B/C/D and follows global changes. Buttons, knobs, menus and value fields gain Chinese hover help. Both manuals have 51 pages, with a new illustrated guide.

## 安装与升级 / Installation and upgrade

先保存工程并关闭宿主，再完整更新 A Send、B Return、C Mixboard、D Mixboard 四件套，必要时重新扫描。Windows 使用 x64 VST3。Mac 按宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套；Universal 2 AU 同时包含两种架构。详细步骤见安装说明。

Save the session and quit the host before updating all four A/B/C/D components; rescan if necessary. Use x64 VST3 on Windows. On Mac, install one VST3 architecture matching your host: Apple Silicon or Intel. Universal 2 AU includes both architectures. See the installation guides for detailed steps.

## 行为与兼容性 / Behavior and compatibility

本次优化调整分析模式控制和悬停说明，声音处理及旧工程保存格式保持不变。保存过的工程沿用每个插件的模式；后来新插入的插件仍为 FULL。全局切换作用于同一宿主进程里的现有插件，宿主采用不同进程隔离插件时需要分别调整。悬停说明目前为中文。中英文手册各 51 页，原有操作、提示和 Graph 章节保留。

This update changes analysis-mode controls and hover help; audio processing and the saved-project format are unchanged. Saved instances retain their mode; newly inserted instances start in FULL. Global changes reach existing instances in the same host process. Adjust separately when a host isolates plug-ins in different processes. Hover help is currently Chinese. Both 51-page manuals preserve existing operations, tips and the Graph chapter.

## 平台、验证与已知限制 / Platforms, checks and known limits

Windows 10/11 x64；macOS 11.0 或更新系统。Mac 文件采用 ad-hoc 签名，未经 Apple Developer ID 公证。发布前核对版本、架构、签名与文件完整性，并检查原生测试结果。本次没有新增 DAW 听感实测；验证不覆盖所有宿主和系统组合。QQ Host 跨进程多轨兼容仍待处理。

Windows 10/11 x64; macOS 11.0 or later. Mac files are ad-hoc signed, without Apple Developer ID notarization. Release checks cover versions, architectures, signatures, file integrity and native test results. No new DAW listening test is claimed; verification does not cover every host and OS combination. QQ Host cross-process Multi Track compatibility remains pending.

## 下载 / Downloads

八个附件：四个平台 ZIP、两份安装说明、两份手册。产品源码保持私有。GitHub 自动生成的 Source code ZIP 仅含公开仓库的文档。

Eight assets: four platform ZIPs, two installation guides and two manuals. Product source stays private. GitHub's automatic Source code archives contain public-repository documentation only.

- [QQ ChainScope 1.7.25 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ.ChainScope.1.7.25.txt)
- [QQ-ChainScope-1.7.25-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-1.7.25-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.25-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-1.7.25-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.25-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-1.7.25-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.25-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-1.7.25-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.25-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-1.7.25-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.7.25.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ.ChainScope.v1.7.25.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.25.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.7.25/QQ-ChainScope-User-Manual-English-v1.7.25.pdf)
