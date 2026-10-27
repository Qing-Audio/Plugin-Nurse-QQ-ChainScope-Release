# QQ ChainScope 1.8.18 Stable



## 本次更新 / Changes since 1.8.17



### 1.8.18 — MIDI 全范围音量映射 / Full-range MIDI level mapping



- 中文：C/D Mixboard 新增 SOURCE n LEVEL 完整范围参数，音量块可通过 Cubase MIDI Remote／快速控制从静音控制到 +12 dB（约 398.1%）。修正绑定到 BOOST 后最低位置只能到绑定时音量的问题。若已有映射选择了 SOURCE n BOOST，请重新学习音量块或手动选择 SOURCE n LEVEL。

- English: C/D Mixboard now expose full-range SOURCE n LEVEL parameters, allowing Cubase MIDI Remote / Quick Controls to control gain blocks from silence to +12 dB (about 398.1%). This fixes mappings to BOOST being unable to go below the gain present when learned. Relearn the gain block or select SOURCE n LEVEL if an existing mapping targets SOURCE n BOOST.

- 中文：B/C/D 单推子和 L/R 推子的学习通知、点击目标已修正，使用原有静音至 +30 dB 的绝对范围；旧参数编号、范围与工程状态保持兼容。原有 Link、音频处理和图表功能保持不变。

- English: Learning notifications and hit targets are corrected for B/C/D single and L/R faders, retaining the absolute range from silence to +30 dB. Existing parameter identifiers, ranges and saved states remain compatible. Link, audio processing and graph behavior are unchanged.

- 中文：2026-10-27 文档补充：中英文手册功能概览更新为 13 项，MASKING 位于第 8 项；第 13 项加入 D Mixboard 的独立分析与监听。插件成品保持不变。

- English: Documentation update, 2026-10-27: both manuals now list 13 capabilities, with MASKING at item 8 and D Mixboard included in standalone analysis and monitoring at item 13. Plug-in binaries are unchanged.



## 它能帮你做的 13 件事 / Thirteen things it helps you do

| # | 中文 | English |
|---|---|---|
| 1 | **对比处理前／后**：查看 Peak、True Peak、RMS、LUFS-I、Spectrum 与 Waveform。 | **Compare before and after**: View Peak, True Peak, RMS, LUFS-I, Spectrum, and Waveform. |
| 2 | **匹配前／后音量**：用 Match 减少“更响所以更好听”的误判。 | **Match before / after loudness**: Use Match to avoid mistaking louder for better. |
| 3 | **Dry / Wet 与 ADD Wet**：混合原声（Dry）与效果器处理后的声音（Wet）；打开 ADD，可保持原声 100%，再把处理后的声音叠加上去。 | **Dry / Wet and ADD Wet**: Blend the original sound (Dry) with the sound after effects (Wet). Enable ADD to keep Dry at 100% and layer the processed sound on top. |
| 4 | **校准相位偏移**：检查并修正处理链带来的相位偏移。 | **Correct phase offsets**: Inspect and correct phase offsets introduced by the processing chain. |
| 5 | **校准硬件左右电平**：修正硬件额外引入的 L/R 失配，保留素材原有的立体声关系。 | **Calibrate hardware L/R levels**: Correct the extra L/R mismatch introduced by hardware while preserving the source stereo relationship. |
| 6 | **修正残余延迟**：部分插件误报延迟，导致 DAW 无法正确补偿时，用 Latency Rescue 补齐。 | **Correct residual latency**: If a plug-in reports the wrong latency and the DAW cannot compensate correctly, use Latency Rescue to close the gap. |
| 7 | **EQ Match 音色匹配**：让 Wet 或 Main Out（Dry/Wet 混合后的信号）的音色接近 Before，自由调整匹配强度和频段。 | **Match tone with EQ Match**: Bring Wet or Main Out (the signal after Dry/Wet mixing) closer to Before. Adjust the correction amount and frequency range. |
| 8 | **查看轨道间的遮蔽效应**：在 C/D Mixboard 的 OVERLAY 中开启 MASKING，通过频谱和 Waveform 阴影查看轨道间可能存在的遮蔽。 | **Check masking between tracks**: Enable MASKING in C/D Mixboard OVERLAY to see possible masking between tracks as shading on the spectrum and waveform. |
| 9 | **把硬件现场留在工程里**：用 Chain Note 保存旋钮照片、接线、参数与备注。 | **Keep hardware notes in the session**: Use Chain Note to save knob photos, patching, settings, and comments. |
| 10 | **单轨比较或混合多套方案**：用 C Mixboard 比较处理前的原始信号和最多四组效果器方案的差异，或按比例混合。 | **Compare or mix chains on one track**: Use C Mixboard to compare the original signal with up to four effects chains, or blend them by percentage. |
| 11 | **跨轨对比与混合**：用 B Return 对比两条轨道，通过 Dry/Wet 调整两轨的音量比例。 | **Compare and blend two tracks**: Use B Return to compare two tracks and adjust their level balance with Dry/Wet. |
| 12 | **集中控制六路声音**：用 D Mixboard 控制最多六个分轨，进行比较、混合、监听和 EQ Match。 | **Control up to six tracks**: Use D Mixboard to compare, mix, monitor, and EQ Match up to six tracks. |
| 13 | **独立分析与监听**：B Return、C Mixboard、D Mixboard 可独立查看图表，调节音量、声像、极性与监听。 | **Standalone analysis and monitoring**: Use B Return, C Mixboard or D Mixboard on its own to view graphs and control level, pan, polarity, and monitoring. |

