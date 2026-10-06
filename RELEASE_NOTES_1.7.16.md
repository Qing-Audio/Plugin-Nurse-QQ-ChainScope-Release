# QQ ChainScope 1.7.16

发布日期 / Release date: 2026-10-06

## 本次变化 / Changes

### 1.7.16 — Stable — 2026-10-06

- 中文：EQ Match 的 Amount 扩展为 -200% 到 +200%，负值反向应用匹配曲线，正负 200% 将修正幅度加倍。B Return 的 Wet/Main Out、C/D Mixboard 和多轨端口一致支持；默认值与 Alt 复位仍为 100%，保存、恢复和撤销保留完整范围。其他功能不变，A/B/C/D 四件套请一起更新。
- English: Extends EQ Match Amount to -200% through +200%. Negative values reverse the learned correction; +/-200% doubles its magnitude. B Return Wet/Main Out, C/D Mixboard and remote endpoints support the full range, including save/restore and undo. The default and Alt reset remain 100%; other behavior is unchanged. Update all four A/B/C/D plug-ins together.

## 安装与升级 / Installation and upgrade

每个平台 ZIP 包含 A Send、B Return、C Mixboard、D Mixboard。保存工程并关闭宿主后，四件套一起更新，再重新扫描。Windows 选 x64 VST3；Mac 根据宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套。Universal 2 AU 包含两种架构。详细步骤见安装说明。

Every platform ZIP includes A Send, B Return, C Mixboard and D Mixboard. Save the session, quit the host, update all four and rescan. Use x64 VST3 on Windows. Choose one Mac VST3 package matching the host architecture: Apple Silicon or Intel. Universal 2 AU contains both architectures. See the installation guides for detailed steps.

沿用原版 1.7.7 中英文手册和 Classic、SSL、Light、Dark 四种界面。macOS 成品为 ad-hoc 签名，未进行 Apple Developer ID 公证。各平台完成版本和架构检查，Universal AU 在 Intel 自建机通过 auval 自动校验；未增加 DAW 听感实测。QQ Host 跨进程多轨兼容仍待处理。

The original 1.7.7 Chinese and English manuals and Classic, SSL, Light and Dark styles are retained. macOS builds are ad-hoc signed without Apple Developer ID notarization. Platform versions and architectures were checked, and Universal AU passed auval validation on the Intel build machine; no new DAW listening test is claimed. QQ Host cross-process Multi Track compatibility remains pending.

## 下载 / Downloads

八个文件：四个平台 ZIP、两份安装说明、两份手册。源码保持私有。本公开仓库自动生成的 Source code ZIP 只包含公开文档。

Eight files: four platform ZIPs, two installation guides and two manuals. Product source remains private. GitHub's automatic Source code ZIP contains only this public documentation repository.

- [QQ-ChainScope-1.7.16-Installation-Guide-Chinese.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-Installation-Guide-Chinese.txt)
- [QQ-ChainScope-1.7.16-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-Installation-Guide-English.txt)
- [QQ-ChainScope-1.7.16-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.7.16-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.7.16-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.7.16-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-1.7.16-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ.ChainScope.v1.7.7.pdf)
- [QQ-ChainScope-User-Manual-English-v1.7.7.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/untagged-ffb72bb9ea6cb5b5385d/QQ-ChainScope-User-Manual-English-v1.7.7.pdf)
