# Changelog

[中文](CHANGELOG.md)

## 0.3.2 — Plugin ordering, classification, and light theme

### Plugins

- Reordering now reuses loaded VST instances and only changes DSP processing order; plugins are no longer destroyed and reloaded.
- Plugin parameters, bypass, send level, alias, and instance state follow the plugin.
- VST3/VST3i classification follows the primary plugin type; VST2 uses Synth/Instrument metadata.
- Legacy catalog entries are migrated automatically; VST2 plugins with unverifiable type metadata are no longer treated as usable effects.
- Stereo suffixes from vendors such as Waves are hidden only when a matching Mono variant exists. Genuine standalone Stereo names remain unchanged.

### UI

- The light-theme LED now uses a bright background with dark text, with adjusted screen, value, and send-bar contrast.
- Dark and light theme screenshots are included in the public release description.

### Installer

- Version updated to `0.3.2`.

## 0.3.1 — First public release

First public binary release, covering the completed console, driver deployment, resident audio
service, plugin host, loopback system, and long-term stability work.

### Device and runtime

- Automatic UP2 SE detection, firmware/driver versions, and device reset.
- Resident audio service, independent ASIO engine, tray operation, and stable startup ordering.
- Global show hotkey, volume/mute hotkeys, tray-wheel control, and dedicated OSD.
- Dark/light/system themes, Chinese/English UI, smoother text, zoom, and window-position persistence.

### Mixer

- Input, system, Loop, OTG, and physical-output channels.
- Faders, mute, solo, pan, stereo width, groups, and animated controls.
- Five sends with unified drag, wheel, double-click, and pre/post behavior.
- Persistence for channel parameters and visibility layouts.
- `+15/0/-15 dB` speaker/headphone calibration and protected global output volume.

### IN and plugins

- IN gain, 48V, 20 dB pad, INS, phase invert, and 48V safety mute.
- VST2/VST3/CLAP scanning, standards-based type filtering, native editors, Insert/Send, reorder, and state persistence.
- Private ASIO return for IN processing and background plugin preloading.
- Fix incorrect exclusion of 2.0 effects such as Guitar Rig that expose both Instrument and Fx metadata.
- Fix missing unprocessed IN routing to ASIO Loop.
- Calibrate the `3.01 dB` difference between direct IN capture and an unprocessed ASIO Loop recording.

### Loopback and configuration

- Independent WDM/ASIO Loop targets, post-fader level, DIM, mute, solo, width, and meters.
- Route recovery after target switching and USB reconnect.
- Console presets, plugin parameters, restore-default, and asynchronous loading.
- Plugin folders, failed-only rescan, search, and exclusion reasons.

### Known limitations

- Platane UP2 SE only.
- Some older DAWs cannot switch sample rate or buffer size while running.
- Updates briefly restart the audio stack.
- The installer is not commercially code-signed.

