# QQ ChainScope 1.8.0

发布日期 / Release date: 2026-10-14

## 本次变化 / Changes since 1.7.25

### 1.7.26
- 中文：C/D 新增按来源名称、颜色和位置对应的 TP、综合响度与 RMS。FULL/ECO 都从播放起点持续累计 MIX，停止后保持，模式切换不清零。
- English: C/D add source TP, integrated loudness and RMS readings matching source names, colors and positions. FULL/ECO continuously accumulate MIX from Play and retain it through Stop and mode changes.

### 1.7.27
- 中文：COMPARE 数值区移到来源按钮与 Monitor 之间；MIX 卡片直接显示数值，列顺序统一为 I / RMS / TP。MIX 页移除重复卡片；设置页隐藏顶部局部模式按钮及 B 的 NOTE。
- English: COMPARE readings move between source selection and Monitor; MIX readings are visible with I / RMS / TP column order. MIX removes duplicate cards; Settings hides the local mode button and B NOTE.

### 1.7.28
- 中文：C 只显示实际 Return，D 只显示可用的已连接 Group；试听、比例与数值区紧凑排列，名称、颜色和真实连接关系保持一致。
- English: C shows existing Returns and D shows connected available Groups. Listening, proportions and reading cards use compact matching names, colors and connections.

### 1.7.29
- 中文：设置中的全局 ECO/FULL 显示最近的全局选择，与当前单个插件的模式分开。点击全局会更新所有现有 B/C/D，单个调整不改全局显示。中英文手册补充数值、动态来源与全局/局部模式示例。
- English: Settings shows the last global ECO/FULL choice separately from the local instance mode. Global clicks update all existing B/C/D; local changes leave the global display unchanged. Bilingual manuals add source readings, dynamic-source and global/local examples.

### 1.7.30
- 中文：B/C/D 波形悬停改为一行带名称和相减顺序的差值；频谱使用“平均差／峰值差”，保留频率及两路名称。
- English: B/C/D waveform hover uses one named subtraction. Spectrum uses readable Chinese average/peak difference labels, retaining frequency and both source names.

### 1.8.0
- 中文：提高 True Peak 检测精度；响度、RMS、声音处理、停止保持及重置规则保持不变。中英文手册同步到 1.8.0，补充 TP 及图表差值说明。
- English: Improves True Peak detection precision while preserving loudness, RMS, audio processing, Stop hold and Reset behavior. Both manuals are updated to 1.8.0 with TP and graph-difference guidance.

## 安装与升级 / Installation and upgrade

先保存工程并关闭宿主，再完整更新 A Send、B Return、C Mixboard、D Mixboard 四件套，必要时重新扫描。Windows 使用 x64 VST3。Mac 按宿主架构选择 Apple Silicon 或 Intel VST3，两套只装一套；Universal 2 AU 同时包含两种架构。详细步骤见安装说明。

Save the session and quit the host before updating all four A/B/C/D components; rescan if necessary. Use x64 VST3 on Windows. On Mac, install one VST3 architecture matching your host: Apple Silicon or Intel. Universal 2 AU includes both architectures. See the installation guides.

## 行为与兼容性 / Behavior and compatibility

TP 精度升级不改变声音处理、LUFS、RMS 或停止保持与重置规则。无需重新设置工程。图表差值保留名称和相减顺序。设置中的全局 ECO/FULL 与顶部单个模式分开显示；新插入的插件默认 FULL。全局切换作用于同一宿主进程里的现有 B/C/D，宿主跨进程隔离时需分别调整。悬停帮助及差值标题目前为中文。中英文手册各 54 页。

The TP precision update preserves audio processing, LUFS, RMS, Stop hold and Reset behavior. No session reconfiguration is needed. Graph differences retain names and subtraction order. Global Settings and local header modes are displayed separately; new inserts default to FULL. Global changes reach existing B/C/D within the same host process; adjust separately across isolated host processes. Hover help and difference headings are currently Chinese. Both manuals have 54 pages.

## 平台、验证与已知限制 / Platforms, checks and known limits

Windows 10/11 x64；macOS 11.0 或更新系统。Mac 文件为 ad-hoc 签名，未经 Apple Developer ID 公证。发布检查包含同源、版本、架构、签名、文件完整性及原生回归测试。TP 对照使用相同输入与独立参考实现；这不表示所有测量插件在所有素材上完全一致，也不是新增的 DAW 听感测试。QQ Host 跨进程多轨兼容仍待处理。

Windows 10/11 x64; macOS 11.0 or later. Mac files use ad-hoc signatures without Apple Developer ID notarization. Release checks cover source identity, version, architecture, signatures, file integrity and native regressions. TP checks use identical input and an independent reference; they do not claim exact agreement with every meter on every signal or a new DAW listening test. QQ Host cross-process Multi Track compatibility remains pending.

计算开销随平台不同：Windows 表头微基准比旧检测器降低约 4–7%，Intel Mac 降低约 2–11%；M4 上增加约 31–34%，512 帧时单个立体声表头约 9.19 微秒。这是独立表头测量，不代表整个 DAW 的负载变化。

Processing cost varies by platform: the meter microbenchmark is about 4–7% lower on Windows and 2–11% lower on Intel Mac than the old detector. M4 is about 31–34% higher, at roughly 9.19 microseconds per stereo meter with 512 samples. This isolated measurement is not a whole-DAW load comparison.

## 下载 / Downloads

八个附件：四个平台 ZIP、两份安装说明、两份手册。产品源码保持私有。GitHub 自动生成的 Source code ZIP 仅含公开仓库的文档。

Eight assets: four platform ZIPs, two installation guides and two manuals. Product source stays private. GitHub's automatic Source code archives contain public repository documentation only.

- [QQ ChainScope 1.8.0 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ.ChainScope.1.8.0.txt)
- [QQ-ChainScope-1.8.0-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-1.8.0-Installation-Guide-English.txt)
- [QQ-ChainScope-1.8.0-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-1.8.0-Windows-x64-VST3.zip)
- [QQ-ChainScope-1.8.0-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-1.8.0-macOS-Apple-Silicon-VST3.zip)
- [QQ-ChainScope-1.8.0-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-1.8.0-macOS-Intel-x86_64-VST3.zip)
- [QQ-ChainScope-1.8.0-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-1.8.0-macOS-Universal-2-AU.zip)
- [QQ ChainScope 用户手册（中文版）v1.8.0.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ.ChainScope.v1.8.0.pdf)
- [QQ-ChainScope-User-Manual-English-v1.8.0.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.0/QQ-ChainScope-User-Manual-English-v1.8.0.pdf)
