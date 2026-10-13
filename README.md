# AleClip for Windows 📋

<p align="center">
  <strong>A modern, lightweight native clipboard manager for Windows 10 &amp; 11.</strong><br>
  Built natively with C# and .NET 8 WPF.
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#privacy--philosophy">Privacy &amp; Philosophy</a> •
  <a href="#shortcuts">Keyboard Shortcuts</a> •
  <a href="#download--installation">Download</a> •
  <a href="#building-from-source">Build from Source</a> •
  <a href="#license">License</a>
</p>

---

## 👨‍💻 Developed By

**Developed by SoftAI Yazılım (Mehmet Akif Çifçi)**  
*Designed to be completely free, private, and accessible for everyone.*

---

## 🛡️ Privacy & Philosophy

- **Zero Data Collection**: AleClip contains **no telemetry, no analytics, no remote tracking, and no internet access**.
- **100% Local Storage**: All clipboard clips and settings are saved strictly on your local disk (`%LocalAppData%\AleClip\`).
- **Free for Everyone**: Free to use, free to share, and free to fork for personal or commercial workflows.
- **Open Source (MIT)**: Permissive open-source license allows anyone to inspect, modify, fork, and build their own customized versions.

---

## ✨ Features

- **Non-Activating Floating Panel (`WS_EX_NOACTIVATE`)**:
  Slides up smoothly from the bottom of your screen using `Alt + V` without stealing keyboard focus from your active apps (editors, browsers, IDEs).
- **Subtle Background Watermark**:
  Clean, unobtrusive `"ALE"` watermark rendered on the panel background layer.
- **Multi-Type Clipboard Support**:
  - Plain Text & Rich Text (RTF)
  - HTML snippets
  - URLs and Web Links (with one-click browser opening)
  - File Paths & File Drops
  - Hex / RGB Color Codes (with live swatch previews)
- **Quick Look (`Space`)**:
  Press `Space` on any card for an instant enlarged preview.
- **Direct Paste Injection (`Enter`)**:
  Synthesizes `Ctrl + V` directly into your foreground application.
- **Plain Text Paste (`Shift + Enter`)**:
  Strips formatting and pastes pure unformatted text on the fly.
- **Card-Based Settings Window**:
  - **General**: Configurable history limits (50–1000 items), paste behavior, and bilingual language switching.
  - **Shortcuts**: In-panel keyboard guide.
  - **Backup & Restore**: Export history to a standard `.json` file, restore with automatic deduplication, or clear unpinned items.
- **System Tray Agent**:
  Lightweight system tray icon with quick access to recent clips, settings, and unpinned history cleanup.
- **Bilingual Interface**:
  Full English (`en`) and Turkish (`tr`) localization with dotted/dotless `I/ı/İ/i` search case-folding.

---

## ⌨️ Shortcuts Reference

| Shortcut | Action |
| :--- | :--- |
| `Alt + V` | **Toggle Panel** (Open / Dismiss AleClip bottom panel from any app) |
| `←` `→` | **Navigate** between clipboard cards |
| `Enter` | **Paste** selected clip into active application |
| `Shift + Enter` | **Paste as Plain Text** (strips rich text / HTML styling) |
| `Space` | **Quick Look Preview** (fullscreen card inspection) |
| `Delete` | **Delete Clip** from history |
| `Esc` | **Close** panel without pasting |

---

## 📦 Download & Installation

Download the latest standalone executable from [GitHub Releases](https://github.com/themanoftalent/aleclip-windows/releases):

- **[AleClip.exe](https://github.com/themanoftalent/aleclip-windows/releases/latest/download/AleClip.exe)** — Standalone single-file executable (no installation required).
- **[AleClip-Windows-x64.zip](https://github.com/themanoftalent/aleclip-windows/releases/latest/download/AleClip-Windows-x64.zip)** — Compressed ZIP archive.

---

## 🛠️ Building from Source

### Requirements
- **Windows 10 / 11 (64-bit)**
- **.NET 8.0 SDK** or Visual Studio 2022

### Publish Single-File Executable
```bash
# Clone the repository
git clone https://github.com/themanoftalent/aleclip-windows.git
cd aleclip-windows

# Publish self-contained single-file binary
dotnet publish AleClip/AleClip.csproj -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true -o ./publish
```

The resulting `AleClip.exe` in `./publish/` is completely standalone and ready to run.

---

## 🍎 macOS Version

Looking for the native macOS version (Swift 6 / AppKit)?  
Visit: [**themanoftalent/aleclip**](https://github.com/themanoftalent/aleclip)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.  
Created and maintained by **SoftAI Yazılım (Mehmet Akif Çifçi)**.
