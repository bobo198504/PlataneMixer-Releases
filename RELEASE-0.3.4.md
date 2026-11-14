> **个人项目，无任何商业用途。仅支持 Platane UP2 SE。**
>
> **Personal project, non-commercial use only. Platane UP2 SE only.**

## 中文

`0.3.4` 集中修复自研 ASIO 宿主的生命期问题，并补充锁屏/休眠恢复和多显示器窗口定位。

```text
* 补齐 ASIO reset/resync、采样率、缓冲和 Time Info 协议
* 回调停止时在常驻进程内部安全重建 ASIO 流，不再依赖外部杀进程
* 锁屏或休眠前释放自研 ASIO 宿主，解锁或唤醒后延迟恢复
* 切换显示器、分辨率或主屏后，控台按原显示器锚点恢复位置
* Windows 临时移动控台时不再触发吸附或覆盖保存位置
* 新增 audio-engine.health，记录回调数量和恢复状态
```

### 注意事项

- 仅支持 Platane UP2 SE。
- 安装前退出 DAW 和所有使用 Platane ASIO 的程序。
- 本次没有修改系统电源策略，也没有修改官方驱动二进制。
- 如果音频路径再次异常，可查看 `%LOCALAPPDATA%\PlataneMixer2\audio-engine.health`。
- 安装包未做商业代码签名。

安装包 SHA-256：

```text
E84070A85B3B585381516E6FC1FD342B94B11E9E895B4A3302F44F4C2D31FA0A
```

## English

`0.3.4` focuses on standalone ASIO host lifecycle stability, lock/suspend recovery, and
multi-monitor window placement.

```text
* Adds ASIO reset/resync, sample-rate, buffer, and Time Info protocol support
* Rebuilds the ASIO stream safely inside the resident process when callbacks stop
* Releases the standalone ASIO host before lock or sleep and restores it after resume
* Restores the console to its monitor anchor after display, resolution, or primary changes
* System-driven moves no longer trigger snapping or overwrite the saved position
* Adds audio-engine.health callback and recovery diagnostics
```

### Important

- Platane UP2 SE only.
- Close DAWs and all applications using Platane ASIO before installing.
- This release does not modify system power policy or the official driver binaries.
- If the audio path fails, inspect `%LOCALAPPDATA%\PlataneMixer2\audio-engine.health`.
- The installer is not commercially code-signed.

Installer SHA-256:

```text
E84070A85B3B585381516E6FC1FD342B94B11E9E895B4A3302F44F4C2D31FA0A
```