## 下载 / Downloads



- [QQ ChainScope 1.8.18 安装说明（中文版）.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.1.8.18.txt)

- [QQ-ChainScope-1.8.18-Installation-Guide-English.txt](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-Installation-Guide-English.txt)

- [QQ-ChainScope-1.8.18-Windows-x64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-Windows-x64-VST3.zip)

- [QQ-ChainScope-1.8.18-macOS-Apple-Silicon-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Apple-Silicon-VST3.zip)

- [QQ-ChainScope-1.8.18-macOS-Intel-x86_64-VST3.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Intel-x86_64-VST3.zip)

- [QQ-ChainScope-1.8.18-macOS-Universal-2-AU.zip](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ-ChainScope-1.8.18-macOS-Universal-2-AU.zip)

- [QQ ChainScope 用户手册（中文版）v1.8.18.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.v1.8.18.pdf)

- [QQ ChainScope User Manual English v1.8.18.pdf](https://github.com/Qing-Audio/Plugin-Nurse-QQ-ChainScope-Release/releases/download/v1.8.18/QQ.ChainScope.User.Manual.English.v1.8.18.pdf)



## 安装与兼容性 / Installation and compatibility



- 中文：Windows 使用 x64 VST3。Mac 原生 Apple Silicon 宿主选 arm64 VST3；Intel／Rosetta 宿主选 x86_64 VST3，二者只装一套。AU 使用 Universal 2，包含 arm64 与 x86_64。每包包含 A/B/C/D 四件套，请一起升级；替换前退出所有音频宿主并备份工程。

- English: Use x64 VST3 on Windows. On Mac, choose arm64 VST3 for native Apple Silicon hosts or x86_64 VST3 for Intel/Rosetta hosts; install only one VST3 architecture. Universal 2 AU contains both architectures. Each package includes A/B/C/D; upgrade all four together. Close audio hosts and save a session copy before replacing plug-ins.

- 中文：Mac 成品使用 ad-hoc 签名，未经过 Apple Developer ID 公证。Windows 成品复用已验证构建，Mac 成品经对应架构构建、签名检查及原生／Rosetta 插件接口测试。自动化测试不代表所有 DAW 与实体 MIDI 控制器组合均已验收。

- English: Mac builds use ad-hoc signatures without Apple Developer ID notarization. The verified Windows build is reused. Mac builds are checked for architecture, signatures and native/Rosetta plug-in interface behavior. Automated testing does not certify every DAW and physical MIDI controller combination.

- 中文：MASKING 仍属于试验性辅助分析，SENS 默认 20、REF SPL 默认 75；阴影需结合听感判断。源码保持私有，本 Release 仅提供成品与文档。

- English: MASKING remains experimental visual assistance with defaults of SENS 20 and REF SPL 75; interpret shading with listening judgment. Source remains private; this Release distributes compiled products and documentation only.

