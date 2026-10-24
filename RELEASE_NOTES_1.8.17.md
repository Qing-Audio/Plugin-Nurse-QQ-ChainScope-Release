# QQ ChainScope 1.8.17 Stable

发布日期 / Release date: 2026-10-24

新增 C/D OVERLAY、独立眼睛与静音、模式对应的 Link 和试验性 MASKING（SENS 20 / REF SPL 75）。本版还修复 ECO 切换图表及播放中跳转后的频谱更新问题。完整变化按真实版本列在下面。

Adds C/D OVERLAY, independent eyes and mute, mode-aware Link and experimental MASKING (SENS 20 / REF SPL 75). Includes ECO graph-switching and playback-seek spectrum fixes. Every intervening version is listed below.

## 安装 / Installation

保存工程，完全退出宿主，再一起升级 A Send、B Return、C Mixboard、D Mixboard。Windows 10/11 x64 使用 VST3；macOS 11.0 或更新系统，VST3 选择与宿主架构一致的一套。Universal 2 AU 同时包含 arm64 与 x86_64。Mac 为 ad-hoc 签名，未经过 Apple Developer ID 公证；重扫与必要的解除隔离步骤见安装说明。不要在用户与系统目录同时保留重复副本。

Save the session, quit the host completely and update A/B/C/D together. Windows 10/11 x64 uses VST3. On macOS 11.0 or later, choose one VST3 architecture matching the host. Universal 2 AU contains arm64 and x86_64. Mac builds are ad-hoc signed, without Apple Developer ID notarization. See the guides for rescanning and quarantine handling. Avoid duplicate user/system copies.

## 手册与验证 / Manuals and validation

附中英文手册各 62 页，保留原配色与文字风格，补齐 OVERLAY、眼睛、静音、Link、MASKING、SENS 与 REF SPL。Windows 复用已验证成品；Mac 检查产品版本、架构、签名、实际 AU 加载和相关回归。Intel 成品在 Apple Silicon 上交叉编译，并通过 Rosetta 执行验证；不把自动检查说成实际 DAW 听感测试。

Includes both 62-page manuals in the established style, covering OVERLAY, eyes, mute, Link, MASKING, SENS and REF SPL. Windows artifacts are reused from the verified build. Mac checks cover versions, architectures, signatures, actual AU loading and relevant regressions. Intel binaries are cross-compiled on Apple Silicon and executed under Rosetta for validation. Automated checks do not imply DAW listening tests.

## 版本变化 / Version history

### 1.8.17

- 中文：修复播放中跳转位置后 C/D 的 COMPARE、OVERLAY 频谱保留旧曲线、后续更新停滞的问题。保留既有音频处理、测量算法与累计规则。
- English: Fixes stalled COMPARE/OVERLAY spectrum updates after playback seeks in C/D Mixboard. Audio processing, meter algorithms and accumulation rules are preserved.

### 1.8.16

- 中文：MASKING 的 SENS 默认值调整为 20，Alt 恢复 20；已保存的实例数值不被覆盖。中文手册补充 SENS、REF SPL、多轨选择和阴影示例。
- English: Sets the default MASKING SENS to 20, including Alt reset, without overwriting saved instance values. Adds Chinese manual examples for SENS, REF SPL, source selection and shading.

### 1.8.15

- 中文：ECO 下展开 Graph 时同时维护 COMPARE、OVERLAY、MIX 图表，修复来回切换后频谱消失。收起 Graph 或关窗后仍按 ECO 规则节省分析。此版将 SENS 默认值设为 30，后续 1.8.16 改为 20。
- English: Keeps all three graph modes ready while Graph is open in ECO, fixing missing spectra after mode changes. Collapsing Graph or closing the window retains ECO savings. This version used SENS 30; 1.8.16 supersedes it with 20.

### 1.8.14

- 中文：降低图表快照与历史重建对线程栈的占用，修复在 QQ Host 较小线程栈下可能导致断线的路径，保留图表与音频功能。
- English: Reduces stack use in graph snapshots and history projection, addressing a disconnect path on QQ Host threads with smaller stacks while preserving audio and graph behavior.

### 1.8.13

- 中文：为 C/D 的 OVERLAY 增加独立 SENS 灵敏度参数、保存和精细调整。此版默认 50，后续版本继续调整默认值。
- English: Adds a saved, finely adjustable SENS control to C/D OVERLAY. The initial default was 50; later versions refine that default.

### 1.8.12

- 中文：进一步收紧 MASKING 对微弱尾部和不显著重叠的判断，减少过多阴影提示。
- English: Makes MASKING more selective about weak tails and insignificant overlap to reduce excessive shading.

### 1.8.11

- 中文：MASKING 增加渐亮、渐暗和平滑处理，减少闪烁，并继续降低过度敏感的提示。
- English: Smooths MASKING shading with gradual attack and release, reducing flicker and over-sensitive indications.

