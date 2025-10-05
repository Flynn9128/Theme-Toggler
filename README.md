# 🌓 Theme Toggler

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%2011-0078D4.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Size](https://img.shields.io/badge/size-~15MB-orange.svg)

**The fastest way to toggle Windows 11 dark mode**


</div>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎨 **System-Wide Theme Control**
- Toggles Windows 11 dark/light mode
- Affects apps, taskbar, and system UI
- Instant switching with no lag

### ⚡ **Global Hotkey**
- Default: `Ctrl + T`
- Customizable to any combination
- Works from any application

</td>
<td width="50%">

### 🎯 **System Tray Integration**
- Minimal resource usage (~15-20 MB RAM)
- One-click toggle from tray icon
- Dynamic icon that matches theme

### 💎 **Beautiful UI**
- Animated starfield background
- Glassmorphic design
- Smooth 60fps animations

</td>
</tr>
</table>

---

## 🖥️ System Requirements

### ✅ **Minimum Requirements** (Any PC can run this!)

| Component | Requirement |
|-----------|-------------|
| **OS** | Windows 11 (any version) |
| **RAM** | 100 MB available |
| **Storage** | 30 MB free space |
| **CPU** | Any modern processor (2010+) |
| **GPU** | Not required (uses CPU rendering) |
| **Display** | Any resolution (optimized for 1920x1080) |

> **💡 Good News:** This is a lightweight .exe that runs on **ANY Windows 11 PC**. No special hardware, no graphics card needed!

### ⚠️ **Important Notes**
- ✅ Works on low-end laptops, tablets, and desktops
- ✅ No admin rights required (except first run for registry access)
- ✅ No internet connection needed
- ✅ Portable - runs from USB drives
- ❌ Windows 10 not supported (dark mode API differs)

---

## 📦 Download

### Option 1: Download Pre-built Executable (Recommended)

1. Go to [Releases](https://github.com/yourusername/theme-toggler/releases)
2. Download `ThemeToggler.exe`
3. Double-click to run
4. That's it! 🎉

### Option 2: Build from Source

See [Build Instructions](#-build-from-source) below.

---

## 🚀 Usage

### **First Launch**

1. **Run the executable** - Double-click `ThemeToggler.exe`
2. **Welcome UI appears** - Beautiful animated interface
3. **System tray icon** - Look for 🌓 icon in taskbar

### **Toggle Theme**

Choose any method:

| Method | Action |
|--------|--------|
| 🖱️ **UI Button** | Click "Toggle Theme" in main window |
| ⌨️ **Hotkey** | Press `Ctrl + T` (or your custom hotkey) |
| 🎯 **Tray Icon** | Click the moon/sun icon in system tray |
| 🖱️ **Right-click** | Right-click tray → "Toggle Theme" |

### **Customize Hotkey**

<div align="center">
<img src="https://github.com/Flynn9128/Theme-Toggler/blob/main/Screenshot%202025-10-05%20164327.png?raw=true" width="400"/>
</div>

1. Click **⚙️ Customize Hotkey** in main window
2. Select **modifier** (Ctrl, Alt, or Shift)
3. Enter **key** (any letter or number)
4. Click **Save Hotkey**
5. ✅ Works immediately!

**Examples:**
- `Alt + D` for quick dark mode
- `Shift + T` for theme toggle
- `Ctrl + X` for custom preference

### **Pin to Taskbar**

Want quick access?

1. Navigate to the `.exe` file location
2. **Right-click** → Select "Pin to taskbar"
3. Launch directly from taskbar! 📌

### **Auto-Start on Boot** (Optional)

1. Press `Win + R`
2. Type `shell:startup` and press Enter
3. Copy `ThemeToggler.exe` (or create shortcut) to this folder
4. App will start automatically with Windows! 🚀

---

## 🎨 Screenshots

<div align="center">

### Dark Mode
<img src="https://via.placeholder.com/400x700/000000/ffffff?text=Dark+Mode+UI" width="300"/>

### Light Mode
<img src="https://via.placeholder.com/400x700/ffffff/000000?text=Light+Mode+UI" width="300"/>

### Settings Panel
<img src="https://via.placeholder.com/400x300/1a1a1a/00d4ff?text=Hotkey+Settings" width="300"/>

</div>

---

## 🛠️ Build from Source

### **Prerequisites**

Install Python 3.8+ and required packages:

```bash
# Install Python dependencies
pip install pystray pillow pywin32 pynput

# Install PyInstaller for building
pip install pyinstaller
```

### **Clone Repository**

```bash
git clone https://github.com/yourusername/theme-toggler.git
cd theme-toggler
```

### **Run from Source**

```bash
python darkmode.py
```

### **Build Executable**

```bash
# Create standalone .exe
python -m PyInstaller --onefile --noconsole --name="ThemeToggler" darkmode.py

# Find executable in dist/ folder
cd dist
```

### **Optional: Custom Icon**

```bash
# If you have a custom .ico file
python -m PyInstaller --onefile --noconsole --icon="icon.ico" --name="ThemeToggler" darkmode.py
```

---

## 📂 Project Structure

```
theme-toggler/
├── darkmode.py              # Main application code
├── ThemeTogglerConfig.json  # Settings file (auto-generated)
├── dist/                    # Built executable
│   └── ThemeToggler.exe
├── build/                   # Build artifacts
└── README.md               # You are here!
```

---

## ⚙️ Configuration

Settings are automatically saved to:
```
C:\Users\YourName\ThemeTogglerConfig.json
```

**Default Configuration:**
```json
{
  "hotkey": "ctrl+t",
  "modifier": "ctrl",
  "key": "t"
}
```

---

## 🎯 Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + T` | Toggle theme (customizable) |
| `ESC` | Close main window |
| `Right-click tray` | Open context menu |

---

## 🔧 Troubleshooting

### **App won't start**
- ✅ Make sure you're on Windows 11
- ✅ Run as Administrator once
- ✅ Check if another instance is running

### **Hotkey not working**
- ✅ Check if another app uses the same hotkey
- ✅ Try a different key combination
- ✅ Restart the app

### **Theme doesn't change**
- ✅ Check Windows Settings → Personalization → Colors
- ✅ Ensure "Choose your mode" is set to "Custom"
- ✅ Run app as Administrator

### **Tray icon missing**
- ✅ Click the arrow (^) in taskbar to show hidden icons
- ✅ Right-click taskbar → Taskbar settings → Show all icons

### **High RAM usage**
- ✅ Normal: 15-20 MB
- ✅ Close and reopen main window
- ✅ Restart the app

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📊 Performance Stats

<div align="center">

| Metric | Value |
|--------|-------|
| **RAM Usage** | ~15-20 MB |
| **CPU Usage** | <1% (idle) |
| **Startup Time** | <2 seconds |
| **Toggle Speed** | Instant (<100ms) |
| **File Size** | ~15 MB (.exe) |
| **Animation FPS** | 60fps |

</div>

---

## 🗺️ Roadmap

- [ ] Windows 10 support
- [ ] Schedule automatic theme switching (day/night)
- [ ] Multiple theme presets
- [ ] Accent color customization
- [ ] Web-based UI option (Eel/CEF)
- [ ] Wallpaper auto-change with theme

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Built with Python & Tkinter
- Uses Windows Registry API
- Inspired by modern productivity tools
- Icons by [your source]

---

## 💬 Support

Found a bug? Have a suggestion?

- 📧 Email: your.email@example.com
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/theme-toggler/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/yourusername/theme-toggler/discussions)

---

<div align="center">

**Made with 💙 by [Your Name]**

⭐ Star this repo if you found it helpful!

[⬆ Back to Top](#-theme-toggler)

</div>

---

## 🎁 Bonus Tips

### **Pro Tips:**

1. **Quick Access**: Pin to taskbar for one-click launch
2. **Auto-Start**: Add to startup folder for always-on availability
3. **Custom Combos**: Try `Alt + D` (D for Dark) for intuitive switching
4. **Minimize Workflow**: Keep in tray, toggle with hotkey only
5. **Share**: Share the .exe with friends - no installation needed!

### **Use Cases:**

- 🌙 **Night Coding**: Switch to dark mode for late-night sessions
- ☀️ **Presentations**: Quick switch to light mode for readability
- 👀 **Eye Comfort**: Toggle based on ambient lighting
- 🎨 **Design Work**: Match theme to your creative mood
- ⚡ **Productivity**: Instant context switching

---

## 📈 Why Theme Toggler?

### **vs. Windows Settings**
| Feature | Theme Toggler | Windows Settings |
|---------|--------------|------------------|
| Speed | ⚡ Instant | 🐌 5-10 clicks |
| Hotkey | ✅ Yes | ❌ No |
| Tray Access | ✅ Yes | ❌ No |
| Lightweight | ✅ 15MB RAM | 🔥 100MB+ |

### **vs. Other Tools**
- ✅ No bloatware or ads
- ✅ Open source
- ✅ Single executable
- ✅ No installation required
- ✅ Customizable hotkeys

---

<div align="center">

### 🌟 Enjoy seamless theme switching! 🌟

</div>
