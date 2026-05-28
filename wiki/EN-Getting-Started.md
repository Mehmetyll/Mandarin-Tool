**🇺🇸 EN - Getting Started** · [🇹🇷 TR - Başlangıç](TR-Baslangic)

# 🚀 Getting Started

## Prerequisites

| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| **Java (JDK)** | 21 | 21+ (latest LTS) |
| **Operating System** | Windows 10 | Windows 10/11 |


> **⚠️ Important:** MandarinTool is designed for **Windows** and relies on Windows-specific APIs (Registry, Prefetch, USN Journal, Event Logs, etc.). Running on Linux/macOS will result in limited functionality.

---

## Download

1. Go to the [Releases page](https://github.com/Mehmetyll/Mandarin-Tool/releases)
2. Download the latest `MandarinTool.jar`
3. Place it anywhere on your system (e.g., `C:\Tools\MandarinTool\`)

---

## Running MandarinTool

### Option 1: Command Prompt (Recommended)

Open **CMD as Administrator** and run:

```bash
java -jar MandarinTool.jar
```

> **💡 Tip:** Running as Administrator unlocks all features. Without admin privileges, some modules (USN Journal, certain Registry keys, Prefetch parsing) will have limited or no results.

### Option 2: Double-click

If your system has `.jar` files associated with Java, you can simply double-click `MandarinTool.jar`. However, this will **not** grant Administrator privileges, so some features may be restricted.

---

## First Launch

When you first open MandarinTool, you'll see a **Welcome Dialog** with three tabs:

| Tab | Content |
|-----|---------|
| **⚠️ Important** | Warnings about admin privileges and usage notes |
| **📖 Usage** | Quick guide on how to use the main features |
| **ℹ️ Info** | Version info, credits, and project details |

You can also **select your language** from the dropdown in this dialog before closing it.

### Admin Privilege Warning

If MandarinTool detects it's **not** running as Administrator, it will show a warning popup listing the features that require elevation:

- Prefetch file parsing
- USN Journal scanning
- Certain Registry hive access
- Service enumeration
- Event Log deep queries
- USB history via event logs

---

## Application Layout

MandarinTool has **5 main tabs** across the top:

```
Manual Analyze  │ Auto Analyze  │ Scripts │  Download  │ Settings │
```

| Tab | Purpose |
|-----|---------|
| **Manual Analyze** | Mod scanning, class search, JAR analyzer, Zimmerman assistant |
| **Auto Analyze** | 14 one-click forensic sub-modules |
| **Scripts** | Run community PowerShell scripts |
| **Download** | Download and manage forensic tools from various creators |
| **Settings** | Theme selection, language preferences |

Each tab is described in detail in its own wiki page.

---

## Next Steps

- 📂 **[Manual Analyze Tab](EN-Manual-Analyze)** — Start scanning for mods and suspicious files
- 🔍 **[Auto Analyze Tab](EN-Auto-Analyze)** — Run forensic scans with one click
- 🧰 **[Tool Downloader](EN-Tool-Downloader)** — Download community forensic tools
