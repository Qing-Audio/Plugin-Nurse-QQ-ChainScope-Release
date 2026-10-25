# QQ ChainScope 1.8.18 Stable

## 本次更新 / Changes since 1.8.17

### 1.8.18 — MIDI 全范围音量映射 / Full-range MIDI level mapping

- 中文：C/D Mixboard 新增 SOURCE n LEVEL 完整范围参数，音量块可通过 Cubase MIDI Remote／快速控制从静音控制到 +12 dB（约 398.1%）。修正绑定到 BOOST 后最低位置只能到绑定时音量的问题。若已有映射选择了 SOURCE n BOOST，请重新学习音量块或手动选择 SOURCE n LEVEL。
- English: C/D Mixboard now expose full-range SOURCE n LEVEL parameters, allowing Cubase MIDI Remote / Quick Controls to control gain blocks from silence to +12 dB (about 398.1%). This fixes mappings to BOOST being unable to go below the gain present when learned. Relearn the gain block or select SOURCE n LEVEL if an existing mapping targets SOURCE n BOOST.
- 中文：B/C/D 单推子和 L/R 推子的学习通知、点击目标已修正，使用原有静音至 +30 dB 的绝对范围；旧参数编号、范围与工程状态保持兼容。原有 Link、音频处理和图表功能保持不变。
- English: Learning notifications and hit targets are corrected for B/C/D single and L/R faders, retaining the absolute range from silence to +30 dB. Existing parameter identifiers, ranges and saved states remain compatible. Link, audio processing and graph behavior are unchanged.
- 中文：中英文手册沿用 v1.8.17 原文件，各 62 页；本次不修改内容或版本标识，两份 PDF 随包与 Release 提供。
- English: Both 62-page v1.8.17 manuals are included unchanged in the package and Release, with their original content and version labels.

## 下载 / Downloads

- [QQ ChainScope 1.8.18 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.1.8.18.txt)
- [QQ-ChainScope-1.8.18-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-Installation-Guide-English.txt)
- [QQ-ChainScope-1.8.18-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.8.18-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.8.18-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.8.18-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.8.17.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.v1.8.17.pdf)
- [QQ ChainScope User Manual English v1.8.17.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.User.Manual.English.v1.8.17.pdf)

## 安装与兼容性 / Installation and compatibility

- 中文：Windows 使用 x64 VST3。Mac 原生 Apple Silicon 宿主选 arm64 VST3；Intel／Rosetta 宿主选 x86_64 VST3，二者只装一套。AU 使用 Universal 2，包含 arm64 与 x86_64。每包包含 A/B/C/D 四件套，请一起升级；替换前退出所有音频宿主并备份工程。
- English: Use x64 VST3 on Windows. On Mac, choose arm64 VST3 for native Apple Silicon hosts or x86_64 VST3 for Intel/Rosetta hosts; install only one VST3 architecture. Universal 2 AU contains both architectures. Each package includes A/B/C/D; upgrade all four together. Close audio hosts and save a session copy before replacing plug-ins.
- 中文：Mac 成品使用 ad-hoc 签名，未经过 Apple Developer ID 公证。Windows 成品复用已验证构建，Mac 成品经对应架构构建、签名检查及原生／Rosetta 插件接口测试。自动化测试不代表所有 DAW 与实体 MIDI 控制器组合均已验收。
- English: Mac builds use ad-hoc signatures without Apple Developer ID notarization. The verified Windows build is reused. Mac builds are checked for architecture, signatures and native/Rosetta plug-in interface behavior. Automated testing does not certify every DAW and physical MIDI controller combination.
- 中文：MASKING 仍属于试验性辅助分析，SENS 默认 20、REF SPL 默认 75；阴影需结合听感判断。源码保持私有，本 Release 仅提供成品与文档。
- English: MASKING remains experimental visual assistance with defaults of SENS 20 and REF SPL 75; interpret shading with listening judgment. Source remains private; this Release distributes compiled products and documentation only.
