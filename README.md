<div align="center">

# 🎵 AirPlay Audio Sender (Windows to HomePod)

**A beautifully designed, highly optimized, completely FREE Windows application that streams your PC audio directly to your Apple AirPlay speakers.**

Developed with ❤️ by **Maor Eliezer**

</div>

---

## ✨ Features

- **Seamless PC-to-HomePod Streaming**: Wirelessly push your Windows system audio to any AirPlay-compatible speaker on your network.
- **Multiple Device Support**: Stream to multiple speakers at the very same time.
- **True Stereo Pair Detection**: Automatically groups paired HomePods into a single entity (🔗) for effortless control, just like native Apple devices.
- **Highly Optimized Audio Engine**: Uses smart VU meter throttling and peak-detection to keep background CPU usage near 0% while streaming.
- **Smart Device Recognition**: Automatically detects and displays your specific device models (e.g., *HomePod mini*, *Apple TV 4K*).
- **Independent Volume Control**: Individual, dynamic volume sliders for every single speaker you connect to.
- **Real-Time Network Diagnostics**: Built-in ping monitor that displays your actual network latency and connection health (🟢/🟡/🔴) in real-time.
- **Minimize to System Tray**: Keep your desktop clean. The app can minimize to your Windows system tray and run silently in the background.
- **Ultra-Low Latency Configuration**: Fine-tune your audio buffer to eliminate delay.
- **Zero Configuration**: No complicated virtual audio cables or external dependencies required for basic streaming. Just open the app, click connect, and listen.
- **Gorgeous UI Customization**: Built with `CustomTkinter`, featuring a sleek, dark-mode-first modern aesthetic with fluid animations.

## 💸 Completely Free

This software was developed by **Maor Eliezer** to solve the pain point of using Apple HomePods natively on a Windows machine. It is **100% completely free and open-source**. There are no ads, no premium versions, and no paywalls. 

---

## 🚀 How to Use (For Users)

1. Download the latest **`AirPlayAudioSender.exe`** from the [Releases](#) tab on the right.
2. Ensure your Windows PC and your AirPlay speakers are on the **same Wi-Fi network**.
3. Run the executable (no installation required!).
4. Check the boxes next to the speakers you want to stream to.
5. Click **Connect** and enjoy!

---

## 🛠️ How to Build (For Developers)

If you want to compile the source code into an executable yourself, make sure you have Python 3.10+ installed and run the following command:

```cmd
pyinstaller --noconfirm --onefile --windowed --icon=icon.ico --add-data "icon.ico;." --collect-all customtkinter --collect-all pystray --collect-all PIL --name AirPlayAudioSender main.py
```

## 📝 License
This project is provided "as is" and is free to use and distribute. Developed by Maor Eliezer.
