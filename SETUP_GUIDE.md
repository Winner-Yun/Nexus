# 📖 NEXUS Control Center User Setup & Getting Started Guide

This guide provides step-by-step instructions to install, configure, and master **NEXUS Control Center** on your Windows 10 or Windows 11 workstation.

---

## 📋 Table of Contents
1. [Installation](#1-installation)
2. [Configuring Background Tray & Startup Preferences](#2-configuring-background-tray--startup-preferences)
3. [Global Hotkeys & Command Palette](#3-global-hotkeys--command-palette)
4. [Using Core Modules](#4-using-core-modules)
   - [Telemetry Dashboard & Quick Controls](#telemetry-dashboard--quick-controls)
   - [Applications Catalog & Process Manager](#applications-catalog--process-manager)
   - [Tabbed File Explorer & Inspector](#tabbed-file-explorer--inspector)
   - [Screen Studio, MP4 Recorder & Android Mirroring](#screen-studio-mp4-recorder--android-mirroring)
   - [Storage Suite (TreeMap, Duplicates, Renamer, Hashes & Cleaner)](#storage-suite-treemap-duplicates-renamer-hashes--cleaner)
   - [Network Center & Diagnostics](#network-center--diagnostics)
   - [Hardware Devices & Driver Health](#hardware-devices--driver-health)
   - [Settings Applets, Custom Commands & Audit Logs](#settings-applets-custom-commands--audit-logs)
5. [Troubleshooting](#5-troubleshooting)

---

## 1. Installation

1. Navigate to the `installer` folder or download [**NEXUS-Setup-v1.0.0.exe**](installer/NEXUS-Setup-v1.0.0.exe).
2. *(Optional)* Verify the installer integrity against [installer/SHA256SUMS.txt](installer/SHA256SUMS.txt):
   ```powershell
   Get-FileHash .\installer\NEXUS-Setup-v1.0.0.exe -Algorithm SHA256
   ```
3. Double-click **NEXUS-Setup-v1.0.0.exe** to launch the setup wizard:
   - If Windows SmartScreen displays **Windows protected your PC**, click **More info** and select **Run anyway**.
4. Follow the setup prompts (installs to your Windows Programs directory and optionally creates a Desktop shortcut).
5. Click **Install**, then **Finish** to launch **NEXUS Control Center**.

---

## 2. Configuring Background Tray & Startup Preferences

NEXUS is engineered to stay instantly accessible with minimal resource usage:

1. Open **Settings** (`Ctrl+9`) > **General Preferences** (`Alt+1`).
2. **System Tray & Background Execution**:
   - Toggle **ON** to minimize NEXUS to the Windows notification area when closing the main window (`[X]`).
   - While in background mode, NEXUS automatically trims its physical RAM working set by ~90%+ (~15–25 MB) and wakes instantaneously on hotkey triggers.
3. **Windows Startup Auto-Launch**:
   - Toggle **ON** to launch NEXUS silently in the notification tray on Windows login (`HKCU\Software\Microsoft\Windows\CurrentVersion\Run`).
4. **Theme Switching**:
   - Press `Ctrl+Shift+D` (or click the sun/moon icon in the top-right header) at any time to switch smoothly between **Executive Dark Mode** and **Crisp Light Mode**.

---

## 3. Global Hotkeys & Command Palette

NEXUS registers system-wide shortcuts for rapid keyboard-driven navigation:

| Shortcut | Action |
| :--- | :--- |
| `Ctrl + Space` / `Ctrl + P` | Summon **Global Command Palette & Universal Search** |
| `Ctrl + Double Space` | Open **Custom Command Manager & App Registry** |
| `Ctrl + 1` … `Ctrl + 9` | Jump directly to sidebar routes (`Dashboard` through `Settings`) |
| `Alt + 1` … `Alt + 5` | Switch sub-tabs within the active module |
| `Ctrl + Shift + S` | Launch interactive rectangular region screenshot snip |
| `PrtScn` | Capture full desktop screenshot to clipboard & Screen Studio |
| `Ctrl + Shift + R` | Start / Stop MP4 screen video recording |
| `Ctrl + Shift + D` | Toggle Dark / Light visual theme |
| `F1` / `Ctrl + /` | Open contextual **Keyboard Shortcuts Cheat Sheet** |

---

## 4. Using Core Modules

> **Full Visual Tour Available:** See [README.md - Visual Tour & Demo Walkthrough](README.md#-visual-tour--demo-walkthrough-from-dashboard-to-settings) for complete annotated screenshots and walkthroughs of every page and sub-tab.

### Telemetry Dashboard & Quick Controls
- Press `Ctrl+1` to view real-time CPU & RAM wave charts, logical core metrics, battery status, and drive health bars.
- Drag the **System Volume** and **Display Brightness** sliders for instant two-way Windows synchronization, or toggle **Keep Awake** and **Power Saver** with one click.

### Applications Catalog & Process Manager
- Press `Ctrl+2` then `Alt+1` (**Installed Apps**) to search installed 32-bit/64-bit programs, launch apps, or trigger official Windows uninstallers.
- Press `Alt+2` (**Process Manager**) to monitor live CPU% and RAM usage per process. Press `Space` to freeze updates or `Delete` to terminate an unresponsive task.

### Tabbed File Explorer & Inspector
- Press `Ctrl+3` to browse drives and favorite folders across multiple tabs (`Ctrl+N` new tab, `Ctrl+W` close tab).
- Press `Ctrl+I` to open the **Metadata & Checksum Inspector**, `Ctrl+H` to toggle hidden files, and `Ctrl+Shift+T` to launch a terminal in the active folder.

### Screen Studio, MP4 Recorder & Android Mirroring
- Press `Ctrl+4` to open **Screen Studio & Recorder**.
- **Desktop Screen Studio**: Capture full monitors or custom regions, draw vector shapes/arrows, apply privacy blur redactions, pick pixel hex colors, and record `.mp4` screen videos.
- **Connected Device (`scrcpy`)**: Connect an Android phone with **USB Debugging** enabled via USB or Wi-Fi (`IP:5555`) to mirror and control the device at 60+ FPS.

### Storage Suite (TreeMap, Duplicates, Renamer, Hashes & Cleaner)
- Press `Ctrl+5` to access the 5-tool Storage Center:
  - `Alt+1` **Disk TreeMap**: Click **Browse Folder** (`Ctrl+O`) to visualize space usage as an interactive squarified block map.
  - `Alt+2` **Duplicate Finder**: Detect byte-identical duplicates via progressive 3-stage hashing and safely clean redundant copies.
  - `Alt+3` **File Renamer**: Standardize messy filenames in bulk with live Before/After previews and 1-click batch undo.
  - `Alt+4` **File Hashes**: Compute `SHA-256`, `SHA-1`, `MD5`, and `SHA-512` digests and compare against expected release hashes.
  - `Alt+5` **Junk Cleaner**: Scan and purge Windows Temp, User Temp, browser caches, Prefetch, and crash dumps.

### Network Center & Diagnostics
- Press `Ctrl+6` to inspect active TCP/UDP connections mapped to owning PIDs (`Alt+1`), or switch to **Network Diagnostics** (`Alt+2`) to run **ICMP Ping**, **DNS Benchmarks**, and **Traceroute**.

### Hardware Devices & Driver Health
- Press `Ctrl+7` to audit connected hardware peripherals by category, check driver status and Config Manager problem codes, or open Windows Device Manager.

### Settings Applets, Custom Commands & Audit Logs
- Press `Ctrl+8` (**How to Use**) for built-in page guides, shortcut search, and the live command syntax simulator.
- Press `Ctrl+9` (**Settings**) to launch 50+ native `ms-settings:*` Windows applets, register custom CLI commands/aliases, and inspect or export the SQLite **Administrative Audit Trail** as JSON.

---

## 5. Troubleshooting

| Issue | Cause | Solution |
| :--- | :--- | :--- |
| **Windows SmartScreen prompt on install** | Unsigned community installer | Click **More info** > **Run anyway**. Verify SHA-256 hash in `installer/SHA256SUMS.txt`. |
| **Global hotkey (`Ctrl+Space`) doesn't trigger** | Another launcher holds the hotkey or elevated app has focus | Use `Ctrl+P` inside NEXUS, or run NEXUS with matching privilege level. |
| **Android device not listed in Screen Studio (`scrcpy`)** | USB Debugging disabled or unauthorized | Enable **Developer Options > USB Debugging** on your phone, replug USB, and tap **Allow** on the prompt. |
| **Some Windows Temp files skipped during cleanup** | Files locked by active Windows services | Normal safe behavior — NEXUS skips locked in-use system files to ensure OS stability. |
| **Closing `[X]` minimizes instead of quitting** | System Tray persistence is enabled | Right-click the NEXUS tray icon and click **Exit**, or toggle off **System Tray** in **Settings > General Preferences**. |

---
*For release history and version checksums, see [CHANGELOG.md](CHANGELOG.md) and [installer/SHA256SUMS.txt](installer/SHA256SUMS.txt).*
