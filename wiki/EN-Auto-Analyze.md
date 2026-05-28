**🇺🇸 EN - Auto** · [🇹🇷 TR - Otomatik](TR-Otomatik-Analiz)

# 🔍 Auto Analyze Tab

Contains **14 forensic scans** that check different parts of the system. Click any sub-tab to run it individually, or click **Analyze All** to run everything at once.

```
Prefetch · USN · JVM · Event Log · Services · Registry · Site Bypass · USB · Recent · CLI · PowerShell · Crash Dumps · Recycle Bin · Alt Checker · Analyze All
```

> ⚠️ Some modules need Admin privileges to work properly.

---

## What Each Module Does

| Module | What it checks |
|--------|---------------|
| **Prefetch** | Program execution history from Windows Prefetch files |
| **USN Journal** | File creation/deletion/rename events from the NTFS journal |
| **JVM** | Running Java processes, loaded agents, classpath info |
| **Event Log** | Windows Event Log entries related to program execution ⚠️ |
| **Services** | Installed Windows services and their executable paths |
| **Registry** | Registry keys used for persistence and program tracking |
| **Site Bypass** | Hosts file changes, DNS/proxy modifications |
| **USB** | USB device connection history (serial, timestamps, drive letters) |
| **Recent Files** | Recently opened files |
| **CLI** | Command Prompt history |
| **PowerShell** | PowerShell command history |
| **Crash Dumps** | Crashed program reports and dump files |
| **Recycle Bin** | Deleted files with original name, path, and timestamp |
| **Alt Checker** | Alternative accounts on Lunar, Feather, SKlauncher, Vanilla |

---

## ⚠️ JVM Analyze — Important Note

**Modrinth**, **Badlion Client** and **SKlauncher** can cause false positives in JVM Analyze results.(Injection Detected log) Some of their normal activity looks suspicious to automated checks. (Tested clients: Vanilla, Lunar, Feather, Prism, Norisk etc.)

**However, it's NOT a false flag if:**
- The result directly names a cheat/hack (e.g., `Wurst`, `Meteor`)
- The result shows suspicious indicators as "+ Suspect Detected"

If you only see Modrinth/SKlauncher entries (Injection Detected log) with no cheat names → likely clean. If you see cheat names in the results or "+ Suspect Detected" → very high probability of real detection.

Additionally, if you see "Bypass Detected" in the results, its suspected for trying to bypass. (Lunar Client and Badlion Client could false this)
