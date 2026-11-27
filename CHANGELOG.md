# 📋 NEXUS Control Center Changelog & Release Notes

All notable changes to the **NEXUS Control Center** application are documented in this file.

---

## [1.0.0] - Initial Production Release (Windows 64-bit)

### 🚀 Highlights
- **First Official Production Release** of **NEXUS Control Center** ("One laptop. One control center.") for Windows 10 & Windows 11 (64-bit / x64).
- Self-contained standalone Windows installer (`NEXUS-Setup-v1.0.0.exe`, ~76.6 MB) verified with SHA-256 integrity checksums in `installer/SHA256SUMS.txt`.
- **100% Local-First, Zero-Telemetry Architecture** backed by an embedded WAL-mode SQLite persistence engine (`nexus.db` & `nexus_search.db`) and automatic background working-set RAM trimming (~90%+ reduction when minimized to tray).
- **Dual Executive Themes**: Instant animated runtime switching (`Ctrl+Shift+D`) between **Executive Dark Mode** and **Crisp Light Mode** without application restarts, plus English and Khmer (`Kantumruy Pro`) typography support.

### 📊 System Telemetry, Applications & Productivity
- **Executive Telemetry Dashboard**: Real-time 1,000 ms CPU & RAM wave graphs, processor core/frequency breakdown, two-way Windows Volume & Display Brightness sliders, Keep Awake toggle, Battery & Power Saver control, and multi-drive health cards.
- **Installed Applications Catalog**: Unified inventory of 32-bit and 64-bit desktop software with publisher/version filtering, 1-click app launching, and native Windows uninstaller triggers.
- **Live Process Manager**: Asynchronous Windows task telemetry sorting by CPU%, RAM working set, threads, and PID, with `Space` stream freeze and safe process termination.
- **Tabbed File Explorer**: Multi-tab filesystem browser (`Ctrl+N` / `Ctrl+W`) with persistent favorites, directory tree, instant filename filter (`Ctrl+F`), live Metadata & SHA-256 Inspector (`Ctrl+I`), Clipboard History card, hidden files toggle (`Ctrl+H`), and 1-click PowerShell/Terminal launch (`Ctrl+Shift+T`).
- **Global Command Palette & Universal Search**: Spotlight/Raycast-inspired floating launcher (`Ctrl+Space` / `Ctrl+P` / `Ctrl+Double Space`) indexing installed apps, files, folders, custom CLI aliases, and Windows settings with fuzzy scoring.

### 📸 Screen Studio, Recording & Mobile Mirroring
- **Desktop Screen Studio & Recorder**: Interactive rectangular region snip (`Ctrl+Shift+S`), fullscreen capture (`PrtScn`), vector annotations, privacy blur/redaction brush, pixel color picker, MP4 screen video recorder (`Ctrl+Shift+R`) with live elapsed timer, and Saved Captures Gallery.
- **Connected Device Mirror (`scrcpy`)**: Low-latency USB and wireless Wi-Fi ADB Android screen mirroring with touch gestures, hardware navigation toolbar, framerate/bitrate tuning, and audio forwarding.

### 🗄️ Storage Optimization & Cryptographic Integrity
- **Interactive Disk TreeMap**: Squarified `O(N)` block TreeMap (`Bruls et al.`) visualizing disk space consumption across directories with drill-down navigation and top space consumer rankings.
- **3-Stage Duplicate File Finder**: Progressive size, partial edge-hash, and full cryptographic hash deduplication with smart cleanup suggestions and crash-resilient batch undo journal.
- **File Organizer & Batch Renamer**: Rule-based filename standardization, magic-byte & extension categorization, editable Before/After diff previews, and 1-click transactional rollback.
- **Cryptographic Hash Calculator & Verifier**: Streaming `64 KiB` constant-memory digest computation (`SHA-256`, `SHA-1`, `MD5`, `SHA-512`) with instant expected-checksum verification and file-to-file binary comparison.
- **Windows Junk & Temp Cleaner**: Proportional color-mapped scanner and safe cleaner across Windows Temp, User Temp, browser caches, Prefetch, and crash dumps.

### 🌐 Networking, Hardware & System Administration
- **Network Center & Diagnostics Suite**: Live TCP/UDP socket-to-process correlation table alongside an integrated ICMP Ping tester, DNS Resolver Benchmark, and multi-hop Traceroute engine.
- **Hardware Device & Driver Inspector**: Categorized WMI peripheral inventory, driver health verification, Config Manager problem-code diagnostics, and 1-click Windows Device Manager deep-links.
- **Interactive Operational Guide & Settings Hub**: Built-in **How to Use** manual, searchable master Keyboard Shortcuts cheatsheet (`F1`), interactive Command Simulator, 50+ validated `ms-settings:*` Windows 10/11 deep-link applets, Custom Command & Application Registry, and immutable SQLite **Administrative Audit Trail** with JSON export.

---