### 1.8.10

- 中文：B 的音量、PAN、Dry/Wet 以及 C/D MIX 的音量与静音可重新呈现已记录的图表，停止后也能查看变化；C/D 模式顺序改为 COMPARE、OVERLAY、MIX。
- English: Updates retained graphs for B gain, PAN and Dry/Wet and C/D MIX gain and mute, including while stopped. Orders C/D mode buttons as COMPARE, OVERLAY, MIX.

### 1.8.9

- 中文：MASKING 改为眼睛点亮来源之间的两两分析，移除参考轨和 AUTO/PAIR 的额外选择。C 增加与 D 一致的 OVERLAY、dB 音量与 Link；右键静音采用更深的黑色。
- English: Uses pairwise MASKING across sources with lit eyes, removing the extra reference-track and AUTO/PAIR choices. Adds matching OVERLAY, dB gain and Link behavior to C. Muted source blocks use a deeper black.

### 1.8.8

- 中文：减少 MASKING 对很弱成分的误提示，统一频谱与波形的遮蔽可见条件。
- English: Reduces MASKING indications from very weak components and aligns spectrum and waveform visibility criteria.

### 1.8.7

- 中文：眼睛仅控制图表、数值显示及 Link/Alt 参与范围，不再决定声音是否混合。MIX/OVERLAY 中右键独立静音；COMPARE 右键不静音。解除 D 连接时释放遥控静音。
- English: Separates eye-controlled display and Link/Alt participation from audio mixing. Adds independent right-click mute in MIX/OVERLAY, with no right-click mute in COMPARE. Disconnecting D releases its remote mute.

### 1.8.6

- 中文：加入首版 MASKING 与 REF SPL、频率和时间阴影；进一步放慢音量调整。MIX Link 保持总百分比，OVERLAY Link 同步增减 dB。无 Before 时仍显示 After，禁用新 EQ Match 计算但保留已有结果。B/D 解除连接时释放隐藏遥控处理，重新连接后按当前控制器状态恢复。
- English: Introduces MASKING, REF SPL and frequency/time shading, with slower gain adjustment. MIX Link preserves the total percentage; OVERLAY Link applies equal dB changes. After remains available without Before; new EQ Match calculation is disabled but existing results remain. Disconnecting B/D releases hidden remote processing, and reconnection reapplies the current controller state.

### 1.8.5

- 中文：放慢 C/D 音量操作；OVERLAY 的 Alt 恢复 0 dB，MIX 保留平均分配。全局 ECO/FULL 记住用户上次选择，独立于新实例默认 FULL。
- English: Slows C/D gain controls. Alt resets OVERLAY to 0 dB while MIX retains equal-share reset. The global ECO/FULL choice persists independently of new instances starting in FULL.

### 1.8.4

- 中文：D 的 OVERLAY 使用 dB 显示，与 MIX 百分比互相换算，最大 +12 dB。超过 100% 时颜色填充仍限制在音量块边界。
- English: Displays D OVERLAY gain in dB, sharing values with MIX percentages up to +12 dB. Fill remains bounded when percentages exceed 100%.

### 1.8.3

- 中文：将 D 的新模式命名为 OVERLAY，修复单路频谱显示并计入音量；保留与 MIX 共用的混合音量和 Link，以及流畅的模式切换。
- English: Renames the new D mode OVERLAY, fixes per-source spectra with applied gain, and retains shared MIX gains, Link and smooth mode changes.

### 1.8.2

- 中文：为 D 加入首次交付时名为 FULL 的叠加分析模式：共用 MIX 的音量和 Link，分别查看各 Group 的图表与数值，同时显示总 MIX。此名称在 1.8.3 改为 OVERLAY。
- English: Introduces D's layered analysis mode, initially named FULL, with shared MIX gains and Link, per-Group graphs/readings and the total MIX result. Version 1.8.3 renames it OVERLAY.

## 下载 / Downloads

四个平台 ZIP、两份安装说明和两本手册，共八个附件。源码保持私有。GitHub 自动生成的 Source code 压缩包只包含本公开仓库文档。

Eight assets: four platform ZIPs, two installation guides and two manuals. Product source stays private; GitHub's automatic Source code archives contain public repository documentation only.

- [QQ ChainScope 1.8.17 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ.ChainScope.1.8.17.txt)
- [QQ-ChainScope-1.8.17-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ-ChainScope-1.8.17-Installation-Guide-English.txt)
- [QQ-ChainScope-1.8.17-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ-ChainScope-1.8.17-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.8.17-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ-ChainScope-1.8.17-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.8.17-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ-ChainScope-1.8.17-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.8.17-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ-ChainScope-1.8.17-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.8.17.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ.ChainScope.v1.8.17.pdf)
- [QQ ChainScope User Manual English v1.8.17.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.17/QQ.ChainScope.User.Manual.English.v1.8.17.pdf)
