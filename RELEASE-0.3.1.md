> **个人项目，无任何商业用途。仅支持 Platane UP2 SE。**
>
> **Personal project, non-commercial use only. Platane UP2 SE only.**

## 中文

首个公开二进制发行版，包含完整的 UP2 SE 替代控台、驱动部署、常驻音频服务、Loopback 路由、插件宿主、预置、主题、快捷键和音量 OSD。

### 主要内容

```text
* 完整输入、系统、Loop、OTG、SP、PH 通道和五路发送
* IN 增益、48V、20dB、INS、反相、安全静音和第三方 Insert/Send
* VST2 / VST3 / CLAP 插件扫描、原生窗口、排序、重命名和状态保存
* 独立 WDM / ASIO Loopback、推子后发送、DIM、Mute、Solo、宽度和电平
* 调音台预置、布局、插件参数、采样率和缓冲设置
* 音箱/耳机 +15/0/-15 dB 输出校正
* 深浅主题、中英界面、全局快捷键、托盘控制和新版 OSD
# 修复无插件 IN 无法发送到 ASIO Loop
# 修复 Guitar Rig 等 2.0 效果器被误判为乐器
* 校准 IN 直录与无插件 ASIO Loop 记录的电平
```

### 注意事项

- 仅支持 Platane UP2 SE。
- 安装前退出 DAW 和所有使用 ASIO 的程序。
- 升级会重启音频栈，播放可能短暂中断。
- 安装包未做商业代码签名。
- 建议安装前备份 `%LOCALAPPDATA%\PlataneMixer2`。

安装包 SHA-256：

```text
4783F4B61496CE33307D0E078E25583F4041C9EE45BCE6645423AA91DC72155C
```

## English

First public binary release with the complete UP2 SE replacement console, driver deployment,
resident audio service, loopback routing, plugin host, presets, themes, shortcuts, and volume OSD.

### Highlights

```text
* Full input, system, Loop, OTG, SP, and PH channels with five sends
* IN gain, 48V, 20 dB pad, INS, phase invert, safety mute, and third-party Insert/Send
* VST2 / VST3 / CLAP scanning, native editors, reorder, rename, and state persistence
* Independent WDM / ASIO loopback with post-fader level, DIM, mute, solo, width, and meters
* Console presets, layouts, plugin state, sample rate, and buffer settings
* +15/0/-15 dB speaker/headphone output calibration
* Dark/light themes, Chinese/English UI, global hotkeys, tray control, and the new OSD
# Fix unprocessed IN not reaching ASIO Loop
# Fix 2.0 effects such as Guitar Rig being misclassified as instruments
* Calibrate direct IN capture against unprocessed ASIO Loop recording level
```

### Important

- Platane UP2 SE only.
- Close DAWs and all ASIO applications before installing.
- Updates restart the audio stack; playback may briefly stop.
- The installer is not commercially code-signed.
- Back up `%LOCALAPPDATA%\PlataneMixer2` before installing.

Installer SHA-256:

```text
4783F4B61496CE33307D0E078E25583F4041C9EE45BCE6645423AA91DC72155C
```

