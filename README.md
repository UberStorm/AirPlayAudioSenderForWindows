<div align="center">

# 🎵 AirPlay Audio Sender (Windows to HomePod)

**A beautifully designed, highly optimized, completely FREE Windows application that streams your PC audio directly to your Apple AirPlay speakers.**

Developed with ❤️ by **Maor Eliezer**

</div>

---

## ✨ Features

- **Seamless PC-to-HomePod Streaming**: Wirelessly push your Windows system audio to any AirPlay-compatible speaker on your network.
- **Multiple Device Support**: Stream to multiple speakers at the very same time.
- **Per-Application Audio Routing**: (New!) Select a specific application (e.g., Spotify, Chrome) from the drop-down menu to stream *only* that app's audio to your HomePod, while keeping system sounds on your PC. No virtual audio cables required!
- **True Stereo Pair Detection**: Automatically groups paired HomePods into a single entity (🔗) for effortless control, just like native Apple devices.
- **Intelligent "Zero-Stutter" CPU Priority**: Automatically elevates its own Windows process priority to `HIGH_PRIORITY_CLASS` during streaming, mathematically preventing background audio stutter even while gaming.
- **Wi-Fi Mesh Network Diagnostics**: Built-in ping monitor that pings *both* your Router and your HomePod simultaneously, showing exactly where network lag is originating (`Router: 2ms → Speaker: 50ms 🟢`).
- **Dual Auto-Recovery Watchdogs**: Features both an audio watchdog (recovers if Windows kills the loopback stream) and a network watchdog (automatically reconnects if a HomePod drops off Wi-Fi).
- **O(1) Zero-Copy Streaming Engine**: Utilizes a highly optimized, lock-free `deque` memory buffer and hardware-level chunking to keep background streaming CPU usage near 0%.
- **Ultra-Low Latency Configuration**: Fine-tune your audio buffer to eliminate delay, starting from a razor-thin 1024-frame raw WASAPI capture base.
- **Smart Device Recognition**: Automatically detects and displays your specific device models (e.g., *HomePod mini*, *Apple TV 4K*).
- **Independent Volume Control**: Individual, dynamic volume sliders for every single speaker you connect to.
- **Minimize to System Tray**: Keep your desktop clean. The app can minimize to your Windows system tray and run silently in the background.
- **Zero Configuration**: No complicated virtual audio cables or external dependencies required for basic streaming. Just open the app, click connect, and listen.
- **Gorgeous UI Customization**: Built with `CustomTkinter`, featuring a sleek, dark-mode-first modern aesthetic with fluid animations.

---

## 🚀 How to Use

1. Download the latest **`AirPlayAudioSender.exe`** from the [Releases](#) tab on the right.
2. Ensure your Windows PC and your AirPlay speakers are on the **same Wi-Fi network**.
3. Run the executable (no installation required!).
4. Select your desired **Audio Source** (e.g., System Audio or a specific running app).
5. Check the boxes next to the speakers you want to stream to.
6. Click **Connect** and enjoy!

---

## 💸 Completely Free

This software was developed by **Maor Eliezer** to solve the pain point of using Apple HomePods natively on a Windows machine. It is **100% completely free and open-source**. There are no ads, no premium versions, and no paywalls. 

---

## 📜 Changelog

### v1.2.0 (Latest)
- **⚡ Faster Startup**: Re-engineered the initialization sequence to draw the UI instantly while heavy audio and network engines load smoothly in the background.
- **✨ Auto-Optimize Latency Mode**: A smart new button in the Settings menu that calculates your current network ping (Router + Speaker) + jitter, and mathematically snaps your stream to the absolute lowest safe latency.
- **🚀 Ultra-Low 75ms Floor**: Removed the old 100ms restriction. If your network is fast enough, the app now allows you to push latency all the way down to a blistering 75ms for near-instant playback! This is the lowest it will ever be.
- **🟢 Robust Diagnostics**: Replaced unstable string-parsing with native `route print -4` to ensure the Router MS ping works perfectly across all international Windows locales (including Hebrew!). Added a `Total:` latency readout.

### v1.1.0
- **🎧 Ghost Volume**: Added the ability to mute a specific application (like Spotify) on your local PC speakers, while simultaneously streaming its audio to your HomePod! Perfect for listening to music while talking on Discord.
- **🎨 UI Overhaul**: Redesigned the entire user interface to be fully responsive. Added a sleek new Settings window, dynamic Audio Level VU meter, and modernized layout elements.
- **🔄 Auto-Refresh**: The app now automatically scans for Audio Sources and AirPlay devices the moment you open it.

---

## 📝 License
This project is provided "as is" and is free to use and distribute. Developed by Maor Eliezer.
