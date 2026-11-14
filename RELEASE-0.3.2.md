> **个人项目，无任何商业用途。仅支持 Platane UP2 SE。**
>
> **Personal project, non-commercial use only. Platane UP2 SE only.**

## 中文

`0.3.2` 集中优化了插件排序、插件类型过滤和浅色主题。

```text
* 插件排序复用已加载实例，只改变 DSP 处理顺序，不再重新加载插件
* 参数、旁通、发送量、别名和实例状态跟随插件移动
* VST3/VST3i 按主类型识别，VST2 使用 Synth/Instrument 类型信息
* 自动迁移旧插件缓存，过滤 EZbass、Superior Drummer 3、Ample 等乐器
* Waves 等同厂 Mono/Stereo 成对插件隐藏 Stereo 后缀，独立 Stereo 名称保留
* 浅色主题 LED 改为亮底深字
* 公开发行说明加入深色与浅色主题截图
```

### 注意事项

- 仅支持 Platane UP2 SE。
- 安装前退出 DAW 和所有使用 ASIO 的程序。
- 第一次运行 `0.3.2` 会自动重扫一次旧插件缓存，之后启动不再重复扫描。
- 安装包未做商业代码签名。

安装包 SHA-256：

```text
3914ACB17277E9FCB99957DBABEF44C9E3C1146AD17EFFC619CB7EEEC2A4EEED
```

## English

`0.3.2` focuses on plugin ordering, plugin type filtering, and the light theme.

```text
* Plugin reordering reuses loaded instances and only changes DSP processing order
* Parameters, bypass, send level, alias, and instance state follow the plugin
* VST3/VST3i uses the primary plugin type; VST2 uses Synth/Instrument metadata
* Legacy catalogs are migrated automatically, filtering instruments such as EZbass, Superior Drummer 3, and Ample
* Stereo suffixes are hidden for paired Mono/Stereo plugins; genuine standalone Stereo names remain
* Light-theme LED uses a bright background with dark text
* Public release description includes dark and light theme screenshots
```

### Important

- Platane UP2 SE only.
- Close DAWs and all ASIO applications before installing.
- The first `0.3.2` launch rescans the legacy plugin catalog once; later launches do not rescan automatically.
- The installer is not commercially code-signed.

Installer SHA-256:

```text
3914ACB17277E9FCB99957DBABEF44C9E3C1146AD17EFFC619CB7EEEC2A4EEED
```

